# Comparing `tmp/khoj_assistant-1.9.1.dev74.tar.gz` & `tmp/khoj_assistant-1.9.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr 11 18:38:29 2024, max compression
+gzip compressed data, last modified: Mon Apr  8 06:13:34 2024, max compression
```

## Comparing `khoj_assistant-1.9.1.dev74.tar` & `khoj_assistant-1.9.1.dev8.tar`

### file list

```diff
@@ -1,188 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/__init__.py
--rw-r--r--   0        0        0    14279 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/configure.py
--rw-r--r--   0        0        0     5330 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/main.py
--rwxr-xr-x   0        0        0      664 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/manage.py
--rw-r--r--   0        0        0     2832 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/app/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/app/__init__.py
--rw-r--r--   0        0        0     4587 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/app/settings.py
--rw-r--r--   0        0        0      869 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/app/urls.py
--rw-r--r--   0        0        0      388 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/__init__.py
--rw-r--r--   0        0        0     5531 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/admin.py
--rw-r--r--   0        0        0      153 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/apps.py
--rw-r--r--   0        0        0       60 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/tests.py
--rw-r--r--   0        0        0    33920 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/adapters/__init__.py
--rw-r--r--   0        0        0     4077 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0001_khojuser.py
--rw-r--r--   0        0        0     1195 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0002_googleuser.py
--rw-r--r--   0        0        0      224 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0003_vector_extension.py
--rw-r--r--   0        0        0     8202 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0004_content_types_and_more.py
--rw-r--r--   0        0        0      429 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0005_embeddings_corpus_id.py
--rw-r--r--   0        0        0     1131 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0006_embeddingsdates.py
--rw-r--r--   0        0        0      917 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0007_add_conversation.py
--rw-r--r--   0        0        0      399 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
--rw-r--r--   0        0        0      876 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0009_khojapiuser.py
--rw-r--r--   0        0        0     3347 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
--rw-r--r--   0        0        0      773 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
--rw-r--r--   0        0        0      331 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0011_merge_20231102_0138.py
--rw-r--r--   0        0        0      552 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0012_entry_file_source.py
--rw-r--r--   0        0        0     1311 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0013_subscription.py
--rw-r--r--   0        0        0      411 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0014_alter_googleuser_picture.py
--rw-r--r--   0        0        0      584 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0015_alter_subscription_user.py
--rw-r--r--   0        0        0      429 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
--rw-r--r--   0        0        0     1219 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0017_searchmodel.py
--rw-r--r--   0        0        0     1152 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
--rw-r--r--   0        0        0      843 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
--rw-r--r--   0        0        0     1190 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0020_reflectivequestion.py
--rw-r--r--   0        0        0     1504 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
--rw-r--r--   0        0        0      904 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
--rw-r--r--   0        0        0     1122 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0023_usersearchmodelconfig.py
--rw-r--r--   0        0        0      405 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0024_alter_entry_embeddings.py
--rw-r--r--   0        0        0     1573 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
--rw-r--r--   0        0        0      691 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      731 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      375 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0027_merge_20240118_1324.py
--rw-r--r--   0        0        0      405 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
--rw-r--r--   0        0        0      934 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0029_userrequests.py
--rw-r--r--   0        0        0     1252 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0030_conversation_slug_and_title.py
--rw-r--r--   0        0        0     2033 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0031_agent_conversation_agent.py
--rw-r--r--   0        0        0      812 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0031_alter_googleuser_locale.py
--rw-r--r--   0        0        0      317 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0032_merge_20240322_0427.py
--rw-r--r--   0        0        0      369 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
--rw-r--r--   0        0        0     1251 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/__init__.py
--rw-r--r--   0        0        0    11129 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/database/models/__init__.py
--rw-r--r--   0        0        0     6577 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/email/welcome.html
--rw-r--r--   0        0        0     1651 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     8953 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/agent.html
--rw-r--r--   0        0        0     6672 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/agents.html
--rw-r--r--   0        0        0    11089 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0   112686 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    38365 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     5367 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_computer_input.html
--rw-r--r--   0        0        0     7225 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_github_input.html
--rw-r--r--   0        0        0     3497 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_notion_input.html
--rw-r--r--   0        0        0     1628 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0     4218 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/login.html
--rw-r--r--   0        0        0     2910 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0    18326 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/search.html
--rw-r--r--   0        0        0     2690 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/utils.html
--rw-r--r--   0        0        0     5504 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73396 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0     1222 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/utils.js
--rw-r--r--   0        0        0     1722 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/agents.svg
--rw-r--r--   0        0        0     2424 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0    10517 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/computer.png
--rw-r--r--   0        0        0      549 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0      829 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/copy-button-success.svg
--rw-r--r--   0        0        0      669 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/copy-button.svg
--rw-r--r--   0        0        0      503 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/copy-solid.svg
--rw-r--r--   0        0        0    19662 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/credit-card.png
--rw-r--r--   0        0        0   205167 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    30234 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-256x256.png
--rw-r--r--   0        0        0    31531 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0     1100 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/key.svg
--rw-r--r--   0        0        0    13011 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0    29856 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
--rw-r--r--   0        0        0  1301428 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0      616 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/microphone-solid.svg
--rw-r--r--   0        0        0     1578 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     1736 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/openai-logomark.svg
--rw-r--r--   0        0        0     7946 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     2945 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/plaintext.svg
--rw-r--r--   0        0        0     1877 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0     1210 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/search.svg
--rw-r--r--   0        0        0     1319 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/stop-solid.svg
--rw-r--r--   0        0        0      503 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/trash-solid.svg
--rw-r--r--   0        0        0     2233 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/user-silhouette.svg
--rw-r--r--   0        0        0      951 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/web.svg
--rw-r--r--   0        0        0     2417 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/whatsapp.svg
--rw-r--r--   0        0        0   591182 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
--rw-r--r--   0        0        0   197173 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
--rw-r--r--   0        0        0   268309 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
--rw-r--r--   0        0        0   406179 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
--rw-r--r--   0        0        0    82985 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
--rw-r--r--   0        0        0   236285 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_default_model.py
--rw-r--r--   0        0        0     2034 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_default_model_2.py
--rw-r--r--   0        0        0     2510 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_schema.py
--rw-r--r--   0        0        0      975 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_model.py
--rw-r--r--   0        0        0     2025 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_processor_config_openai.py
--rw-r--r--   0        0        0     5132 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_server_pg.py
--rw-r--r--   0        0        0      569 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_version.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4715 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/__init__.py
--rw-r--r--   0        0        0    13637 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/text_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/github/__init__.py
--rw-r--r--   0        0        0     9775 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/github/github_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/markdown/__init__.py
--rw-r--r--   0        0        0     7007 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/markdown/markdown_to_entries.py
--rw-r--r--   0        0        0     9915 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/notion/notion_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/org_mode/__init__.py
--rw-r--r--   0        0        0     9728 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/org_mode/org_to_entries.py
--rw-r--r--   0        0        0    18476 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/pdf/__init__.py
--rw-r--r--   0        0        0     4494 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/pdf/pdf_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/plaintext/__init__.py
--rw-r--r--   0        0        0     4934 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/content/plaintext/plaintext_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0    21099 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0    10226 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/__init__.py
--rw-r--r--   0        0        0     8555 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/chat_model.py
--rw-r--r--   0        0        0     1793 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/utils.py
--rw-r--r--   0        0        0      470 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/whisper.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/__init__.py
--rw-r--r--   0        0        0     6849 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/gpt.py
--rw-r--r--   0        0        0     3284 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/utils.py
--rw-r--r--   0        0        0      432 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/whisper.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/tools/__init__.py
--rw-r--r--   0        0        0     6663 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/processor/tools/online_search.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    14893 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1443 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/api_agents.py
--rw-r--r--   0        0        0    25874 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/api_chat.py
--rw-r--r--   0        0        0    10826 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/api_config.py
--rw-r--r--   0        0        0     2208 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/api_phone.py
--rw-r--r--   0        0        0     4948 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/auth.py
--rw-r--r--   0        0        0     1067 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/email.py
--rw-r--r--   0        0        0    28684 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0    10958 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/indexer.py
--rw-r--r--   0        0        0     3137 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/notion.py
--rw-r--r--   0        0        0     1151 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/storage.py
--rw-r--r--   0        0        0     4285 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/subscription.py
--rw-r--r--   0        0        0     1081 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/twilio.py
--rw-r--r--   0        0        0    13469 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      358 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0    10101 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0      939 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     1005 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0     8916 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     3466 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     1740 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/config.py
--rw-r--r--   0        0        0      791 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     9919 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/fs_syncer.py
--rw-r--r--   0        0        0    12595 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     7245 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/initialization.py
--rw-r--r--   0        0        0     1192 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2009 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4028 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1309 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1430 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      565 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/.gitignore
--rw-r--r--   0        0        0    34523 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/LICENSE
--rw-r--r--   0        0        0     2612 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/README.md
--rw-r--r--   0        0        0     3571 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/pyproject.toml
--rw-r--r--   0        0        0     6015 2024-04-11 18:38:29.000000 khoj_assistant-1.9.1.dev74/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/__init__.py
+-rw-r--r--   0        0        0    14394 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/configure.py
+-rw-r--r--   0        0        0     5330 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/main.py
+-rwxr-xr-x   0        0        0      664 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/manage.py
+-rw-r--r--   0        0        0     2832 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/settings.py
+-rw-r--r--   0        0        0      869 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/urls.py
+-rw-r--r--   0        0        0      388 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/__init__.py
+-rw-r--r--   0        0        0     5523 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/admin.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/apps.py
+-rw-r--r--   0        0        0       60 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/tests.py
+-rw-r--r--   0        0        0    33625 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/adapters/__init__.py
+-rw-r--r--   0        0        0     4077 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0001_khojuser.py
+-rw-r--r--   0        0        0     1195 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0002_googleuser.py
+-rw-r--r--   0        0        0      224 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0003_vector_extension.py
+-rw-r--r--   0        0        0     8202 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0004_content_types_and_more.py
+-rw-r--r--   0        0        0      429 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0005_embeddings_corpus_id.py
+-rw-r--r--   0        0        0     1131 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0006_embeddingsdates.py
+-rw-r--r--   0        0        0      917 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0007_add_conversation.py
+-rw-r--r--   0        0        0      399 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
+-rw-r--r--   0        0        0      876 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0009_khojapiuser.py
+-rw-r--r--   0        0        0     3347 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
+-rw-r--r--   0        0        0      773 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
+-rw-r--r--   0        0        0      331 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0011_merge_20231102_0138.py
+-rw-r--r--   0        0        0      552 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0012_entry_file_source.py
+-rw-r--r--   0        0        0     1311 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0013_subscription.py
+-rw-r--r--   0        0        0      411 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0014_alter_googleuser_picture.py
+-rw-r--r--   0        0        0      584 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0015_alter_subscription_user.py
+-rw-r--r--   0        0        0      429 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
+-rw-r--r--   0        0        0     1219 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0017_searchmodel.py
+-rw-r--r--   0        0        0     1152 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
+-rw-r--r--   0        0        0      843 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
+-rw-r--r--   0        0        0     1190 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0020_reflectivequestion.py
+-rw-r--r--   0        0        0     1504 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
+-rw-r--r--   0        0        0      904 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
+-rw-r--r--   0        0        0     1122 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0023_usersearchmodelconfig.py
+-rw-r--r--   0        0        0      405 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0024_alter_entry_embeddings.py
+-rw-r--r--   0        0        0     1573 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
+-rw-r--r--   0        0        0      691 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      731 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      375 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0027_merge_20240118_1324.py
+-rw-r--r--   0        0        0      405 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
+-rw-r--r--   0        0        0      934 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0029_userrequests.py
+-rw-r--r--   0        0        0     1252 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0030_conversation_slug_and_title.py
+-rw-r--r--   0        0        0     2033 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_agent_conversation_agent.py
+-rw-r--r--   0        0        0      812 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_alter_googleuser_locale.py
+-rw-r--r--   0        0        0      317 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0032_merge_20240322_0427.py
+-rw-r--r--   0        0        0      369 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
+-rw-r--r--   0        0        0     1251 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/__init__.py
+-rw-r--r--   0        0        0    11129 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/database/models/__init__.py
+-rw-r--r--   0        0        0     1651 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     8953 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agent.html
+-rw-r--r--   0        0        0     6672 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agents.html
+-rw-r--r--   0        0        0    11089 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0   112026 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    38365 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     5367 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_computer_input.html
+-rw-r--r--   0        0        0     7225 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_github_input.html
+-rw-r--r--   0        0        0     3497 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_notion_input.html
+-rw-r--r--   0        0        0     1628 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0     4218 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/login.html
+-rw-r--r--   0        0        0     2910 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0    18326 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/search.html
+-rw-r--r--   0        0        0     2168 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/utils.html
+-rw-r--r--   0        0        0     5160 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73396 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0     1222 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/utils.js
+-rw-r--r--   0        0        0    51584 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0    10517 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/computer.png
+-rw-r--r--   0        0        0      549 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0      503 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/copy-solid.svg
+-rw-r--r--   0        0        0      746 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/copy_button.svg
+-rw-r--r--   0        0        0    19662 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/credit-card.png
+-rw-r--r--   0        0        0   205167 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    30234 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-256x256.png
+-rw-r--r--   0        0        0    31531 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0     1100 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/key.svg
+-rw-r--r--   0        0        0    13011 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0    29856 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
+-rw-r--r--   0        0        0  1301428 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0      616 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/microphone-solid.svg
+-rw-r--r--   0        0        0     1578 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     1736 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/openai-logomark.svg
+-rw-r--r--   0        0        0     7946 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     2945 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/plaintext.svg
+-rw-r--r--   0        0        0     1877 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0     1319 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/stop-solid.svg
+-rw-r--r--   0        0        0      503 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/trash-solid.svg
+-rw-r--r--   0        0        0     2233 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/user-silhouette.svg
+-rw-r--r--   0        0        0      951 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/web.svg
+-rw-r--r--   0        0        0     2417 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/whatsapp.svg
+-rw-r--r--   0        0        0   591182 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
+-rw-r--r--   0        0        0   197173 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
+-rw-r--r--   0        0        0   268309 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
+-rw-r--r--   0        0        0   406179 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
+-rw-r--r--   0        0        0    82985 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
+-rw-r--r--   0        0        0   236285 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model.py
+-rw-r--r--   0        0        0     2034 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model_2.py
+-rw-r--r--   0        0        0     2510 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_schema.py
+-rw-r--r--   0        0        0      975 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_model.py
+-rw-r--r--   0        0        0     2025 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_processor_config_openai.py
+-rw-r--r--   0        0        0     5132 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_server_pg.py
+-rw-r--r--   0        0        0      569 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_version.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/__init__.py
+-rw-r--r--   0        0        0    12604 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/text_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/github/__init__.py
+-rw-r--r--   0        0        0    14040 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/github/github_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/markdown_to_entries.py
+-rw-r--r--   0        0        0     9906 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/notion/notion_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/org_to_entries.py
+-rw-r--r--   0        0        0    18246 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/pdf_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/plaintext/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/content/plaintext/plaintext_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0    21189 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0    10226 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/__init__.py
+-rw-r--r--   0        0        0     8579 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/chat_model.py
+-rw-r--r--   0        0        0     1793 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/utils.py
+-rw-r--r--   0        0        0      470 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/__init__.py
+-rw-r--r--   0        0        0     6896 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/gpt.py
+-rw-r--r--   0        0        0     3284 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/utils.py
+-rw-r--r--   0        0        0      432 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/__init__.py
+-rw-r--r--   0        0        0     5929 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/online_search.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13865 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1443 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_agents.py
+-rw-r--r--   0        0        0    25148 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_chat.py
+-rw-r--r--   0        0        0    10827 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_config.py
+-rw-r--r--   0        0        0     2208 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/api_phone.py
+-rw-r--r--   0        0        0     4569 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/auth.py
+-rw-r--r--   0        0        0    28306 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0    10974 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/indexer.py
+-rw-r--r--   0        0        0     3137 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/notion.py
+-rw-r--r--   0        0        0     1151 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/storage.py
+-rw-r--r--   0        0        0     4285 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/subscription.py
+-rw-r--r--   0        0        0     1081 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/twilio.py
+-rw-r--r--   0        0        0    13329 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0    10101 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0      939 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     1005 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0     8916 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     1740 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/config.py
+-rw-r--r--   0        0        0      791 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     9519 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/fs_syncer.py
+-rw-r--r--   0        0        0    12034 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     7245 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/initialization.py
+-rw-r--r--   0        0        0     1192 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2009 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4028 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1309 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1430 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      565 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/LICENSE
+-rw-r--r--   0        0        0     2378 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/README.md
+-rw-r--r--   0        0        0     3525 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0     5705 2024-04-08 06:13:34.000000 khoj_assistant-1.9.1.dev8/PKG-INFO
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/configure.py` & `khoj_assistant-1.9.1.dev8/src/khoj/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,40 +227,40 @@
                     )
                 }
             )
 
         state.SearchType = configure_search_types()
         state.search_models = configure_search(state.search_models, state.config.search_type)
         setup_default_agent()
-
-        if not init:
-            initialize_content(regenerate, search_type, user)
-
+        initialize_content(regenerate, search_type, init, user)
     except Exception as e:
         raise e
 
 
 def setup_default_agent():
     AgentAdapters.create_default_agent()
 
 
-def initialize_content(regenerate: bool, search_type: Optional[SearchType] = None, user: KhojUser = None):
+def initialize_content(regenerate: bool, search_type: Optional[SearchType] = None, init=False, user: KhojUser = None):
     # Initialize Content from Config
     if state.search_models:
         try:
-            logger.info("📬 Updating content index...")
-            all_files = collect_files(user=user)
-            status = configure_content(
-                all_files,
-                regenerate,
-                search_type,
-                user=user,
-            )
-            if not status:
-                raise RuntimeError("Failed to update content index")
+            if init:
+                logger.info("📬 No-op...")
+            else:
+                logger.info("📬 Updating content index...")
+                all_files = collect_files(user=user)
+                status = configure_content(
+                    all_files,
+                    regenerate,
+                    search_type,
+                    user=user,
+                )
+                if not status:
+                    raise RuntimeError("Failed to update content index")
         except Exception as e:
             raise e
 
 
 def configure_routes(app):
     # Import APIs here to setup search types before while configuring server
     from khoj.routers.api import api
@@ -323,15 +323,15 @@
     # Extract core search types
     core_search_types = {e.name: e.value for e in SearchType}
 
     # Dynamically generate search type enum by merging core search types with configured plugin search types
     return Enum("SearchType", core_search_types)
 
 
-@schedule.repeat(schedule.every(2).minutes)
+@schedule.repeat(schedule.every(5).minutes)
 def upload_telemetry():
     if not state.config or not state.config.app or not state.config.app.should_log_telemetry or not state.telemetry:
         message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
         logger.debug(message)
         return
 
     try:
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/main.py` & `khoj_assistant-1.9.1.dev8/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/manage.py` & `khoj_assistant-1.9.1.dev8/src/khoj/manage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/app/README.md` & `khoj_assistant-1.9.1.dev8/src/khoj/app/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/app/settings.py` & `khoj_assistant-1.9.1.dev8/src/khoj/app/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 ]
 
 COOKIE_SAMESITE = "None"
 if DEBUG or os.getenv("KHOJ_DOMAIN") == None:
     SESSION_COOKIE_DOMAIN = "localhost"
     CSRF_COOKIE_DOMAIN = "localhost"
 else:
-    # Production Settings
     SESSION_COOKIE_DOMAIN = KHOJ_DOMAIN
     CSRF_COOKIE_DOMAIN = KHOJ_DOMAIN
-    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")
+    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTOCOL", "https")
 
 SESSION_COOKIE_SECURE = True
 CSRF_COOKIE_SECURE = True
 COOKIE_SAMESITE = "None"
 SESSION_COOKIE_SAMESITE = "None"
 
 # Application definition
@@ -147,14 +146,14 @@
 USE_TZ = True
 
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/4.2/howto/static-files/
 
 STATIC_ROOT = BASE_DIR / "static"
-STATICFILES_DIRS = [BASE_DIR / "interface/web", BASE_DIR / "interface/email"]
+STATICFILES_DIRS = [BASE_DIR / "interface/web"]
 STATIC_URL = "/static/"
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.2/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/app/urls.py` & `khoj_assistant-1.9.1.dev8/src/khoj/app/urls.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/admin.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "email",
         "username",
         "is_active",
         "is_staff",
         "is_superuser",
         "phone_number",
     )
-    search_fields = ("email", "username", "phone_number", "uuid")
+    search_fields = ("email", "username", "phone_number")
     filter_horizontal = ("groups", "user_permissions")
 
     fieldsets = (("Personal info", {"fields": ("phone_number",)}),) + UserAdmin.fieldsets
 
 
 admin.site.register(KhojUser, KhojUserAdmin)
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/adapters/__init__.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,25 +192,14 @@
     google_profile: GoogleUser = GoogleUser.objects.filter(user=user).first()
     if google_profile:
         return google_profile.given_name
 
     return None
 
 
-def get_user_photo(user: KhojUser):
-    full_name = user.get_full_name()
-    if not is_none_or_empty(full_name):
-        return full_name
-    google_profile: GoogleUser = GoogleUser.objects.filter(user=user).first()
-    if google_profile:
-        return google_profile.picture
-
-    return None
-
-
 def get_user_subscription(email: str) -> Optional[Subscription]:
     return Subscription.objects.filter(user__email=email).first()
 
 
 async def set_user_subscription(
     email: str, is_recurring=None, renewal_date=None, type="standard"
 ) -> Optional[Subscription]:
@@ -803,15 +792,15 @@
         return await Entry.objects.filter(user=user).aexists()
 
     @staticmethod
     async def adelete_entry_by_file(user: KhojUser, file_path: str):
         return await Entry.objects.filter(user=user, file_path=file_path).adelete()
 
     @staticmethod
-    def get_all_filenames_by_source(user: KhojUser, file_source: str):
+    def aget_all_filenames_by_source(user: KhojUser, file_source: str):
         return (
             Entry.objects.filter(user=user, file_source=file_source)
             .distinct("file_path")
             .values_list("file_path", flat=True)
         )
 
     @staticmethod
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0001_khojuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0001_khojuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0002_googleuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0002_googleuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0004_content_types_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0004_content_types_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0006_embeddingsdates.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0006_embeddingsdates.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0007_add_conversation.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0007_add_conversation.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0009_khojapiuser.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0009_khojapiuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0012_entry_file_source.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0012_entry_file_source.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0013_subscription.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0013_subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0015_alter_subscription_user.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0015_alter_subscription_user.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0017_searchmodel.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0017_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0020_reflectivequestion.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0020_reflectivequestion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0022_texttoimagemodelconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0022_texttoimagemodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0023_usersearchmodelconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0023_usersearchmodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0029_userrequests.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0029_userrequests.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0030_conversation_slug_and_title.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0030_conversation_slug_and_title.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0031_agent_conversation_agent.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_agent_conversation_agent.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0031_alter_googleuser_locale.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0031_alter_googleuser_locale.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/database/models/__init__.py` & `khoj_assistant-1.9.1.dev8/src/khoj/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/404.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/agent.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agent.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/agents.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/agents.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/base_config.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/chat.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/chat.html`

 * *Files 1% similar despite different names*

```diff
@@ -26,33 +26,35 @@
 Get the Khoj [Desktop](https://khoj.dev/downloads), [Obsidian](https://docs.khoj.dev/clients/obsidian#setup), [Emacs](https://docs.khoj.dev/clients/emacs#setup) apps to search, chat with your 🖥️ computer docs. You can manage all the files you've shared with me at any time by going to [your settings](/config/content-source/computer/).
 
 To get started, just start typing below. You can also type / to see a list of commands.
 `.trim()
         const allowedExtensions = ['text/org', 'text/markdown', 'text/plain', 'text/html', 'application/pdf'];
         const allowedFileEndings = ['org', 'md', 'txt', 'html', 'pdf'];
         let chatOptions = [];
-        function copyParentText(event) {
+        function copyProgrammaticOutput(event) {
+            // Remove the first 4 characters which are the "Copy" button
             const button = event.currentTarget;
-            const textContent = button.parentNode.textContent.trim();
-            navigator.clipboard.writeText(textContent).then(() => {
-                button.firstChild.src = "/static/assets/icons/copy-button-success.svg";
+            const programmaticOutput = button.parentNode.textContent.trim();
+            navigator.clipboard.writeText(programmaticOutput).then(() => {
+                button.textContent = "✅ Copied to clipboard!";
                 setTimeout(() => {
-                    button.firstChild.src = "/static/assets/icons/copy-button.svg";
+                    button.textContent = "✅";
                 }, 1000);
             }).catch((error) => {
                 console.error("Error copying programmatic output to clipboard:", error);
-                const originalButtonText = button.innerHTML;
-                button.innerHTML = "⛔️";
+                button.textContent = "⛔️ Failed to copy!";
                 setTimeout(() => {
-                    button.innerHTML = originalButtonText;
-                    button.firstChild.src = "/static/assets/icons/copy-button.svg";
+                    button.textContent = "⛔️";
                 }, 1000);
             });
         }
         var websocket = null;
+        var timeout = null;
+        var timeoutDuration = 600000; // 10 minutes
+
         let region = null;
         let city = null;
         let countryName = null;
         let waitingForLocation = true;
 
         let websocketState = {
             newResponseText: null,
@@ -320,15 +322,15 @@
                 renderMessage(imageMarkdown, by, dt, references);
                 return;
             }
 
             renderMessage(message, by, dt, references);
         }
 
-        function formatHTMLMessage(htmlMessage, raw=false, willReplace=true) {
+        function formatHTMLMessage(htmlMessage, raw=false) {
             var md = window.markdownit();
             let newHTML = htmlMessage;
 
             // Remove any text between <s>[INST] and </s> tags. These are spurious instructions for the AI chat model.
             newHTML = newHTML.replace(/<s>\[INST\].+(<\/s>)?/g, '');
 
             // Customize the rendering of images
@@ -345,50 +347,34 @@
             // Render markdown
             newHTML = raw ? newHTML : md.render(newHTML);
             // Set rendered markdown to HTML DOM element
             let element = document.createElement('div');
             element.innerHTML = newHTML;
             element.className = "chat-message-text-response";
 
-            // Add a copy button to each chat message, if it doesn't already exist
-            if (willReplace === true) {
-                let copyButton = document.createElement('button');
-                copyButton.classList.add("copy-button");
-                copyButton.title = "Copy Message";
-                let copyIcon = document.createElement("img");
-                copyIcon.src = "/static/assets/icons/copy-button.svg";
-                copyIcon.classList.add("copy-icon");
-                copyButton.appendChild(copyIcon);
-                copyButton.addEventListener('click', copyParentText);
-                element.append(copyButton);
-            }
-
             // Get any elements with a class that starts with "language"
             let codeBlockElements = element.querySelectorAll('[class^="language-"]');
             // For each element, add a parent div with the class "programmatic-output"
             codeBlockElements.forEach((codeElement) => {
                 // Create the parent div
                 let parentDiv = document.createElement('div');
                 parentDiv.classList.add("programmatic-output");
                 // Add the parent div before the code element
                 codeElement.parentNode.insertBefore(parentDiv, codeElement);
                 // Move the code element into the parent div
                 parentDiv.appendChild(codeElement);
-                // Add a copy button to each code block, if it doesn't already exist
-                if (willReplace === true) {
-                    let copyButton = document.createElement('button');
-                    copyButton.classList.add("copy-button");
-                    copyButton.title = "Copy Code";
-                    let copyIcon = document.createElement("img");
-                    copyIcon.src = "/static/assets/icons/copy-button.svg";
-                    copyIcon.classList.add("copy-icon");
-                    copyButton.appendChild(copyIcon);
-                    copyButton.addEventListener('click', copyParentText);
-                    codeElement.prepend(copyButton);
-                }
+                // Add a copy button to each element
+                let copyButton = document.createElement('button');
+                copyButton.classList.add("copy-button");
+                let copyIcon = document.createElement("img");
+                copyIcon.src = "/static/assets/icons/copy_button.svg";
+                copyIcon.classList.add("copy-icon");
+                copyButton.appendChild(copyIcon);
+                copyButton.addEventListener('click', copyProgrammaticOutput);
+                codeElement.prepend(copyButton);
             });
 
             // Get all code elements that have no class.
             let codeElements = element.querySelectorAll('code:not([class])');
             codeElements.forEach((codeElement) => {
                 // Add the class "chat-response" to each element
                 codeElement.classList.add("chat-response");
@@ -586,15 +572,15 @@
         function handleStreamResponse(newResponseElement, rawResponse, loadingEllipsis, replace=true) {
             if (newResponseElement.getElementsByClassName("lds-ellipsis").length > 0 && loadingEllipsis) {
                 newResponseElement.removeChild(loadingEllipsis);
             }
             if (replace) {
                 newResponseElement.innerHTML = "";
             }
-            newResponseElement.appendChild(formatHTMLMessage(rawResponse, false, replace));
+            newResponseElement.appendChild(formatHTMLMessage(rawResponse));
             document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
         }
 
         function handleCompiledReferences(rawResponseElement, chunk, references, rawResponse) {
             const additionalResponse = chunk.split("### compiled references:")[0];
             rawResponse += additionalResponse;
             rawResponseElement.innerHTML = "";
@@ -884,20 +870,33 @@
                 newResponseText: null,
                 newResponseElement: null,
                 loadingEllipsis: null,
                 references: {},
                 rawResponse: "",
             }
 
+            function resetTimeout() {
+                if (timeout) {
+                    clearTimeout(timeout);
+                }
+
+                timeout = setTimeout(function() {
+                    if (websocket) {
+                        websocket.close();
+                    }
+                }, timeoutDuration);
+            }
+
             if (chatBody.dataset.conversationId) {
                 webSocketUrl += `?conversation_id=${chatBody.dataset.conversationId}`;
                 webSocketUrl += (!!region && !!city && !!countryName) ? `&region=${region}&city=${city}&country=${countryName}` : '';
 
                 websocket = new WebSocket(webSocketUrl);
                 websocket.onmessage = function(event) {
+                    resetTimeout();
 
                     // Get the last element in the chat-body
                     let chunk = event.data;
                     if (chunk == "start_llm_response") {
                         console.log("Started streaming", new Date());
                     } else if(chunk == "end_llm_response") {
                         console.log("Stopped streaming", new Date());
@@ -929,24 +928,22 @@
                             try {
                                 if (chunk.image || chunk.detail) {
                                     ({rawResponse, references } = handleImageResponse(chunk, websocketState.rawResponse));
                                     websocketState.rawResponse = rawResponse;
                                     websocketState.references = references;
                                 } else if (chunk.type == "status") {
                                     handleStreamResponse(websocketState.newResponseText, chunk.message, null, false);
-                                } else if (chunk.type == "rate_limit") {
-                                    handleStreamResponse(websocketState.newResponseText, chunk.message, websocketState.loadingEllipsis, true);
                                 } else {
                                     rawResponse = chunk.response;
                                 }
                             } catch (error) {
                                 // If the chunk is not a JSON object, just display it as is
                                 websocketState.rawResponse += chunk;
                             } finally {
-                                if (chunk.type != "status" && chunk.type != "rate_limit") {
+                                if (chunk.type != "status") {
                                     addMessageToChatBody(websocketState.rawResponse, websocketState.newResponseText, websocketState.references);
                                 }
                             }
                         } else {
 
                             // Handle streamed response of type text/event-stream or text/plain
                             if (chunk && chunk.includes("### compiled references:")) {
@@ -983,14 +980,17 @@
             websocket.onopen = function(event) {
                 console.log("WebSocket is open now.")
                 let statusDotIcon = document.getElementById("connection-status-icon");
                 statusDotIcon.style.backgroundColor = "green";
                 let statusDotText = document.getElementById("connection-status-text");
                 statusDotText.style.marginTop = "10px";
                 statusDotText.textContent = "Connected to Server";
+
+                // Setup the timeout to close the connection after inactivity.
+                resetTimeout();
             }
         }
 
         function sendMessageViaWebSocket(event) {
             if (event) {
                 event.preventDefault();
             }
@@ -1111,14 +1111,15 @@
                         let agentMetadataElement = document.getElementById("agent-metadata");
                         agentMetadataElement.style.display = "block";
                     } else {
                         let agentMetadataElement = document.getElementById("agent-metadata");
                         agentMetadataElement.style.display = "none";
                     }
 
+                    let chatBodyWrapper = document.getElementById("chat-body-wrapper");
                     const fullChatLog = response.chat || [];
 
                     fullChatLog.forEach(chat_log => {
                         if (chat_log.message != null){
                             renderMessageWithReference(
                                 chat_log.message,
                                 chat_log.by,
@@ -1128,15 +1129,14 @@
                                 chat_log.intent?.type,
                                 chat_log.intent?.["inferred-queries"]);
                         }
                         loadingScreen.style.height = chatBody.scrollHeight + 'px';
                     });
 
                     // Add fade out animation to loading screen and remove it after the animation ends
-                    let chatBodyWrapper = document.getElementById("chat-body-wrapper");
                     chatBodyWrapperHeight = chatBodyWrapper.clientHeight;
                     chatBody.style.height = chatBodyWrapperHeight;
                     setTimeout(() => {
                         loadingScreen.remove();
                         chatBody.classList.remove("relative-position");
                         setupDropZone();
                     }, 500);
@@ -2177,15 +2177,15 @@
 
         img.copy-icon {
             width: 16px;
             height: 16px;
         }
 
         button.copy-button:hover {
-            background-color: var(--primary-hover);
+            background-color: black;
             color: #f5f5f5;
         }
 
         pre {
             text-wrap: unset;
         }
 
@@ -2424,45 +2424,26 @@
 
         .loading-spinner {
             display: inline-block;
             position: relative;
             width: 80px;
             height: 80px;
         }
+
         .loading-spinner div {
             position: absolute;
             border: 4px solid var(--primary-hover);
             opacity: 1;
             border-radius: 50%;
             animation: lds-ripple 0.5s cubic-bezier(0, 0.2, 0.8, 1) infinite;
         }
+
         .loading-spinner div:nth-child(2) {
             animation-delay: -0.5s;
         }
-        @keyframes lds-ripple {
-            0% {
-                top: 36px;
-                left: 36px;
-                width: 0;
-                height: 0;
-                opacity: 1;
-                border-color: var(--primary-hover);
-            }
-            50% {
-                border-color: var(--flower);
-            }
-            100% {
-                top: 0px;
-                left: 0px;
-                width: 72px;
-                height: 72px;
-                opacity: 0;
-                border-color: var(--water);
-            }
-        }
 
         #agent-metadata-content {
             display: grid;
             grid-template-columns: auto 1fr;
             padding: 10px;
             background-color: var(--primary);
             border-radius: 5px;
@@ -2620,14 +2601,36 @@
         .modal-body select {
             padding: 8px;
             border-radius: 12px;
             border: 1px solid var(--main-text-color);
         }
 
 
+        @keyframes lds-ripple {
+            0% {
+                top: 36px;
+                left: 36px;
+                width: 0;
+                height: 0;
+                opacity: 1;
+                border-color: var(--primary-hover);
+            }
+            50% {
+                border-color: var(--flower);
+            }
+            100% {
+                top: 0px;
+                left: 0px;
+                width: 72px;
+                height: 72px;
+                opacity: 0;
+                border-color: var(--water);
+            }
+        }
+
         .lds-ellipsis {
             display: inline-block;
             position: relative;
             width: 60px;
             height: 32px;
         }
         .lds-ellipsis div {
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/config.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_computer_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_computer_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_github_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/content_source_notion_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/content_source_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/khoj.webmanifest` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/khoj.webmanifest`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/login.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/login.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/search.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/search.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/utils.html` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/utils.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 {% macro heading_pane(user_photo, username, is_active, has_documents) -%}
     <div class="khoj-header">
         <a class="khoj-logo" href="/">
             <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways-500.png?v={{ khoj_version }}" alt="Khoj"></img>
         </a>
         <nav class="khoj-nav">
-            <a id="chat-nav" class="khoj-nav" href="/chat">
-                <img class="nav-icon" src="/static/assets/icons/chat.svg" alt="Chat">
-                <span class="khoj-nav-item-text">Chat</span></a>
-            <a id="agents-nav" class="khoj-nav" href="/agents">
-                <img id="agents-icon" class="nav-icon" src="/static/assets/icons/agents.svg" alt="Agents">
-                <span class="khoj-nav-item-text">Agents</span></a>
+            <a id="agents-nav" class="khoj-nav" href="/agents">Agents</a>
             {% if has_documents %}
-            <a id="search-nav" class="khoj-nav" href="/search">
-                <img class="nav-icon" src="/static/assets/icons/search.svg" alt="Search">
-                <span class="khoj-nav-item-text">Search</span></a>
+            <a id="search-nav" class="khoj-nav" href="/search">Search</a>
             {% endif %}
             <!-- Dropdown Menu -->
             {% if username %}
                 <div id="khoj-nav-menu-container" class="khoj-nav dropdown">
                     {% if user_photo and user_photo != "None" %}
                         {% if is_active %}
                         <img id="profile-picture" class="circle subscribed" src="{{ user_photo }}" alt="{{ username[0].upper() }}" onclick="toggleMenu()" referrerpolicy="no-referrer">
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/khoj.css`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,14 @@
 .khoj-header {
     display: grid;
     grid-auto-flow: column;
     gap: 20px;
     padding: 16px 0;
     margin: 0;
 }
-.khoj-header {
-    align-items: center;
-}
 .khoj-footer {
     margin: 16px 0 0 0;
 }
 
 nav.khoj-nav {
     display: grid;
     grid-auto-flow: column;
@@ -111,26 +108,14 @@
 }
 .khoj-nav a:hover {
     background-color: var(--primary-hover);
 }
 .khoj-nav-selected {
     background-color: var(--primary);
 }
-.nav-icon {
-    width: 24px;
-    height: 24px;
-}
-#agents-icon {
-    width: 30px;
-    height: 30px;
-}
-span.khoj-nav-item-text {
-    padding-top: 6px;
-    padding-left: 8px;
-}
 img.khoj-logo {
     width: min(60vw, 90px);
     max-width: 100%;
     justify-self: center;
 }
 
 /* Dropdown in navigation menu*/
@@ -188,16 +173,15 @@
     color: black;
     display: grid;
     justify-content: center;
     align-items: center;
     font-size: 20px;
     box-sizing: unset;
     width: 40px;
-    height: 35px;
-    padding-top: 8px
+    height: 40px;
 }
 .subscribed {
     border: 3px solid var(--primary-hover);
 }
 
 @media screen and (max-width: 700px) {
     .khoj-nav-dropdown-content {
@@ -224,14 +208,8 @@
         margin: 0;
     }
 
     nav.khoj-nav {
         grid-gap: 0px;
         justify-content: space-between;
     }
-    a.khoj-nav {
-        padding: 0 16px;
-    }
-    span.khoj-nav-item-text {
-        display: none;
-    }
 }
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/utils.js` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/utils.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/computer.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/computer.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/credit-card.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/credit-card.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon-256x256.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/key.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/key.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/microphone-solid.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/microphone-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/openai-logomark.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/openai-logomark.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/plaintext.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/plaintext.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/stop-solid.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/stop-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/user-silhouette.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/user-silhouette.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/web.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/web.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/icons/whatsapp.svg` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png` & `khoj_assistant-1.9.1.dev8/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_default_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_default_model_2.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_default_model_2.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_chat_schema.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_chat_schema.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_offline_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_offline_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_processor_config_openai.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_processor_config_openai.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_server_pg.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_server_pg.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/migrations/migrate_version.py` & `khoj_assistant-1.9.1.dev8/src/khoj/migrations/migrate_version.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/embeddings.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/embeddings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/content/text_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/text_to_entries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import hashlib
 import logging
-import re
 import uuid
 from abc import ABC, abstractmethod
 from itertools import repeat
 from typing import Any, Callable, List, Set, Tuple
 
-from langchain.text_splitter import RecursiveCharacterTextSplitter
 from tqdm import tqdm
 
 from khoj.database.adapters import EntryAdapters, get_user_search_model_or_default
 from khoj.database.models import Entry as DbEntry
 from khoj.database.models import EntryDates, KhojUser
 from khoj.search_filter.date_filter import DateFilter
 from khoj.utils import state
@@ -33,72 +31,45 @@
         ...
 
     @staticmethod
     def hash_func(key: str) -> Callable:
         return lambda entry: hashlib.md5(bytes(getattr(entry, key), encoding="utf-8")).hexdigest()
 
     @staticmethod
-    def remove_long_words(text: str, max_word_length: int = 500) -> str:
-        "Remove words longer than max_word_length from text."
-        # Split the string by words, keeping the delimiters
-        splits = re.split(r"(\s+)", text) + [""]
-        words_with_delimiters = list(zip(splits[::2], splits[1::2]))
-
-        # Filter out long words while preserving delimiters in text
-        filtered_text = [
-            f"{word}{delimiter}"
-            for word, delimiter in words_with_delimiters
-            if not word.strip() or len(word.strip()) <= max_word_length
-        ]
-
-        return "".join(filtered_text)
-
-    @staticmethod
-    def tokenizer(text: str) -> List[str]:
-        "Tokenize text into words."
-        return text.split()
-
-    @staticmethod
     def split_entries_by_max_tokens(
-        entries: List[Entry], max_tokens: int = 256, max_word_length: int = 500, raw_is_compiled: bool = False
+        entries: List[Entry], max_tokens: int = 256, max_word_length: int = 500
     ) -> List[Entry]:
         "Split entries if compiled entry length exceeds the max tokens supported by the ML model."
         chunked_entries: List[Entry] = []
         for entry in entries:
             if is_none_or_empty(entry.compiled):
                 continue
 
-            # Split entry into chunks of max_tokens
-            # Use chunking preference order: paragraphs > sentences > words > characters
-            text_splitter = RecursiveCharacterTextSplitter(
-                chunk_size=max_tokens,
-                separators=["\n\n", "\n", "!", "?", ".", " ", "\t", ""],
-                keep_separator=True,
-                length_function=lambda chunk: len(TextToEntries.tokenizer(chunk)),
-                chunk_overlap=0,
-            )
-            chunked_entry_chunks = text_splitter.split_text(entry.compiled)
+            # Split entry into words
+            compiled_entry_words = [word for word in entry.compiled.split(" ") if word != ""]
+
+            # Drop long words instead of having entry truncated to maintain quality of entry processed by models
+            compiled_entry_words = [word for word in compiled_entry_words if len(word) <= max_word_length]
             corpus_id = uuid.uuid4()
 
-            # Create heading prefixed entry from each chunk
-            for chunk_index, compiled_entry_chunk in enumerate(chunked_entry_chunks):
+            # Split entry into chunks of max tokens
+            for chunk_index in range(0, len(compiled_entry_words), max_tokens):
+                compiled_entry_words_chunk = compiled_entry_words[chunk_index : chunk_index + max_tokens]
+                compiled_entry_chunk = " ".join(compiled_entry_words_chunk)
+
                 # Prepend heading to all other chunks, the first chunk already has heading from original entry
-                if chunk_index > 0 and entry.heading:
+                if chunk_index > 0:
                     # Snip heading to avoid crossing max_tokens limit
                     # Keep last 100 characters of heading as entry heading more important than filename
                     snipped_heading = entry.heading[-100:]
-                    # Prepend snipped heading
-                    compiled_entry_chunk = f"{snipped_heading}\n{compiled_entry_chunk}"
-
-                # Drop long words instead of having entry truncated to maintain quality of entry processed by models
-                compiled_entry_chunk = TextToEntries.remove_long_words(compiled_entry_chunk, max_word_length)
+                    compiled_entry_chunk = f"{snipped_heading}.\n{compiled_entry_chunk}"
 
                 # Clean entry of unwanted characters like \0 character
                 compiled_entry_chunk = TextToEntries.clean_field(compiled_entry_chunk)
-                entry.raw = compiled_entry_chunk if raw_is_compiled else TextToEntries.clean_field(entry.raw)
+                entry.raw = TextToEntries.clean_field(entry.raw)
                 entry.heading = TextToEntries.clean_field(entry.heading)
                 entry.file = TextToEntries.clean_field(entry.file)
 
                 chunked_entries.append(
                     Entry(
                         compiled=compiled_entry_chunk,
                         raw=entry.raw,
@@ -185,15 +156,15 @@
                     )
                     logger.error(f"Error adding entries to database:\n{batch_indexing_error}\n---\n{e}", exc_info=True)
             logger.debug(f"Added {len(added_entries)} {file_type} entries to database")
 
         new_dates = []
         with timer("Indexed dates from added entries in", logger):
             for added_entry in added_entries:
-                dates_in_entries = zip(self.date_filter.extract_dates(added_entry.compiled), repeat(added_entry))
+                dates_in_entries = zip(self.date_filter.extract_dates(added_entry.raw), repeat(added_entry))
                 dates_to_create = [
                     EntryDates(date=date, entry=added_entry)
                     for date, added_entry in dates_in_entries
                     if not is_none_or_empty(date)
                 ]
                 new_dates += EntryDates.objects.bulk_create(dates_to_create)
             logger.debug(f"Indexed {len(new_dates)} dates from added {file_type} entries")
@@ -270,9 +241,14 @@
             existing_entries_sorted = sorted(existing_entries, key=lambda e: e[0])
 
             entries_with_ids = existing_entries_sorted + new_entries_sorted
 
         return entries_with_ids
 
     @staticmethod
+    def convert_text_maps_to_jsonl(entries: List[Entry]) -> str:
+        # Convert each entry to JSON and write to JSONL file
+        return "".join([f"{entry.to_json()}\n" for entry in entries])
+
+    @staticmethod
     def clean_field(field: str) -> str:
         return field.replace("\0", "") if not is_none_or_empty(field) else ""
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/content/markdown/markdown_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/markdown/markdown_to_entries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import re
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import List, Tuple
 
 import urllib3
 
 from khoj.database.models import Entry as DbEntry
 from khoj.database.models import KhojUser
 from khoj.processor.content.text_to_entries import TextToEntries
+from khoj.utils.constants import empty_escape_sequences
 from khoj.utils.helpers import timer
 from khoj.utils.rawconfig import Entry
 
 logger = logging.getLogger(__name__)
 
 
 class MarkdownToEntries(TextToEntries):
@@ -26,22 +27,23 @@
         if not full_corpus:
             deletion_file_names = set([file for file in files if files[file] == ""])
             files_to_process = set(files) - deletion_file_names
             files = {file: files[file] for file in files_to_process}
         else:
             deletion_file_names = None
 
-        max_tokens = 256
         # Extract Entries from specified Markdown files
-        with timer("Extract entries from specified Markdown files", logger):
-            current_entries = MarkdownToEntries.extract_markdown_entries(files, max_tokens)
+        with timer("Parse entries from Markdown files into dictionaries", logger):
+            current_entries = MarkdownToEntries.convert_markdown_entries_to_maps(
+                *MarkdownToEntries.extract_markdown_entries(files)
+            )
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
-            current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens)
+            current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
             num_new_embeddings, num_deleted_embeddings = self.update_embeddings(
                 current_entries,
                 DbEntry.EntryType.MARKDOWN,
                 DbEntry.EntrySource.COMPUTER,
@@ -51,112 +53,82 @@
                 user,
                 regenerate=regenerate,
             )
 
         return num_new_embeddings, num_deleted_embeddings
 
     @staticmethod
-    def extract_markdown_entries(markdown_files, max_tokens=256) -> List[Entry]:
+    def extract_markdown_entries(markdown_files):
         "Extract entries by heading from specified Markdown files"
-        entries: List[str] = []
-        entry_to_file_map: List[Tuple[str, str]] = []
+
+        # Regex to extract Markdown Entries by Heading
+
+        entries = []
+        entry_to_file_map = []
         for markdown_file in markdown_files:
             try:
                 markdown_content = markdown_files[markdown_file]
                 entries, entry_to_file_map = MarkdownToEntries.process_single_markdown_file(
-                    markdown_content, markdown_file, entries, entry_to_file_map, max_tokens
+                    markdown_content, markdown_file, entries, entry_to_file_map
                 )
             except Exception as e:
-                logger.error(
-                    f"Unable to process file: {markdown_file}. This file will not be indexed.\n{e}", exc_info=True
-                )
+                logger.warning(f"Unable to process file: {markdown_file}. This file will not be indexed.")
+                logger.warning(e, exc_info=True)
 
-        return MarkdownToEntries.convert_markdown_entries_to_maps(entries, dict(entry_to_file_map))
+        return entries, dict(entry_to_file_map)
 
     @staticmethod
     def process_single_markdown_file(
-        markdown_content: str,
-        markdown_file: str,
-        entries: List[str],
-        entry_to_file_map: List[Tuple[str, str]],
-        max_tokens=256,
-        ancestry: Dict[int, str] = {},
-    ) -> Tuple[List[str], List[Tuple[str, str]]]:
-        # Prepend the markdown section's heading ancestry
-        ancestry_string = "\n".join([f"{'#' * key} {ancestry[key]}" for key in sorted(ancestry.keys())])
-        markdown_content_with_ancestry = f"{ancestry_string}{markdown_content}"
-
-        # If content is small or content has no children headings, save it as a single entry
-        if len(TextToEntries.tokenizer(markdown_content_with_ancestry)) <= max_tokens or not re.search(
-            rf"^#{{{len(ancestry)+1},}}\s", markdown_content, flags=re.MULTILINE
-        ):
-            entry_to_file_map += [(markdown_content_with_ancestry, markdown_file)]
-            entries.extend([markdown_content_with_ancestry])
-            return entries, entry_to_file_map
-
-        # Split by next heading level present in the entry
-        next_heading_level = len(ancestry)
-        sections: List[str] = []
-        while len(sections) < 2:
-            next_heading_level += 1
-            sections = re.split(rf"(\n|^)(?=[#]{{{next_heading_level}}} .+\n?)", markdown_content, flags=re.MULTILINE)
-
-        for section in sections:
-            # Skip empty sections
-            if section.strip() == "":
-                continue
-
-            # Extract the section body and (when present) the heading
-            current_ancestry = ancestry.copy()
-            first_line = [line for line in section.split("\n") if line.strip() != ""][0]
-            if re.search(rf"^#{{{next_heading_level}}} ", first_line):
-                # Extract the section body without the heading
-                current_section_body = "\n".join(section.split(first_line)[1:])
-                # Parse the section heading into current section ancestry
-                current_section_title = first_line[next_heading_level:].strip()
-                current_ancestry[next_heading_level] = current_section_title
-            else:
-                current_section_body = section
-
-            # Recurse down children of the current entry
-            MarkdownToEntries.process_single_markdown_file(
-                current_section_body,
-                markdown_file,
-                entries,
-                entry_to_file_map,
-                max_tokens,
-                current_ancestry,
-            )
+        markdown_content: str, markdown_file: Path, entries: List, entry_to_file_map: List
+    ):
+        markdown_heading_regex = r"^#"
+
+        markdown_entries_per_file = []
+        any_headings = re.search(markdown_heading_regex, markdown_content, flags=re.MULTILINE)
+        for entry in re.split(markdown_heading_regex, markdown_content, flags=re.MULTILINE):
+            # Add heading level as the regex split removed it from entries with headings
+            prefix = "#" if entry.startswith("#") else "# " if any_headings else ""
+            stripped_entry = entry.strip(empty_escape_sequences)
+            if stripped_entry != "":
+                markdown_entries_per_file.append(f"{prefix}{stripped_entry}")
 
+        entry_to_file_map += zip(markdown_entries_per_file, [markdown_file] * len(markdown_entries_per_file))
+        entries.extend(markdown_entries_per_file)
         return entries, entry_to_file_map
 
     @staticmethod
     def convert_markdown_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
         "Convert each Markdown entries into a dictionary"
-        entries: List[Entry] = []
+        entries = []
         for parsed_entry in parsed_entries:
             raw_filename = entry_to_file_map[parsed_entry]
 
             # Check if raw_filename is a URL. If so, save it as is. If not, convert it to a Path.
             if type(raw_filename) == str and re.search(r"^https?://", raw_filename):
                 # Escape the URL to avoid issues with special characters
                 entry_filename = urllib3.util.parse_url(raw_filename).url
             else:
                 entry_filename = str(Path(raw_filename))
+            stem = Path(raw_filename).stem
 
             heading = parsed_entry.splitlines()[0] if re.search("^#+\s", parsed_entry) else ""
             # Append base filename to compiled entry for context to model
             # Increment heading level for heading entries and make filename as its top level heading
-            prefix = f"# {entry_filename}\n#" if heading else f"# {entry_filename}\n"
-            compiled_entry = f"{prefix}{parsed_entry}"
+            prefix = f"# {stem}\n#" if heading else f"# {stem}\n"
+            compiled_entry = f"{entry_filename}\n{prefix}{parsed_entry}"
             entries.append(
                 Entry(
                     compiled=compiled_entry,
                     raw=parsed_entry,
                     heading=f"{prefix}{heading}",
                     file=f"{entry_filename}",
                 )
             )
 
         logger.debug(f"Converted {len(parsed_entries)} markdown entries to dictionaries")
 
         return entries
+
+    @staticmethod
+    def convert_markdown_maps_to_jsonl(entries: List[Entry]):
+        "Convert each Markdown entry to JSON and collate as JSONL"
+        return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/content/notion/notion_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/notion/notion_to_entries.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,16 +219,15 @@
     def get_page_content(self, page_id):
         try:
             page = self.get_page(page_id)
             content = self.get_page_children(page_id)
         except Exception as e:
             logger.error(f"Error getting page {page_id}: {e}", exc_info=True)
             return None, None
-        properties = page.get("properties", {})
-
+        properties = page["properties"]
         title_field = "title"
         if "Title" in properties:
             title_field = "Title"
         elif "Name" in properties:
             title_field = "Name"
         elif "Page" in properties:
             title_field = "Page"
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/content/org_mode/orgnode.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/org_mode/orgnode.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 constructing data structures of these classes.
 """
 
 import datetime
 import re
 from os.path import relpath
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import List
 
 indent_regex = re.compile(r"^ *")
 
 
 def normalize_filename(filename):
     "Normalize and escape filename for rendering"
     if not Path(filename).is_absolute():
@@ -54,15 +54,15 @@
 
 
 def makelist_with_filepath(filename):
     f = open(filename, "r")
     return makelist(f, filename)
 
 
-def makelist(file, filename) -> List["Orgnode"]:
+def makelist(file, filename):
     """
     Read an org-mode file and return a list of Orgnode objects
     created from this file.
     """
     ctr = 0
 
     if type(file) == str:
@@ -76,51 +76,51 @@
         "ACTIVE": "",
         "DONE": "",
         "CANCELLED": "",
         "FAILED": "",
     }  # populated from #+SEQ_TODO line
     level = ""
     heading = ""
-    ancestor_headings: List[str] = []
+    ancestor_headings = []
     bodytext = ""
     introtext = ""
-    tags: List[str] = list()  # set of all tags in headline
-    closed_date: datetime.date = None
-    sched_date: datetime.date = None
-    deadline_date: datetime.date = None
-    logbook: List[Tuple[datetime.datetime, datetime.datetime]] = list()
+    tags = list()  # set of all tags in headline
+    closed_date = ""
+    sched_date = ""
+    deadline_date = ""
+    logbook = list()
     nodelist: List[Orgnode] = list()
-    property_map: Dict[str, str] = dict()
+    property_map = dict()
     in_properties_drawer = False
     in_logbook_drawer = False
     file_title = f"{filename}"
 
     for line in f:
         ctr += 1
         heading_search = re.search(r"^(\*+)\s(.*?)\s*$", line)
         if heading_search:  # we are processing a heading line
             if heading:  # if we have are on second heading, append first heading to headings list
                 thisNode = Orgnode(level, heading, bodytext, tags, ancestor_headings)
                 if closed_date:
                     thisNode.closed = closed_date
-                    closed_date = None
+                    closed_date = ""
                 if sched_date:
                     thisNode.scheduled = sched_date
-                    sched_date = None
+                    sched_date = ""
                 if deadline_date:
                     thisNode.deadline = deadline_date
-                    deadline_date = None
+                    deadline_date = ""
                 if logbook:
                     thisNode.logbook = logbook
                     logbook = list()
                 thisNode.properties = property_map
                 nodelist.append(thisNode)
             property_map = {"LINE": f"file:{normalize_filename(filename)}::{ctr}"}
             previous_level = level
-            previous_heading: str = heading
+            previous_heading = heading
             level = heading_search.group(1)
             heading = heading_search.group(2)
             bodytext = ""
             tags = list()  # set of all tags in headline
             tag_search = re.search(r"(.*?)\s*:([a-zA-Z0-9].*?):$", heading)
             if tag_search:
                 heading = tag_search.group(1)
@@ -491,21 +491,20 @@
             n = n + "*"
         n = n + " "
         if self._todo:
             n = n + self._todo + " "
         if self._priority:
             n = n + "[#" + self._priority + "] "
         n = n + self._heading
-        if self._tags:
-            n = "%-60s " % n  # hack - tags will start in column 62
-            closecolon = ""
-            for t in self._tags:
-                n = n + ":" + t
-                closecolon = ":"
-            n = n + closecolon
+        n = "%-60s " % n  # hack - tags will start in column 62
+        closecolon = ""
+        for t in self._tags:
+            n = n + ":" + t
+            closecolon = ":"
+        n = n + closecolon
         n = n + "\n"
 
         # Get body indentation from first line of body
         indent = indent_regex.match(self._body).group()
 
         # Output Closed Date, Scheduled Date, Deadline Date
         if self._closed or self._scheduled or self._deadline:
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/content/pdf/pdf_to_entries.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/content/pdf/pdf_to_entries.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             deletion_file_names = set([file for file in files if files[file] == b""])
             files_to_process = set(files) - deletion_file_names
             files = {file: files[file] for file in files_to_process}
         else:
             deletion_file_names = None
 
         # Extract Entries from specified Pdf files
-        with timer("Extract entries from specified PDF files", logger):
-            current_entries = PdfToEntries.extract_pdf_entries(files)
+        with timer("Parse entries from PDF files into dictionaries", logger):
+            current_entries = PdfToEntries.convert_pdf_entries_to_maps(*PdfToEntries.extract_pdf_entries(files))
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
@@ -51,19 +51,19 @@
                 user,
                 regenerate=regenerate,
             )
 
         return num_new_embeddings, num_deleted_embeddings
 
     @staticmethod
-    def extract_pdf_entries(pdf_files) -> List[Entry]:
+    def extract_pdf_entries(pdf_files):
         """Extract entries by page from specified PDF files"""
 
-        entries: List[str] = []
-        entry_to_location_map: List[Tuple[str, str]] = []
+        entries = []
+        entry_to_location_map = []
         for pdf_file in pdf_files:
             try:
                 # Write the PDF file to a temporary file, as it is stored in byte format in the pdf_file object and the PDF Loader expects a file path
                 timestamp_now = datetime.utcnow().timestamp()
                 tmp_file = f"tmp_pdf_file_{timestamp_now}.pdf"
                 with open(f"{tmp_file}", "wb") as f:
                     bytes = pdf_files[pdf_file]
@@ -79,15 +79,15 @@
             except Exception as e:
                 logger.warning(f"Unable to process file: {pdf_file}. This file will not be indexed.")
                 logger.warning(e, exc_info=True)
             finally:
                 if os.path.exists(f"{tmp_file}"):
                     os.remove(f"{tmp_file}")
 
-        return PdfToEntries.convert_pdf_entries_to_maps(entries, dict(entry_to_location_map))
+        return entries, dict(entry_to_location_map)
 
     @staticmethod
     def convert_pdf_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
         "Convert each PDF entries into a dictionary"
         entries = []
         for parsed_entry in parsed_entries:
             entry_filename = entry_to_file_map[parsed_entry]
@@ -102,7 +102,12 @@
                     file=f"{entry_filename}",
                 )
             )
 
         logger.debug(f"Converted {len(parsed_entries)} PDF entries to dictionaries")
 
         return entries
+
+    @staticmethod
+    def convert_pdf_maps_to_jsonl(entries: List[Entry]):
+        "Convert each PDF entry to JSON and collate as JSONL"
+        return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 Q: {query}
 """.strip()
 )
 
 
 extract_questions = PromptTemplate.from_template(
     """
-You are Khoj, an extremely smart and helpful document search assistant with only the ability to retrieve information from the user's notes. Disregard online search requests. Construct search queries to retrieve relevant information to answer the user's question.
+You are Khoj, an extremely smart and helpful search assistant with the ability to retrieve information from the user's notes. Construct search queries to retrieve relevant information to answer the user's question.
 - You will be provided past questions(Q) and answers(A) for context.
 - Add as much context from the previous questions and answers as required into your search queries.
 - Break messages into multiple search queries when required to retrieve the relevant information.
 - Add date filters to your search queries from questions and answers when required to retrieve the relevant information.
 
 What searches will you perform to answer the users question? Respond with search queries as list of strings in a JSON object.
 Current Date: {day_of_week}, {current_date}
@@ -507,16 +507,18 @@
 """.strip()
 )
 
 # Personalization to the user
 # --
 user_location = PromptTemplate.from_template(
     """
+Mention the user's location only if it's relevant to the conversation.
 User's Location: {location}
 """.strip()
 )
 
 user_name = PromptTemplate.from_template(
     """
+Mention the user's name only if it's relevant to the conversation.
 User's Name: {name}
 """.strip()
 )
```

#### html2text {}

```diff
@@ -105,105 +105,105 @@
 plants? Khoj: ["What kind of plants do I have?", "What issues do my plants
 have?"] Q: Who all did I meet here yesterday? Khoj: ["Met in {location} on
 {yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"] Chat History:
 {chat_history} What searches will you perform to answer the following question,
 using the chat history as reference? Respond with relevant search queries as
 list of strings. Q: {query} """.strip() ) extract_questions =
 PromptTemplate.from_template( """ You are Khoj, an extremely smart and helpful
-document search assistant with only the ability to retrieve information from
-the user's notes. Disregard online search requests. Construct search queries to
-retrieve relevant information to answer the user's question. - You will be
-provided past questions(Q) and answers(A) for context. - Add as much context
-from the previous questions and answers as required into your search queries. -
-Break messages into multiple search queries when required to retrieve the
-relevant information. - Add date filters to your search queries from questions
-and answers when required to retrieve the relevant information. What searches
-will you perform to answer the users question? Respond with search queries as
-list of strings in a JSON object. Current Date: {day_of_week}, {current_date}
-User's Location: {location} Q: How was my trip to Cambodia? Khoj: {{"queries":
-["How was my trip to Cambodia?"]}} A: The trip was amazing. You went to the
-Angkor Wat temple and it was beautiful. Q: Who did i visit that temple with?
-Khoj: {{"queries": ["Who did I visit the Angkor Wat Temple in Cambodia
-with?"]}} A: You visited the Angkor Wat Temple in Cambodia with Pablo, Namita
-and Xi. Q: What national parks did I go to last year? Khoj: {{"queries":
-["National park I visited in {last_new_year} dt>='{last_new_year_date}' dt<'
-{current_new_year_date}'"]}} A: You visited the Grand Canyon and Yellowstone
-National Park in {last_new_year}. Q: How can you help me? Khoj: {{"queries":
-["Social relationships", "Physical and mental health", "Education and career",
-"Personal life goals and habits"]}} A: I can help you live healthier and
-happier across work and personal life Q: How many tennis balls fit in the back
-of a 2002 Honda Civic? Khoj: {{"queries": ["What is the size of a tennis
-ball?", "What is the trunk size of a 2002 Honda Civic?"]}} A: 1085 tennis balls
-will fit in the trunk of a Honda Civic Q: Is Bob older than Tom? Khoj: {
-{"queries": ["When was Bob born?", "What is Tom's age?"]}} A: Yes, Bob is older
-than Tom. As Bob was born on 1984-01-01 and Tom is 30 years old. Q: What is
-their age difference? Khoj: {{"queries": ["What is Bob's age?", "What is Tom's
-age?"]}} A: Bob is {bob_tom_age_difference} years older than Tom. As Bob is
-{bob_age} years old and Tom is 30 years old. Q: Who all did I meet here
-yesterday? Khoj: {{"queries": ["Met in {location} on {yesterday_date} dt>='
-{yesterday_date}' dt<'{current_date}'"]}} A: Yesterday's note mentions your
-visit to your local beach with Ram and Shyam. {chat_history} Q: {text} Khoj:
-""".strip() ) system_prompt_extract_relevant_information = """As a professional
-analyst, create a comprehensive report of the most relevant information from a
-web page in response to a user's query. The text provided is directly from
-within the web page. The report you create should be multiple paragraphs, and
-it should represent the content of the website. Tell the user exactly what the
-website says in response to their query, while adhering to these guidelines: 1.
-Answer the user's query as specifically as possible. Include many supporting
-details from the website. 2. Craft a report that is detailed, thorough, in-
-depth, and complex, while maintaining clarity. 3. Rely strictly on the provided
-text, without including external information. 4. Format the report in multiple
-paragraphs with a clear structure. 5. Be as specific as possible in your answer
-to the user's query. 6. Reproduce as much of the provided text as possible,
-while maintaining readability. """.strip() extract_relevant_information =
-PromptTemplate.from_template( """ Target Query: {query} Web Pages: {corpus}
-Collate only relevant information from the website to answer the target query.
-""".strip() ) pick_relevant_output_mode = PromptTemplate.from_template( """ You
-are Khoj, an excellent analyst for selecting the correct way to respond to a
-user's query. You have access to a limited set of modes for your response. You
-can only use one of these modes. {modes} Here are some example responses:
-Example: Chat History: User: I just visited Jerusalem for the first time. Pull
-up my notes from the trip. AI: You mention visiting Masjid Al-Aqsa and the
-Western Wall. You also mention trying the local cuisine and visiting the Dead
-Sea. Q: Draw a picture of my trip to Jerusalem. Khoj: image Example: Chat
-History: User: I'm having trouble deciding which laptop to get. I want
-something with at least 16 GB of RAM and a 1 TB SSD. AI: I can help with that.
-I see online that there is a new model of the Dell XPS 15 that meets your
-requirements. Q: What are the specs of the new Dell XPS 15? Khoj: default Now
-it's your turn to pick the mode you would like to use to answer the user's
-question. Provide your response as a string. Chat History: {chat_history} Q:
-{query} Khoj: """.strip() ) pick_relevant_information_collection_tools =
-PromptTemplate.from_template( """ You are Khoj, an extremely smart and helpful
-search assistant. - You have access to a variety of data sources to help you
-answer the user's question - You can use the data sources listed below to
-collect more relevant information - You can use any combination of these data
-sources to answer the user's question Which of the data sources listed below
-you would use to answer the user's question? {tools} Here are some example
-responses: Example: Chat History: User: I'm thinking of moving to a new city.
-I'm trying to decide between New York and San Francisco. AI: Moving to a new
-city can be challenging. Both New York and San Francisco are great cities to
-live in. New York is known for its diverse culture and San Francisco is known
-for its tech scene. Q: What is the population of each of those cities? Khoj: {
-{"source": ["online"]}} Example: Chat History: User: I'm thinking of my next
-vacation idea. Ideally, I want to see something new and exciting. AI:
-Excellent! Taking a vacation is a great way to relax and recharge. Q: Where did
-Grandma grow up? Khoj: {{"source": ["notes"]}} Example: Chat History: Q: What
-can you do for me? Khoj: {{"source": ["notes", "online"]}} Example: Chat
-History: User: Good morning AI: Good morning! How can I help you today? Q: How
-can I share my files with Khoj? Khoj: {{"source": ["default", "online"]}}
-Example: Chat History: User: What is the first element in the periodic table?
-AI: The first element in the periodic table is Hydrogen. Q: Summarize this
-article https://en.wikipedia.org/wiki/Hydrogen Khoj: {{"source": ["webpage"]}}
-Example: Chat History: User: I want to start a new hobby. I'm thinking of
-learning to play the guitar. AI: Learning to play the guitar is a great hobby.
-It can be a lot of fun and a great way to express yourself. Q: What is the
-first element of the periodic table? Khoj: {{"source": ["general"]}} Now it's
-your turn to pick the data sources you would like to use to answer the user's
-question. Respond with data sources as a list of strings in a JSON object. Chat
-History: {chat_history} Q: {query} Khoj: """.strip() ) infer_webpages_to_read =
+search assistant with the ability to retrieve information from the user's
+notes. Construct search queries to retrieve relevant information to answer the
+user's question. - You will be provided past questions(Q) and answers(A) for
+context. - Add as much context from the previous questions and answers as
+required into your search queries. - Break messages into multiple search
+queries when required to retrieve the relevant information. - Add date filters
+to your search queries from questions and answers when required to retrieve the
+relevant information. What searches will you perform to answer the users
+question? Respond with search queries as list of strings in a JSON object.
+Current Date: {day_of_week}, {current_date} User's Location: {location} Q: How
+was my trip to Cambodia? Khoj: {{"queries": ["How was my trip to Cambodia?"]}}
+A: The trip was amazing. You went to the Angkor Wat temple and it was
+beautiful. Q: Who did i visit that temple with? Khoj: {{"queries": ["Who did I
+visit the Angkor Wat Temple in Cambodia with?"]}} A: You visited the Angkor Wat
+Temple in Cambodia with Pablo, Namita and Xi. Q: What national parks did I go
+to last year? Khoj: {{"queries": ["National park I visited in {last_new_year}
+dt>='{last_new_year_date}' dt<'{current_new_year_date}'"]}} A: You visited the
+Grand Canyon and Yellowstone National Park in {last_new_year}. Q: How can you
+help me? Khoj: {{"queries": ["Social relationships", "Physical and mental
+health", "Education and career", "Personal life goals and habits"]}} A: I can
+help you live healthier and happier across work and personal life Q: How many
+tennis balls fit in the back of a 2002 Honda Civic? Khoj: {{"queries": ["What
+is the size of a tennis ball?", "What is the trunk size of a 2002 Honda
+Civic?"]}} A: 1085 tennis balls will fit in the trunk of a Honda Civic Q: Is
+Bob older than Tom? Khoj: {{"queries": ["When was Bob born?", "What is Tom's
+age?"]}} A: Yes, Bob is older than Tom. As Bob was born on 1984-01-01 and Tom
+is 30 years old. Q: What is their age difference? Khoj: {{"queries": ["What is
+Bob's age?", "What is Tom's age?"]}} A: Bob is {bob_tom_age_difference} years
+older than Tom. As Bob is {bob_age} years old and Tom is 30 years old. Q: Who
+all did I meet here yesterday? Khoj: {{"queries": ["Met in {location} on
+{yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"]}} A: Yesterday's
+note mentions your visit to your local beach with Ram and Shyam. {chat_history}
+Q: {text} Khoj: """.strip() ) system_prompt_extract_relevant_information =
+"""As a professional analyst, create a comprehensive report of the most
+relevant information from a web page in response to a user's query. The text
+provided is directly from within the web page. The report you create should be
+multiple paragraphs, and it should represent the content of the website. Tell
+the user exactly what the website says in response to their query, while
+adhering to these guidelines: 1. Answer the user's query as specifically as
+possible. Include many supporting details from the website. 2. Craft a report
+that is detailed, thorough, in-depth, and complex, while maintaining clarity.
+3. Rely strictly on the provided text, without including external information.
+4. Format the report in multiple paragraphs with a clear structure. 5. Be as
+specific as possible in your answer to the user's query. 6. Reproduce as much
+of the provided text as possible, while maintaining readability. """.strip()
+extract_relevant_information = PromptTemplate.from_template( """ Target Query:
+{query} Web Pages: {corpus} Collate only relevant information from the website
+to answer the target query. """.strip() ) pick_relevant_output_mode =
+PromptTemplate.from_template( """ You are Khoj, an excellent analyst for
+selecting the correct way to respond to a user's query. You have access to a
+limited set of modes for your response. You can only use one of these modes.
+{modes} Here are some example responses: Example: Chat History: User: I just
+visited Jerusalem for the first time. Pull up my notes from the trip. AI: You
+mention visiting Masjid Al-Aqsa and the Western Wall. You also mention trying
+the local cuisine and visiting the Dead Sea. Q: Draw a picture of my trip to
+Jerusalem. Khoj: image Example: Chat History: User: I'm having trouble deciding
+which laptop to get. I want something with at least 16 GB of RAM and a 1 TB
+SSD. AI: I can help with that. I see online that there is a new model of the
+Dell XPS 15 that meets your requirements. Q: What are the specs of the new Dell
+XPS 15? Khoj: default Now it's your turn to pick the mode you would like to use
+to answer the user's question. Provide your response as a string. Chat History:
+{chat_history} Q: {query} Khoj: """.strip() )
+pick_relevant_information_collection_tools = PromptTemplate.from_template( """
+You are Khoj, an extremely smart and helpful search assistant. - You have
+access to a variety of data sources to help you answer the user's question -
+You can use the data sources listed below to collect more relevant information
+- You can use any combination of these data sources to answer the user's
+question Which of the data sources listed below you would use to answer the
+user's question? {tools} Here are some example responses: Example: Chat
+History: User: I'm thinking of moving to a new city. I'm trying to decide
+between New York and San Francisco. AI: Moving to a new city can be
+challenging. Both New York and San Francisco are great cities to live in. New
+York is known for its diverse culture and San Francisco is known for its tech
+scene. Q: What is the population of each of those cities? Khoj: {{"source":
+["online"]}} Example: Chat History: User: I'm thinking of my next vacation
+idea. Ideally, I want to see something new and exciting. AI: Excellent! Taking
+a vacation is a great way to relax and recharge. Q: Where did Grandma grow up?
+Khoj: {{"source": ["notes"]}} Example: Chat History: Q: What can you do for me?
+Khoj: {{"source": ["notes", "online"]}} Example: Chat History: User: Good
+morning AI: Good morning! How can I help you today? Q: How can I share my files
+with Khoj? Khoj: {{"source": ["default", "online"]}} Example: Chat History:
+User: What is the first element in the periodic table? AI: The first element in
+the periodic table is Hydrogen. Q: Summarize this article https://
+en.wikipedia.org/wiki/Hydrogen Khoj: {{"source": ["webpage"]}} Example: Chat
+History: User: I want to start a new hobby. I'm thinking of learning to play
+the guitar. AI: Learning to play the guitar is a great hobby. It can be a lot
+of fun and a great way to express yourself. Q: What is the first element of the
+periodic table? Khoj: {{"source": ["general"]}} Now it's your turn to pick the
+data sources you would like to use to answer the user's question. Respond with
+data sources as a list of strings in a JSON object. Chat History:
+{chat_history} Q: {query} Khoj: """.strip() ) infer_webpages_to_read =
 PromptTemplate.from_template( """ You are Khoj, an advanced web page reading
 assistant. You are to construct **up to three, valid** webpage urls to read
 before answering the user's question. - You will receive the conversation
 history as context. - Add as much context from the previous questions and
 answers as required to construct the webpage urls. - Use multiple web page urls
 if required to retrieve the relevant information. - You have access to the the
 whole internet to retrieve information. Which webpages will you need to read to
@@ -265,10 +265,12 @@
 notes**: Chat using the information in your knowledge base. - **/general**:
 Chat using just Khoj's general knowledge. This will not search against your
 notes. - **/default**: Chat using your knowledge base and Khoj's general
 knowledge for context. - **/online**: Chat using the internet as a source of
 information. - **/image**: Generate an image based on your message. - **/
 help**: Show this help message. You are using the **{model}** model on the **
 {device}**. **version**: {version} """.strip() ) # Personalization to the user
-# -- user_location = PromptTemplate.from_template( """ User's Location:
-{location} """.strip() ) user_name = PromptTemplate.from_template( """ User's
-Name: {name} """.strip() )
+# -- user_location = PromptTemplate.from_template( """ Mention the user's
+location only if it's relevant to the conversation. User's Location: {location}
+""".strip() ) user_name = PromptTemplate.from_template( """ Mention the user's
+name only if it's relevant to the conversation. User's Name: {name} """.strip()
+)
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/chat_model.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/chat_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,19 +151,19 @@
         system_prompt = prompts.system_prompt_offline_chat.format(current_date=current_date)
 
     conversation_primer = prompts.query_prompt.format(query=user_query)
 
     if location_data:
         location = f"{location_data.city}, {location_data.region}, {location_data.country}"
         location_prompt = prompts.user_location.format(location=location)
-        system_prompt = f"{system_prompt}\n{location_prompt}"
+        conversation_primer = f"{location_prompt}\n{conversation_primer}"
 
     if user_name:
         user_name_prompt = prompts.user_name.format(name=user_name)
-        system_prompt = f"{system_prompt}\n{user_name_prompt}"
+        conversation_primer = f"{user_name_prompt}\n{conversation_primer}"
 
     # Get Conversation Primer appropriate to Conversation Type
     if conversation_commands == [ConversationCommand.Notes] and is_none_or_empty(compiled_references_message):
         return iter([prompts.no_notes_found.format()])
     elif conversation_commands == [ConversationCommand.Online] and is_none_or_empty(online_results):
         completion_func(chat_response=prompts.no_online_results_found.format())
         return iter([prompts.no_online_results_found.format()])
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/offline/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/offline/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/gpt.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     # Get Response from GPT
     response = completion_with_backoff(
         messages=messages,
         model_name=model,
         temperature=temperature,
         max_tokens=max_tokens,
-        model_kwargs={"response_format": {"type": "json_object"}},
+        model_kwargs={"stop": ["A: ", "\n"], "response_format": {"type": "json_object"}},
         openai_api_key=api_key,
     )
 
     # Extract, Clean Message from GPT's Response
     try:
         response = response.strip()
         response = json.loads(response)
@@ -133,19 +133,19 @@
         )
     else:
         system_prompt = prompts.personality.format(current_date=current_date)
 
     if location_data:
         location = f"{location_data.city}, {location_data.region}, {location_data.country}"
         location_prompt = prompts.user_location.format(location=location)
-        system_prompt = f"{system_prompt}\n{location_prompt}"
+        conversation_primer = f"{location_prompt}\n{conversation_primer}"
 
     if user_name:
         user_name_prompt = prompts.user_name.format(name=user_name)
-        system_prompt = f"{system_prompt}\n{user_name_prompt}"
+        conversation_primer = f"{user_name_prompt}\n{conversation_primer}"
 
     # Get Conversation Primer appropriate to Conversation Type
     if conversation_commands == [ConversationCommand.Notes] and is_none_or_empty(compiled_references):
         completion_func(chat_response=prompts.no_notes_found.format())
         return iter([prompts.no_notes_found.format()])
     elif conversation_commands == [ConversationCommand.Online] and is_none_or_empty(online_results):
         completion_func(chat_response=prompts.no_online_results_found.format())
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/conversation/openai/utils.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/conversation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/processor/tools/online_search.py` & `khoj_assistant-1.9.1.dev8/src/khoj/processor/tools/online_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 import logging
 import os
 from collections import defaultdict
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Dict, Tuple, Union
 
 import aiohttp
 import requests
 from bs4 import BeautifulSoup
 from markdownify import markdownify
 
 from khoj.routers.helpers import (
@@ -38,45 +38,37 @@
     # to retrieve the dataset (from the dataset API) if you only need the markdown or html.
     "expandMarkdown": "True",
     "expandHtml": "False",
 }
 MAX_WEBPAGES_TO_READ = 1
 
 
-async def search_online(
-    query: str, conversation_history: dict, location: LocationData, send_status_func: Optional[Callable] = None
-):
+async def search_online(query: str, conversation_history: dict, location: LocationData):
     if not online_search_enabled():
         logger.warn("SERPER_DEV_API_KEY is not set")
         return {}
 
     # Breakdown the query into subqueries to get the correct answer
     subqueries = await generate_online_subqueries(query, conversation_history, location)
     response_dict = {}
 
     for subquery in subqueries:
-        if send_status_func:
-            await send_status_func(f"**🌐 Searching the Internet for**: {subquery}")
-        logger.info(f"🌐 Searching the Internet for '{subquery}'")
+        logger.info(f"Searching with Google for '{subquery}'")
         response_dict[subquery] = search_with_google(subquery)
 
     # Gather distinct web pages from organic search results of each subquery without an instant answer
     webpage_links = {
         organic["link"]: subquery
         for subquery in response_dict
         for organic in response_dict[subquery].get("organic", [])[:MAX_WEBPAGES_TO_READ]
         if "answerBox" not in response_dict[subquery]
     }
 
     # Read, extract relevant info from the retrieved web pages
-    if webpage_links:
-        logger.info(f"🌐👀 Reading web pages at: {list(webpage_links)}")
-        if send_status_func:
-            webpage_links_str = "\n- " + "\n- ".join(list(webpage_links))
-            await send_status_func(f"**📖 Reading web pages**: {webpage_links_str}")
+    logger.info(f"Reading web pages at: {webpage_links.keys()}")
     tasks = [read_webpage_and_extract_content(subquery, link) for link, subquery in webpage_links.items()]
     results = await asyncio.gather(*tasks)
 
     # Collect extracted info from the retrieved web pages
     for subquery, webpage_extract, url in results:
         if webpage_extract is not None:
             response_dict[subquery]["webpages"] = {"link": url, "snippet": webpage_extract}
@@ -99,27 +91,20 @@
     extracted_search_result = {
         field: json_response[field] for field in extraction_fields if not is_none_or_empty(json_response.get(field))
     }
 
     return extracted_search_result
 
 
-async def read_webpages(
-    query: str, conversation_history: dict, location: LocationData, send_status_func: Optional[Callable] = None
-):
+async def read_webpages(query: str, conversation_history: dict, location: LocationData):
     "Infer web pages to read from the query and extract relevant information from them"
     logger.info(f"Inferring web pages to read")
-    if send_status_func:
-        await send_status_func(f"**🧐 Inferring web pages to read**")
     urls = await infer_webpage_urls(query, conversation_history, location)
 
     logger.info(f"Reading web pages at: {urls}")
-    if send_status_func:
-        webpage_links_str = "\n- " + "\n- ".join(list(urls))
-        await send_status_func(f"**📖 Reading web pages**: {webpage_links_str}")
     tasks = [read_webpage_and_extract_content(query, url) for url in urls]
     results = await asyncio.gather(*tasks)
 
     response: Dict[str, Dict] = defaultdict(dict)
     response[query]["webpages"] = [
         {"query": q, "link": url, "snippet": web_extract} for q, web_extract, url in results if web_extract is not None
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/api.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import concurrent.futures
 import json
 import logging
 import math
 import os
 import time
 import uuid
-from typing import Any, Callable, List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from asgiref.sync import sync_to_async
 from fastapi import APIRouter, Depends, File, HTTPException, Request, UploadFile
 from fastapi.requests import Request
 from fastapi.responses import Response
-from starlette.authentication import has_required_scope, requires
+from starlette.authentication import requires
 
 from khoj.configure import initialize_content
 from khoj.database.adapters import (
     ConversationAdapters,
     EntryAdapters,
-    get_user_photo,
     get_user_search_model_or_default,
 )
 from khoj.database.models import ChatModelOptions, KhojUser, SpeechToTextModelOptions
 from khoj.processor.conversation.offline.chat_model import extract_questions_offline
 from khoj.processor.conversation.offline.whisper import transcribe_audio_offline
 from khoj.processor.conversation.openai.gpt import extract_questions
 from khoj.processor.conversation.openai.whisper import transcribe_audio
@@ -178,15 +177,15 @@
 ):
     user = request.user.object
     if not state.config:
         error_msg = f"🚨 Khoj is not configured.\nConfigure it via http://localhost:42110/config, plugins or by editing {state.config_file}."
         logger.warning(error_msg)
         raise HTTPException(status_code=500, detail=error_msg)
     try:
-        initialize_content(regenerate=force, search_type=t, user=user)
+        initialize_content(regenerate=force, search_type=t, init=False, user=user)
     except Exception as e:
         error_msg = f"🚨 Failed to update server via API: {e}"
         logger.error(error_msg, exc_info=True)
         raise HTTPException(status_code=500, detail=error_msg)
     else:
         components = []
         if state.search_models:
@@ -270,15 +269,14 @@
     common: CommonQueryParams,
     meta_log: dict,
     q: str,
     n: int,
     d: float,
     conversation_commands: List[ConversationCommand] = [ConversationCommand.Default],
     location_data: LocationData = None,
-    send_status_func: Optional[Callable] = None,
 ):
     user = request.user.object if request.user.is_authenticated else None
 
     # Initialize Variables
     compiled_references: List[Any] = []
     inferred_queries: List[str] = []
 
@@ -342,17 +340,14 @@
                 location_data=location_data,
             )
 
     # Collate search results as context for GPT
     with timer("Searching knowledge base took", logger):
         result_list = []
         logger.info(f"🔍 Searching knowledge base with queries: {inferred_queries}")
-        if send_status_func:
-            inferred_queries_str = "\n- " + "\n- ".join(inferred_queries)
-            await send_status_func(f"**🔍 Searching Documents for:** {inferred_queries_str}")
         for query in inferred_queries:
             n_items = min(n, 3) if using_offline_chat else n
             result_list.extend(
                 await execute_search(
                     user,
                     f"{query} {filters_in_query}",
                     n=n_items,
@@ -369,29 +364,7 @@
 
 
 @api.get("/health", response_class=Response)
 @requires(["authenticated"], status_code=200)
 def health_check(request: Request) -> Response:
     response_obj = {"email": request.user.object.email}
     return Response(content=json.dumps(response_obj), media_type="application/json", status_code=200)
-
-
-@api.get("/v1/user", response_class=Response)
-@requires(["authenticated"])
-def user_info(request: Request) -> Response:
-    # Get user information
-    user: KhojUser = request.user.object
-    user_picture = get_user_photo(user=user)
-    is_active = has_required_scope(request, ["premium"])
-    has_documents = EntryAdapters.user_has_entries(user=user)
-
-    # Collect user information in a dictionary
-    user_info = {
-        "email": user.email,
-        "username": user.username,
-        "photo": user_picture,
-        "is_active": is_active,
-        "has_documents": has_documents,
-    }
-
-    # Return user information as a JSON response
-    return Response(content=json.dumps(user_info), media_type="application/json", status_code=200)
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/api_agents.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_agents.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/api_chat.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import math
 from typing import Dict, Optional
 from urllib.parse import unquote
 
 from asgiref.sync import sync_to_async
-from fastapi import APIRouter, Depends, HTTPException, Request, WebSocket
+from fastapi import APIRouter, Depends, Request, WebSocket
 from fastapi.requests import Request
 from fastapi.responses import Response, StreamingResponse
 from starlette.authentication import requires
 from starlette.websockets import WebSocketDisconnect
 from websockets import ConnectionClosedOK
 
 from khoj.database.adapters import ConversationAdapters, EntryAdapters, aget_user_name
@@ -288,30 +288,14 @@
             return
         try:
             await websocket.send_text(message)
         except ConnectionClosedOK:
             connection_alive = False
             logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
 
-    async def send_rate_limit_message(message: str):
-        nonlocal connection_alive
-        if not connection_alive:
-            return
-
-        status_packet = {
-            "type": "rate_limit",
-            "message": message,
-            "content-type": "application/json",
-        }
-        try:
-            await websocket.send_text(json.dumps(status_packet))
-        except ConnectionClosedOK:
-            connection_alive = False
-            logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
-
     user: KhojUser = websocket.user.object
     conversation = await ConversationAdapters.aget_conversation_by_user(
         user, client_application=websocket.user.client_app, conversation_id=conversation_id
     )
 
     hourly_limiter = ApiUserRateLimiter(requests=5, subscribed_requests=60, window=60, slug="chat_minute")
 
@@ -330,59 +314,53 @@
     while connection_alive:
         try:
             q = await websocket.receive_text()
         except WebSocketDisconnect:
             logger.debug(f"User {user} disconnected web socket")
             break
 
-        try:
-            await sync_to_async(hourly_limiter)(websocket)
-            await sync_to_async(daily_limiter)(websocket)
-        except HTTPException as e:
-            await send_rate_limit_message(e.detail)
-            break
+        await sync_to_async(hourly_limiter)(websocket)
+        await sync_to_async(daily_limiter)(websocket)
 
         conversation_commands = [get_conversation_command(query=q, any_references=True)]
 
-        await send_status_update(f"**👀 Understanding Query**: {q}")
+        await send_status_update(f"**Processing query**: {q}")
 
         if conversation_commands == [ConversationCommand.Help]:
             conversation_config = await ConversationAdapters.aget_user_conversation_config(user)
             if conversation_config == None:
                 conversation_config = await ConversationAdapters.aget_default_conversation_config()
             model_type = conversation_config.model_type
             formatted_help = help_message.format(model=model_type, version=state.khoj_version, device=get_device())
             await send_complete_llm_response(formatted_help)
             continue
 
         meta_log = conversation.conversation_log
 
         if conversation_commands == [ConversationCommand.Default]:
             conversation_commands = await aget_relevant_information_sources(q, meta_log)
-            conversation_commands_str = ", ".join([cmd.value for cmd in conversation_commands])
-            await send_status_update(f"**🗃️ Chose Data Sources to Search:** {conversation_commands_str}")
-
             mode = await aget_relevant_output_modes(q, meta_log)
-            await send_status_update(f"**🧑🏾‍💻 Decided Response Mode:** {mode.value}")
             if mode not in conversation_commands:
                 conversation_commands.append(mode)
 
         for cmd in conversation_commands:
             await conversation_command_rate_limiter.update_and_check_if_valid(websocket, cmd)
             q = q.replace(f"/{cmd.value}", "").strip()
 
+        await send_status_update(
+            f"**Using conversation commands:** {', '.join([cmd.value for cmd in conversation_commands])}"
+        )
+
         compiled_references, inferred_queries, defiltered_query = await extract_references_and_questions(
-            websocket, None, meta_log, q, 7, 0.18, conversation_commands, location, send_status_update
+            websocket, None, meta_log, q, 7, 0.18, conversation_commands, location
         )
 
         if compiled_references:
-            headings = "\n- " + "\n- ".join(
-                set([" ".join(c.split("Path: ")[1:]).split("\n ")[0] for c in compiled_references])
-            )
-            await send_status_update(f"**📜 Found Relevant Notes**: {headings}")
+            headings = set([c.split("\n")[0] for c in compiled_references])
+            await send_status_update(f"**Searching references**: {headings}")
 
         online_results: Dict = dict()
 
         if conversation_commands == [ConversationCommand.Notes] and not await EntryAdapters.auser_has_entries(user):
             await send_complete_llm_response(f"{no_entries_found.format()}")
             continue
 
@@ -393,51 +371,50 @@
             if not online_search_enabled():
                 conversation_commands.remove(ConversationCommand.Online)
                 # If online search is not enabled, try to read webpages directly
                 if ConversationCommand.Webpage not in conversation_commands:
                     conversation_commands.append(ConversationCommand.Webpage)
             else:
                 try:
-                    online_results = await search_online(defiltered_query, meta_log, location, send_status_update)
+                    await send_status_update("**Operation**: Searching the web for relevant information...")
+                    online_results = await search_online(defiltered_query, meta_log, location)
+                    online_searches = ", ".join([f"{query}" for query in online_results.keys()])
+                    await send_status_update(f"**Online searches**: {online_searches}")
                 except ValueError as e:
                     logger.warning(f"Error searching online: {e}. Attempting to respond without online results")
                     await send_complete_llm_response(
                         f"Error searching online: {e}. Attempting to respond without online results"
                     )
                     continue
 
         if ConversationCommand.Webpage in conversation_commands:
             try:
-                online_results = await read_webpages(defiltered_query, meta_log, location, send_status_update)
+                await send_status_update("**Operation**: Directly searching web pages...")
+                online_results = await read_webpages(defiltered_query, meta_log, location)
                 webpages = []
                 for query in online_results:
                     for webpage in online_results[query]["webpages"]:
                         webpages.append(webpage["link"])
-                await send_status_update(f"**📚 Read web pages**: {webpages}")
+                await send_status_update(f"**Web pages read**: {webpages}")
             except ValueError as e:
                 logger.warning(
                     f"Error directly reading webpages: {e}. Attempting to respond without online results", exc_info=True
                 )
 
         if ConversationCommand.Image in conversation_commands:
             update_telemetry_state(
                 request=websocket,
                 telemetry_type="api",
                 api="chat",
                 metadata={"conversation_command": conversation_commands[0].value},
             )
+            await send_status_update("**Operation**: Augmenting your query and generating a superb image...")
             intent_type = "text-to-image"
             image, status_code, improved_image_prompt, image_url = await text_to_image(
-                q,
-                user,
-                meta_log,
-                location_data=location,
-                references=compiled_references,
-                online_results=online_results,
-                send_status_func=send_status_update,
+                q, user, meta_log, location_data=location, references=compiled_references, online_results=online_results
             )
             if image is None or status_code != 200:
                 content_obj = {
                     "image": image,
                     "intentType": intent_type,
                     "detail": improved_image_prompt,
                     "content-type": "application/json",
@@ -461,15 +438,14 @@
                 online_results=online_results,
             )
             content_obj = {"image": image, "intentType": intent_type, "inferredQueries": [improved_image_prompt], "context": compiled_references, "content-type": "application/json", "online_results": online_results}  # type: ignore
 
             await send_complete_llm_response(json.dumps(content_obj))
             continue
 
-        await send_status_update(f"**💭 Generating a well-informed response**")
         llm_response, chat_metadata = await agenerate_chat_response(
             defiltered_query,
             meta_log,
             conversation,
             compiled_references,
             online_results,
             inferred_queries,
@@ -509,15 +485,15 @@
 @api_chat.get("", response_class=Response)
 @requires(["authenticated"])
 async def chat(
     request: Request,
     common: CommonQueryParams,
     q: str,
     n: Optional[int] = 5,
-    d: Optional[float] = 0.22,
+    d: Optional[float] = 0.18,
     stream: Optional[bool] = False,
     title: Optional[str] = None,
     conversation_id: Optional[int] = None,
     city: Optional[str] = None,
     region: Optional[str] = None,
     country: Optional[str] = None,
     rate_limiter_per_minute=Depends(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/api_config.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     update_telemetry_state(
         request=request,
         telemetry_type="api",
         api="get_all_filenames",
         client=client,
     )
 
-    return await sync_to_async(list)(EntryAdapters.get_all_filenames_by_source(user, content_source))  # type: ignore[call-arg]
+    return await sync_to_async(list)(EntryAdapters.aget_all_filenames_by_source(user, content_source))  # type: ignore[call-arg]
 
 
 @api_config.post("/data/conversation/model", status_code=200)
 @requires(["authenticated"])
 async def update_chat_model(
     request: Request,
     id: str,
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/api_phone.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/api_phone.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/auth.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import asyncio
-import datetime
 import logging
 import os
 from typing import Optional
 
 from fastapi import APIRouter
 from starlette.authentication import requires
 from starlette.config import Config
@@ -13,15 +11,14 @@
 
 from khoj.database.adapters import (
     create_khoj_token,
     delete_khoj_token,
     get_khoj_tokens,
     get_or_create_user,
 )
-from khoj.routers.email import send_welcome_email
 from khoj.routers.helpers import update_telemetry_state
 from khoj.utils import state
 
 logger = logging.getLogger(__name__)
 
 auth_router = APIRouter()
 
@@ -95,41 +92,37 @@
 async def auth(request: Request):
     form = await request.form()
     next_url = request.query_params.get("next", "/")
     credential = form.get("credential")
 
     csrf_token_cookie = request.cookies.get("g_csrf_token")
     if not csrf_token_cookie:
-        logger.info("Missing CSRF token. Redirecting user to login page")
-        return RedirectResponse(url=f"{next_url}")
+        return Response("Missing CSRF token", status_code=400)
     csrf_token_body = form.get("g_csrf_token")
     if not csrf_token_body:
-        logger.info("Missing CSRF token body. Redirecting user to login page")
-        return RedirectResponse(url=f"{next_url}")
+        return Response("Missing CSRF token", status_code=400)
     if csrf_token_cookie != csrf_token_body:
         return Response("Invalid CSRF token", status_code=400)
 
     try:
         idinfo = id_token.verify_oauth2_token(credential, google_requests.Request(), os.environ["GOOGLE_CLIENT_ID"])
     except OAuthError as error:
         return HTMLResponse(f"<h1>{error.error}</h1>")
     khoj_user = await get_or_create_user(idinfo)
-
     if khoj_user:
         request.session["user"] = dict(idinfo)
 
-        if datetime.timedelta(minutes=3) > (datetime.datetime.now(datetime.timezone.utc) - khoj_user.date_joined):
-            asyncio.create_task(send_welcome_email(idinfo["name"], idinfo["email"]))
+        if not khoj_user.last_login:
             update_telemetry_state(
                 request=request,
                 telemetry_type="api",
                 api="create_user",
                 metadata={"user_id": str(khoj_user.uuid)},
             )
-            logger.log(logging.INFO, f"🥳 New User Created: {khoj_user.uuid}")
+            logger.log(logging.INFO, f"New User Created: {khoj_user.uuid}")
             return RedirectResponse(url=f"{next_url}", status_code=HTTP_302_FOUND)
 
     return RedirectResponse(url=f"{next_url}")
 
 
 @auth_router.get("/logout")
 async def logout(request: Request):
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/helpers.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 import asyncio
 import json
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta, timezone
 from functools import partial
-from typing import (
-    Annotated,
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import Annotated, Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import openai
 from fastapi import Depends, Header, HTTPException, Request, UploadFile
 from starlette.authentication import has_required_scope
 
 from khoj.database.adapters import AgentAdapters, ConversationAdapters, EntryAdapters
 from khoj.database.models import (
@@ -503,15 +493,14 @@
 async def text_to_image(
     message: str,
     user: KhojUser,
     conversation_log: dict,
     location_data: LocationData,
     references: List[str],
     online_results: Dict[str, Any],
-    send_status_func: Optional[Callable] = None,
 ) -> Tuple[Optional[str], int, Optional[str], Optional[str]]:
     status_code = 200
     image = None
     response = None
     image_url = None
 
     text_to_image_config = await ConversationAdapters.aget_text_to_image_model_config()
@@ -529,26 +518,22 @@
                 chat_history += f"Q: {chat['intent']['query']}\n"
                 chat_history += f"A: {chat['message']}\n"
             elif chat["by"] == "khoj" and "text-to-image" in chat["intent"].get("type"):
                 chat_history += f"Q: Query: {chat['intent']['query']}\n"
                 chat_history += f"A: Improved Query: {chat['intent']['inferred-queries'][0]}\n"
         try:
             with timer("Improve the original user query", logger):
-                if send_status_func:
-                    await send_status_func("**✍🏽 Enhancing the Painting Prompt**")
                 improved_image_prompt = await generate_better_image_prompt(
                     message,
                     chat_history,
                     location_data=location_data,
                     note_references=references,
                     online_results=online_results,
                 )
             with timer("Generate image with OpenAI", logger):
-                if send_status_func:
-                    await send_status_func(f"**🖼️ Painting using Enhanced Prompt**:\n{improved_image_prompt}")
                 response = state.openai_client.images.generate(
                     prompt=improved_image_prompt, model=text2image_model, response_format="b64_json"
                 )
                 image = response.data[0].b64_json
 
             with timer("Upload image to S3", logger):
                 image_url = upload_image(image, user.uuid)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/indexer.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,19 @@
     ),
 ):
     user = request.user.object
     index_files: Dict[str, Dict[str, str]] = {"org": {}, "markdown": {}, "pdf": {}, "plaintext": {}}
     try:
         logger.info(f"📬 Updating content index via API call by {client} client")
         for file in files:
-            file_content = file.file.read()
-            file_type, encoding = get_file_type(file.content_type, file_content)
+            file_type, encoding = get_file_type(file.content_type)
             if file_type in index_files:
-                index_files[file_type][file.filename] = file_content.decode(encoding) if encoding else file_content
+                index_files[file_type][file.filename] = (
+                    file.file.read().decode("utf-8") if encoding == "utf-8" else file.file.read()  # type: ignore
+                )
             else:
                 logger.warning(f"Skipped indexing unsupported file type sent by {client} client: {file.filename}")
 
         indexer_input = IndexerInput(
             org=index_files["org"],
             markdown=index_files["markdown"],
             pdf=index_files["pdf"],
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/notion.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/notion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/storage.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/storage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/subscription.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/twilio.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/twilio.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/routers/web_client.py` & `khoj_assistant-1.9.1.dev8/src/khoj/routers/web_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     )
 
 
 @web_client.get("/agents", response_class=HTMLResponse)
 def agents_page(request: Request):
     user: KhojUser = request.user.object if request.user.is_authenticated else None
     user_picture = request.session.get("user", {}).get("picture") if user else None
-    has_documents = EntryAdapters.user_has_entries(user=user)
     agents = AgentAdapters.get_all_accessible_agents(user)
     agents_packet = list()
     for agent in agents:
         agents_packet.append(
             {
                 "slug": agent.slug,
                 "avatar": agent.avatar,
@@ -153,28 +152,27 @@
     return templates.TemplateResponse(
         "agents.html",
         context={
             "request": request,
             "agents": agents_packet,
             "khoj_version": state.khoj_version,
             "username": user.username if user else None,
-            "has_documents": has_documents,
+            "has_documents": False,
             "is_active": has_required_scope(request, ["premium"]),
             "user_photo": user_picture,
         },
     )
 
 
 @web_client.get("/agent/{agent_slug}", response_class=HTMLResponse)
 def agent_page(request: Request, agent_slug: str):
     user: KhojUser = request.user.object if request.user.is_authenticated else None
     user_picture = request.session.get("user", {}).get("picture") if user else None
 
     agent = AgentAdapters.get_agent_by_slug(agent_slug)
-    has_documents = EntryAdapters.user_has_entries(user=user)
 
     if agent == None:
         return templates.TemplateResponse(
             "404.html",
             context={
                 "request": request,
                 "khoj_version": state.khoj_version,
@@ -200,15 +198,15 @@
     return templates.TemplateResponse(
         "agent.html",
         context={
             "request": request,
             "agent": agent_metadata,
             "khoj_version": state.khoj_version,
             "username": user.username if user else None,
-            "has_documents": has_documents,
+            "has_documents": False,
             "is_active": has_required_scope(request, ["premium"]),
             "user_photo": user_picture,
         },
     )
 
 
 @web_client.get("/config", response_class=HTMLResponse)
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/search_filter/date_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/search_filter/file_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/search_filter/word_filter.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/search_type/text_search.py` & `khoj_assistant-1.9.1.dev8/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/cli.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/config.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/constants.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/fs_syncer.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/fs_syncer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import glob
 import logging
 import os
-from pathlib import Path
 from typing import Optional
 
 from bs4 import BeautifulSoup
-from magika import Magika
 
 from khoj.database.models import (
     LocalMarkdownConfig,
     LocalOrgConfig,
     LocalPdfConfig,
     LocalPlaintextConfig,
 )
 from khoj.utils.config import SearchType
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty
 from khoj.utils.rawconfig import TextContentConfig
 
 logger = logging.getLogger(__name__)
-magika = Magika()
 
 
 def collect_files(search_type: Optional[SearchType] = SearchType.All, user=None) -> dict:
     files = {}
 
     if search_type == SearchType.All or search_type == SearchType.Org:
         org_config = LocalOrgConfig.objects.filter(user=user).first()
@@ -46,19 +43,14 @@
         index_heading_entries=db_config.index_heading_entries,
     )
 
 
 def get_plaintext_files(config: TextContentConfig) -> dict[str, str]:
     def is_plaintextfile(file: str):
         "Check if file is plaintext file"
-        # Check if file path exists
-        mime_type = magika.identify_path(Path(file)).output.mime_type
-        if mime_type != "inode/x-empty" and mime_type != "application/unknown":
-            return mime_type.startswith("text/")
-        # Use file extension to decide plaintext if file content is not identifiable
         return file.endswith(("txt", "md", "markdown", "org", "mbox", "rst", "html", "htm", "xml"))
 
     def extract_html_content(html_content: str):
         "Extract content from HTML"
         soup = BeautifulSoup(html_content, "html.parser")
         return soup.get_text(strip=True, separator="\n")
 
@@ -69,15 +61,15 @@
     )
 
     # Input Validation
     if is_none_or_empty(input_files) and is_none_or_empty(input_filters):
         logger.debug("At least one of input-files or input-file-filter is required to be specified")
         return {}
 
-    # Get all plain text files to process
+    "Get all files to process"
     absolute_plaintext_files, filtered_plaintext_files = set(), set()
     if input_files:
         absolute_plaintext_files = {get_absolute_path(jsonl_file) for jsonl_file in input_files}
     if input_filters:
         filtered_plaintext_files = {
             filtered_file
             for plaintext_file_filter in input_filters
@@ -213,15 +205,15 @@
     )
 
     # Input Validation
     if is_none_or_empty(pdf_files) and is_none_or_empty(pdf_file_filters):
         logger.debug("At least one of pdf-files or pdf-file-filter is required to be specified")
         return {}
 
-    # Get PDF files to process
+    "Get PDF files to process"
     absolute_pdf_files, filtered_pdf_files = set(), set()
     if pdf_files:
         absolute_pdf_files = {get_absolute_path(pdf_file) for pdf_file in pdf_files}
     if pdf_file_filters:
         filtered_pdf_files = {
             filtered_file
             for pdf_file_filter in pdf_file_filters
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/helpers.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,24 @@
 from pathlib import Path
 from time import perf_counter
 from typing import TYPE_CHECKING, Optional, Union
 from urllib.parse import urlparse
 
 import torch
 from asgiref.sync import sync_to_async
-from magika import Magika
 
 from khoj.utils import constants
 
 if TYPE_CHECKING:
     from sentence_transformers import CrossEncoder, SentenceTransformer
 
     from khoj.utils.models import BaseEncoder
     from khoj.utils.rawconfig import AppConfig
 
 
-# Initialize Magika for file type identification
-magika = Magika()
-
-
 class AsyncIteratorWrapper:
     def __init__(self, obj):
         self._it = iter(obj)
 
     def __aiter__(self):
         return self
 
@@ -89,39 +84,30 @@
         if key not in priority_dict:
             merged_dict[key] = default_dict[key]
         elif isinstance(priority_dict[key], dict) and isinstance(default_dict[key], dict):
             merged_dict[key] = merge_dicts(priority_dict[key], default_dict[key])
     return merged_dict
 
 
-def get_file_type(file_type: str, file_content: bytes) -> tuple[str, str]:
+def get_file_type(file_type: str) -> tuple[str, str]:
     "Get file type from file mime type"
 
-    # Extract encoding from file_type
     encoding = file_type.split("=")[1].strip().lower() if ";" in file_type else None
     file_type = file_type.split(";")[0].strip() if ";" in file_type else file_type
-
-    # Infer content type from reading file content
-    try:
-        content_type = magika.identify_bytes(file_content).output.mime_type
-    except Exception:
-        # Fallback to using just file type if content type cannot be inferred
-        content_type = file_type
-
-    if file_type in ["text/markdown"] and content_type.startswith("text/"):
+    if file_type in ["text/markdown"]:
         return "markdown", encoding
-    elif file_type in ["text/org"] and content_type.startswith("text/"):
+    elif file_type in ["text/org"]:
         return "org", encoding
-    elif file_type in ["application/pdf"] and content_type == "application/pdf":
+    elif file_type in ["application/pdf"]:
         return "pdf", encoding
-    elif file_type in ["image/jpeg"] and content_type == "image/jpeg":
+    elif file_type in ["image/jpeg"]:
         return "jpeg", encoding
-    elif file_type in ["image/png"] and content_type == "image/png":
+    elif file_type in ["image/png"]:
         return "png", encoding
-    elif content_type.startswith("text/"):
+    elif file_type in ["text/plain", "text/html", "application/xml", "text/x-rst"]:
         return "plaintext", encoding
     else:
         return "other", encoding
 
 
 def load_model(
     model_name: str, model_type, model_dir=None, device: str = None
```

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/initialization.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/initialization.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/jsonl.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/models.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/rawconfig.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/state.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/src/khoj/utils/yaml.py` & `khoj_assistant-1.9.1.dev8/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/.gitignore` & `khoj_assistant-1.9.1.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/LICENSE` & `khoj_assistant-1.9.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.9.1.dev74/README.md` & `khoj_assistant-1.9.1.dev8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,7 @@
 Cheers to our awesome contributors! 🎉
 
 <a href="https://github.com/khoj-ai/khoj/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=khoj-ai/khoj" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
-
-## [Sponsors](https://github.com/sponsors/khoj-ai)
-Shout out to our brilliant sponsors! 🌈
-
-<a href="http://github.com/beekeeb">
-  <img src="https://raw.githubusercontent.com/beekeeb/piantor/main/docs/beekeeb.png" width=250/>
-</a>
```

#### html2text {}

```diff
@@ -21,11 +21,8 @@
 images and understand your speech. - Khoj is open-source, self-hostable.
 Always. ***
 ## See it in action [Khoj Demo]Go to https://app.khoj.dev to see Khoj live. ##
 Full feature list You can see the full feature list [here](https://
 docs.khoj.dev/category/features). ## Self-Host To get started with self-hosting
 Khoj, [read the docs](https://docs.khoj.dev/get-started/setup). ## Contributors
 Cheers to our awesome contributors! ð _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_k_h_o_j_-_a_i_/_k_h_o_j_]Made with [contrib.rocks](https://contrib.rocks). ##
-[Sponsors](https://github.com/sponsors/khoj-ai) Shout out to our brilliant
-sponsors! ð_[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_b_e_e_k_e_e_b_/_p_i_a_n_t_o_r_/_m_a_i_n_/_d_o_c_s_/
-_b_e_e_k_e_e_b_._p_n_g_]
+_i_m_a_g_e_?_r_e_p_o_=_k_h_o_j_-_a_i_/_k_h_o_j_]Made with [contrib.rocks](https://contrib.rocks).
```

### Comparing `khoj_assistant-1.9.1.dev74/pyproject.toml` & `khoj_assistant-1.9.1.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     "defusedxml == 0.7.1",
     "fastapi >= 0.104.1",
     "python-multipart >= 0.0.7",
     "jinja2 == 3.1.3",
     "openai >= 1.0.0",
     "tiktoken >= 0.3.2",
     "tenacity >= 8.2.2",
-    "magika ~= 0.5.1",
     "pillow ~= 9.5.0",
     "pydantic >= 2.0.0",
     "pyyaml ~= 6.0",
     "rich >= 13.3.1",
     "schedule == 1.1.0",
     "sentence-transformers == 2.5.1",
     "transformers >= 4.28.0",
@@ -91,15 +90,14 @@
 
 [project.optional-dependencies]
 prod = [
     "google-auth == 2.23.3",
     "stripe == 7.3.0",
     "twilio == 8.11",
     "boto3 >= 1.34.57",
-    "resend >= 0.8.0",
 ]
 dev = [
     "khoj-assistant[prod]",
     "pytest >= 7.1.2",
     "pytest-xdist[psutil]",
     "pytest-django == 4.5.2",
     "pytest-asyncio == 0.21.1",
```

### Comparing `khoj_assistant-1.9.1.dev74/PKG-INFO` & `khoj_assistant-1.9.1.dev8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: khoj-assistant
-Version: 1.9.1.dev74
+Version: 1.9.1.dev8
 Summary: An AI copilot for your Second Brain
 Project-URL: Homepage, https://khoj.dev
 Project-URL: Documentation, https://docs.khoj.dev
 Project-URL: Code, https://github.com/khoj-ai/khoj
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -35,15 +35,14 @@
 Requires-Dist: httpx==0.25.0
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: langchain-openai>=0.0.5
 Requires-Dist: langchain<=0.2.0
 Requires-Dist: llama-cpp-python==0.2.56
 Requires-Dist: lxml==4.9.3
-Requires-Dist: magika~=0.5.1
 Requires-Dist: markdownify~=0.11.6
 Requires-Dist: openai-whisper>=20231117
 Requires-Dist: openai>=1.0.0
 Requires-Dist: pgvector==0.2.4
 Requires-Dist: phonenumbers==8.13.27
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: psycopg2-binary==2.9.9
@@ -74,15 +73,14 @@
 Requires-Dist: pytest-asyncio==0.21.1; extra == 'dev'
 Requires-Dist: pytest-django==4.5.2; extra == 'dev'
 Requires-Dist: pytest-xdist[psutil]; extra == 'dev'
 Requires-Dist: pytest>=7.1.2; extra == 'dev'
 Provides-Extra: prod
 Requires-Dist: boto3>=1.34.57; extra == 'prod'
 Requires-Dist: google-auth==2.23.3; extra == 'prod'
-Requires-Dist: resend>=0.8.0; extra == 'prod'
 Requires-Dist: stripe==7.3.0; extra == 'prod'
 Requires-Dist: twilio==8.11; extra == 'prod'
 Description-Content-Type: text/markdown
 
 <p align="center"><img src="src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png" width="230" alt="Khoj Logo"></p>
 
 <div align="center">
@@ -146,14 +144,7 @@
 Cheers to our awesome contributors! 🎉
 
 <a href="https://github.com/khoj-ai/khoj/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=khoj-ai/khoj" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
-
-## [Sponsors](https://github.com/sponsors/khoj-ai)
-Shout out to our brilliant sponsors! 🌈
-
-<a href="http://github.com/beekeeb">
-  <img src="https://raw.githubusercontent.com/beekeeb/piantor/main/docs/beekeeb.png" width=250/>
-</a>
```

