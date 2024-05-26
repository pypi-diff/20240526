# Comparing `tmp/ffun-1.5.4.tar.gz` & `tmp/ffun-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.5.4.tar", max compression
+gzip compressed data, was "ffun-1.5.5.tar", max compression
```

## Comparing `ffun-1.5.4.tar` & `ffun-1.5.5.tar`

### file list

```diff
@@ -1,235 +1,235 @@
--rw-r--r--   0        0        0      344 2024-05-23 16:38:10.122613 ffun-1.5.4/README.md
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/__init__.py
--rw-r--r--   0        0        0    10256 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/entities.py
--rw-r--r--   0        0        0    13637 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/http_handlers.py
--rw-r--r--   0        0        0      245 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/application.py
--rw-r--r--   0        0        0      439 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0      538 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/meta.py
--rw-r--r--   0        0        0     1001 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1333 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/migrations.py
--rw-r--r--   0        0        0     4019 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     4551 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     6690 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     4096 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      826 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1937 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0      561 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
--rw-r--r--   0        0        0      531 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
--rw-r--r--   0        0        0      725 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
--rw-r--r--   0        0        0     4062 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0     1178 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     7782 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      553 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     2326 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/tests/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3759 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     3035 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     4104 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/__init__.py
--rw-r--r--   0        0        0     1509 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/entities.py
--rw-r--r--   0        0        0      149 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/errors.py
--rw-r--r--   0        0        0     1498 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     1003 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
--rw-r--r--   0        0        0     1194 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
--rw-r--r--   0        0        0      784 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
--rw-r--r--   0        0        0     5926 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1663 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    15331 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/background_loader.py
--rw-r--r--   0        0        0     5498 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/domain.py
--rw-r--r--   0        0        0       82 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/entities.py
--rw-r--r--   0        0        0      226 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/errors.py
--rw-r--r--   0        0        0      738 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py
--rw-r--r--   0        0        0     9568 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/operations.py
--rw-r--r--   0        0        0      647 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     9569 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0     3558 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/__init__.py
--rw-r--r--   0        0        0      504 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     2447 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/tests/__init__.py
--rw-r--r--   0        0        0     4835 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/__init__.py
--rw-r--r--   0        0        0     3557 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/domain.py
--rw-r--r--   0        0        0      345 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
--rw-r--r--   0        0        0      246 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/tests/__init__.py
--rw-r--r--   0        0        0    15939 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     6307 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      834 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0      408 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/helpers.py
--rw-r--r--   0        0        0     9964 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/domain.py
--rw-r--r--   0        0        0      567 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2362 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6810 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0      348 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/make.py
--rw-r--r--   0        0        0     4263 2024-05-23 16:38:17.154599 ffun-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-05-26 12:46:22.081357 ffun-1.5.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10256 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/api/entities.py
+-rw-r--r--   0        0        0    13637 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0      245 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/api/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1333 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/entities.py
+-rw-r--r--   0        0        0      552 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/register.py
+-rw-r--r--   0        0        0     1442 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     5031 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6690 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     4096 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1937 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      641 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0      531 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      810 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3759 2024-05-26 12:46:22.081357 ffun-1.5.5/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3035 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     4104 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1509 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/errors.py
+-rw-r--r--   0        0        0     1498 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1288 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      710 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1194 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5926 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15331 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/__init__.py
+-rw-r--r--   0        0        0     1218 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0     5498 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/domain.py
+-rw-r--r--   0        0        0       82 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/entities.py
+-rw-r--r--   0        0        0      226 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/errors.py
+-rw-r--r--   0        0        0      738 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py
+-rw-r--r--   0        0        0     9639 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/operations.py
+-rw-r--r--   0        0        0      647 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     9569 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0     6941 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/loader/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/entities.py
+-rw-r--r--   0        0        0      855 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     3557 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/domain.py
+-rw-r--r--   0        0        0      345 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0      246 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    15939 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      520 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      799 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1008 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1919 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2833 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.085357 ffun-1.5.5/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      567 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2362 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      966 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/errors.py
+-rw-r--r--   0        0        0      865 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/errors.py
+-rw-r--r--   0        0        0      851 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      732 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      534 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/errors.py
+-rw-r--r--   0        0        0      718 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-05-26 12:46:22.089357 ffun-1.5.5/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4326 2024-05-26 12:46:30.317376 ffun-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 ffun-1.5.5/PKG-INFO
```

### Comparing `ffun-1.5.4/ffun/api/entities.py` & `ffun-1.5.5/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/api/http_handlers.py` & `ffun-1.5.5/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/application/application.py` & `ffun-1.5.5/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/application/settings.py` & `ffun-1.5.5/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/application/user_settings.py` & `ffun-1.5.5/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/application/workers.py` & `ffun-1.5.5/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/auth/dependencies.py` & `ffun-1.5.5/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/auth/settings.py` & `ffun-1.5.5/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/auth/supertokens.py` & `ffun-1.5.5/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/configs.py` & `ffun-1.5.5/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/entries.py` & `ffun-1.5.5/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/failed_entries.py` & `ffun-1.5.5/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/meta.py` & `ffun-1.5.5/ffun/cli/commands/meta.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/supertokens.py` & `ffun-1.5.5/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/cli/commands/workers.py` & `ffun-1.5.5/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/conftest.py` & `ffun-1.5.5/ffun/conftest.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/api.py` & `ffun-1.5.5/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/background_tasks.py` & `ffun-1.5.5/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/errors.py` & `ffun-1.5.5/ffun/core/errors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/json.py` & `ffun-1.5.5/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/logging.py` & `ffun-1.5.5/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/middlewares.py` & `ffun-1.5.5/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/migrations.py` & `ffun-1.5.5/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/postgresql.py` & `ffun-1.5.5/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/register.py` & `ffun-1.5.5/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/sentry.py` & `ffun-1.5.5/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/core/tests/helpers.py` & `ffun-1.5.5/ffun/core/tests/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -151,7 +151,19 @@
     found_enents = Counter(log["event"] for log in logs)
 
     for key, expected_count in kwargs.items():
         if expected_count != found_enents.get(key, 0):
             pytest.fail(
                 f"Key {key} not found {expected_count} times in logs, but found {found_enents.get(key, 0)} times"
             )
+
+
+def assert_logs_levels(logs: list[MutableMapping[str, Any]], **kwargs: str) -> None:
+    for record in logs:
+        if record["event"] in kwargs:
+            assert record["log_level"] == kwargs[record["event"]], f"Log level is not equal to expected for {record}"
+
+
+def assert_logs_have_no_errors(logs: list[MutableMapping[str, Any]]) -> None:
+    for record in logs:
+        if record["log_level"].lower() == "error":
+            pytest.fail(f"Error found in logs: {record}")
```

### Comparing `ffun-1.5.4/ffun/core/utils.py` & `ffun-1.5.5/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/domain/tests/test_urls.py` & `ffun-1.5.5/ffun/domain/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/domain/urls.py` & `ffun-1.5.5/ffun/domain/urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/domain.py` & `ffun-1.5.5/ffun/feeds/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/entities.py` & `ffun-1.5.5/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.5.5/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.5.5/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py` & `ffun-1.5.5/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py` & `ffun-1.5.5/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py` & `ffun-1.5.5/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/operations.py` & `ffun-1.5.5/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/tests/fixtures.py` & `ffun-1.5.5/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/tests/make.py` & `ffun-1.5.5/ffun/feeds/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds/tests/test_operations.py` & `ffun-1.5.5/ffun/feeds/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.5.5/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_collections/domain.py` & `ffun-1.5.5/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_collections/predefines.py` & `ffun-1.5.5/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.5.5/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_discoverer/domain.py` & `ffun-1.5.5/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_links/domain.py` & `ffun-1.5.5/ffun/feeds_links/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.5.5/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_links/operations.py` & `ffun-1.5.5/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/feeds_links/tests/test_operations.py` & `ffun-1.5.5/ffun/feeds_links/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/background_processors.py` & `ffun-1.5.5/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/domain.py` & `ffun-1.5.5/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.5.5/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.5.5/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/operations.py` & `ffun-1.5.5/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/processors/base.py` & `ffun-1.5.5/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/processors/domain.py` & `ffun-1.5.5/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.5.5/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.5.5/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.5.5/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/settings.py` & `ffun-1.5.5/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/tests/fixtures.py` & `ffun-1.5.5/ffun/librarian/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/tests/make.py` & `ffun-1.5.5/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/tests/test_background_processors.py` & `ffun-1.5.5/ffun/librarian/tests/test_background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/tests/test_domain.py` & `ffun-1.5.5/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/librarian/tests/test_operations.py` & `ffun-1.5.5/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/domain.py` & `ffun-1.5.5/ffun/library/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/entities.py` & `ffun-1.5.5/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.5.5/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.5.5/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.5.5/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.5.5/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py` & `ffun-1.5.5/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py` & `ffun-1.5.5/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py` & `ffun-1.5.5/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/operations.py` & `ffun-1.5.5/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/tests/fixtures.py` & `ffun-1.5.5/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/tests/make.py` & `ffun-1.5.5/ffun/library/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/tests/test_domain.py` & `ffun-1.5.5/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/library/tests/test_operations.py` & `ffun-1.5.5/ffun/library/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/loader/background_loader.py` & `ffun-1.5.5/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/loader/domain.py` & `ffun-1.5.5/ffun/loader/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py` & `ffun-1.5.5/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/loader/operations.py` & `ffun-1.5.5/ffun/loader/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 from ffun.loader.settings import Proxy
 from ffun.parsers import entities as p_entities
 from ffun.parsers.domain import parse_feed
 
 logger = logging.get_module_logger()
 
 
-# TODO: tests
 async def load_content(  # noqa: CFQ001, CCR001, C901 # pylint: disable=R0912, R0915
     url: str, proxy: Proxy, user_agent: str
 ) -> httpx.Response:
     error_code = FeedError.network_unknown
 
     log = logger.bind(url=url, proxy=proxy.name, function="load_content")
 
     try:
         log.info("loading_feed")
 
-        async with httpx.AsyncClient(proxies=proxy.url, headers={"user-agent": user_agent}) as client:
+        headers = {"user-agent": user_agent, "accept-encoding": "br;q=1.0, gzip;q=0.9, deflate;q=0.8"}
+
+        async with httpx.AsyncClient(proxies=proxy.url, headers=headers) as client:
             response = await client.get(url, follow_redirects=True)
 
     except httpx.RemoteProtocolError as e:
         message = str(e)
 
         if "illegal request line" in message:
             # TODO: at least part of such errors are caused by wrong HTTP protocol
```

### Comparing `ffun-1.5.4/ffun/loader/settings.py` & `ffun-1.5.5/ffun/loader/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/loader/tests/test_domain.py` & `ffun-1.5.5/ffun/loader/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.5.5/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/markers/operations.py` & `ffun-1.5.5/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/markers/tests/test_operations.py` & `ffun-1.5.5/ffun/markers/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/meta/domain.py` & `ffun-1.5.5/ffun/meta/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/meta/tests/test_domain.py` & `ffun-1.5.5/ffun/meta/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/domain.py` & `ffun-1.5.5/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/entities.py` & `ffun-1.5.5/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.5.5/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.5.5/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.5.5/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.5.5/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/operations.py` & `ffun-1.5.5/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/tests/fixtures.py` & `ffun-1.5.5/ffun/ontology/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/ontology/tests/test_operations.py` & `ffun-1.5.5/ffun/ontology/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/client.py` & `ffun-1.5.5/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/entities.py` & `ffun-1.5.5/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/keys_rotator.py` & `ffun-1.5.5/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/keys_statuses.py` & `ffun-1.5.5/ffun/openai/keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/tests/fixtures.py` & `ffun-1.5.5/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.5.5/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.5.5/ffun/openai/tests/test_keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/entities.py` & `ffun-1.5.5/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/feed.py` & `ffun-1.5.5/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/feedly.py` & `ffun-1.5.5/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.5.5/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/make.py` & `ffun-1.5.5/ffun/parsers/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/parsers/tests/test_feed.py` & `ffun-1.5.5/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/resources/domain.py` & `ffun-1.5.5/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.5.5/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/resources/operations.py` & `ffun-1.5.5/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/resources/tests/test_domain.py` & `ffun-1.5.5/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/resources/tests/test_operations.py` & `ffun-1.5.5/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/domain.py` & `ffun-1.5.5/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.5.5/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.5.5/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/operations.py` & `ffun-1.5.5/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/tests/test_domain.py` & `ffun-1.5.5/ffun/scores/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/scores/tests/test_operations.py` & `ffun-1.5.5/ffun/scores/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/tags/converters.py` & `ffun-1.5.5/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/tags/tests/test_converters.py` & `ffun-1.5.5/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/domain.py` & `ffun-1.5.5/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.5.5/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.5.5/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/operations.py` & `ffun-1.5.5/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/settings.py` & `ffun-1.5.5/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/tests/test_domain.py` & `ffun-1.5.5/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/tests/test_operations.py` & `ffun-1.5.5/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/user_settings/types.py` & `ffun-1.5.5/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/users/domain.py` & `ffun-1.5.5/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.5.5/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/users/operations.py` & `ffun-1.5.5/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/ffun/users/tests/fixtures.py` & `ffun-1.5.5/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.4/pyproject.toml` & `ffun-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.5.4"
+version = "1.5.5"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
@@ -38,15 +38,18 @@
 python = "^3.11"
 
 uvicorn = {extras = ["standard"], version = "0.*"}
 fastapi = "0.103.*"
 pydantic = "2.4.*"
 pydantic-settings = "2.0.*"
 typer = "0.9.*"
+
 httpx = "0.24.*"
+brotlicffi = "1.1.*"
+# zstandard = "0.22.*"
 
 openai = "0.27.*"
 tiktoken = "0.4.*"
 
 bidict = "0.22.*"
 
 feedparser = "6.0.*"
@@ -82,14 +85,16 @@
 
 [tool.poetry.dev-dependencies]
 
 pytest = "7.4.*"
 pytest-asyncio = "0.21.*"
 pytest-mock = "3.11.*"
 
+respx = "0.21.*"
+
 isort = "5.12.*"
 black = "23.7.*"
 
 flake8 = "6.1.*"
 flake8-docstrings = "1.7.*"
 flake8-functions = "0.0.*"
 flake8-annotations-complexity = "0.0.*"
```

### Comparing `ffun-1.5.4/PKG-INFO` & `ffun-1.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.5.4
+Version: 1.5.5
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -31,14 +31,15 @@
 Classifier: Topic :: Office/Business :: News/Diary
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: PyPika (==0.48.*)
 Requires-Dist: async-lru (==2.0.*)
 Requires-Dist: beautifulsoup4 (==4.12.*)
 Requires-Dist: bidict (==0.22.*)
+Requires-Dist: brotlicffi (==1.1.*)
 Requires-Dist: cryptography (==41.0.*)
 Requires-Dist: fastapi (==0.103.*)
 Requires-Dist: feedparser (==6.0.*)
 Requires-Dist: furl (==2.1.*)
 Requires-Dist: httpx (==0.24.*)
 Requires-Dist: markdown (==3.4.*)
 Requires-Dist: openai (==0.27.*)
```

