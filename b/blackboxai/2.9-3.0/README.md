# Comparing `tmp/blackboxai-2.9.tar.gz` & `tmp/blackboxai-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxai-2.9.tar", last modified: Sat May 25 20:40:27 2024, max compression
+gzip compressed data, was "blackboxai-3.0.tar", last modified: Sun May 26 01:31:43 2024, max compression
```

## Comparing `blackboxai-2.9.tar` & `blackboxai-3.0.tar`

### file list

```diff
@@ -1,302 +1,302 @@
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.395805 blackboxai-2.9/
--rw-rw-r--   0 em         (501) staff       (20)    33813 2024-05-10 07:30:29.000000 blackboxai-2.9/LICENSE
--rw-r--r--   0 em         (501) staff       (20)      750 2024-05-25 20:40:27.395573 blackboxai-2.9/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)      635 2024-05-19 15:41:33.000000 blackboxai-2.9/README.md
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.360853 blackboxai-2.9/blackboxai/
--rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     2718 2024-05-19 20:10:15.000000 blackboxai-2.9/blackboxai/chat.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.360986 blackboxai-2.9/blackboxai/interpreter/
--rw-r--r--   0 em         (501) staff       (20)      652 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.362185 blackboxai-2.9/blackboxai/interpreter/core/
--rw-r--r--   0 em         (501) staff       (20)     2820 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.362563 blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/
--rw-r--r--   0 em         (501) staff       (20)     1293 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-r--r--   0 em         (501) staff       (20)     3138 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     3046 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/browser.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.362774 blackboxai-2.9/blackboxai/interpreter/core/computer/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.363038 blackboxai-2.9/blackboxai/interpreter/core/computer/ai/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/ai/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     5688 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.363268 blackboxai-2.9/blackboxai/interpreter/core/computer/browser/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/browser/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      416 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.363516 blackboxai-2.9/blackboxai/interpreter/core/computer/calendar/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/calendar/__init__.py
--rw-r--r--   0 em         (501) staff       (20)    12950 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/calendar/calendar.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.363788 blackboxai-2.9/blackboxai/interpreter/core/computer/clipboard/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/clipboard/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      879 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/clipboard/clipboard.py
--rw-r--r--   0 em         (501) staff       (20)     2831 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/computer.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.364101 blackboxai-2.9/blackboxai/interpreter/core/computer/contacts/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/contacts/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     3293 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/contacts/contacts.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.364360 blackboxai-2.9/blackboxai/interpreter/core/computer/display/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/display/__init__.py
--rw-r--r--   0 em         (501) staff       (20)    10556 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.364609 blackboxai-2.9/blackboxai/interpreter/core/computer/docs/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/docs/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      749 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.364860 blackboxai-2.9/blackboxai/interpreter/core/computer/files/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/files/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     1698 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.365107 blackboxai-2.9/blackboxai/interpreter/core/computer/keyboard/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/keyboard/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     3553 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.365326 blackboxai-2.9/blackboxai/interpreter/core/computer/mail/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/mail/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     6350 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/mail/mail.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.365534 blackboxai-2.9/blackboxai/interpreter/core/computer/mouse/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/mouse/__init__.py
--rw-r--r--   0 em         (501) staff       (20)    12423 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.365747 blackboxai-2.9/blackboxai/interpreter/core/computer/os/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/os/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     2961 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.365954 blackboxai-2.9/blackboxai/interpreter/core/computer/skills/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/skills/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     4535 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.366171 blackboxai-2.9/blackboxai/interpreter/core/computer/sms/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/sms/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     1399 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/sms/sms.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.366547 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     1090 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.368105 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/
--rw-r--r--   0 em         (501) staff       (20)     5164 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     1812 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
--rw-r--r--   0 em         (501) staff       (20)      858 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/html.py
--rw-r--r--   0 em         (501) staff       (20)     1924 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
--rw-r--r--   0 em         (501) staff       (20)    15293 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-r--r--   0 em         (501) staff       (20)     2193 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
--rw-r--r--   0 em         (501) staff       (20)      293 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/python.py
--rw-r--r--   0 em         (501) staff       (20)     2360 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/r.py
--rw-r--r--   0 em         (501) staff       (20)     2503 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/react.py
--rw-r--r--   0 em         (501) staff       (20)     2727 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/shell.py
--rw-r--r--   0 em         (501) staff       (20)     6715 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-r--r--   0 em         (501) staff       (20)     4946 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.368945 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     7097 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/computer_vision.py
--rw-r--r--   0 em         (501) staff       (20)     1479 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/get_active_window.py
--rw-r--r--   0 em         (501) staff       (20)      929 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
--rw-r--r--   0 em         (501) staff       (20)      396 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/recipient_utils.py
--rw-r--r--   0 em         (501) staff       (20)      586 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/computer/utils/run_applescript.py
--rw-r--r--   0 em         (501) staff       (20)    14532 2024-05-19 20:28:04.000000 blackboxai-2.9/blackboxai/interpreter/core/core.py
--rw-r--r--   0 em         (501) staff       (20)     3288 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/default_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.369710 blackboxai-2.9/blackboxai/interpreter/core/llm/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     7323 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/agent_llm.py
--rw-r--r--   0 em         (501) staff       (20)     9084 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/llm.py
--rw-r--r--   0 em         (501) staff       (20)     5052 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/run_function_calling_llm.py
--rw-r--r--   0 em         (501) staff       (20)     3899 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.370313 blackboxai-2.9/blackboxai/interpreter/core/llm/utils/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/utils/__init__.py
--rw-r--r--   0 em         (501) staff       (20)    11769 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-r--r--   0 em         (501) staff       (20)      711 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/utils/merge_deltas.py
--rw-r--r--   0 em         (501) staff       (20)     1800 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
--rw-r--r--   0 em         (501) staff       (20)      538 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/llm/vision_for_text_llms.py
--rw-r--r--   0 em         (501) staff       (20)     1688 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/render_message.py
--rw-r--r--   0 em         (501) staff       (20)    14523 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/respond.py
--rw-r--r--   0 em         (501) staff       (20)      696 2024-05-19 20:28:05.000000 blackboxai-2.9/blackboxai/interpreter/core/search.py
--rw-r--r--   0 em         (501) staff       (20)     6162 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/server.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.371738 blackboxai-2.9/blackboxai/interpreter/core/utils/
--rw-r--r--   0 em         (501) staff       (20)      630 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
--rw-r--r--   0 em         (501) staff       (20)      360 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-r--r--   0 em         (501) staff       (20)     1096 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      920 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/lazy_import.py
--rw-r--r--   0 em         (501) staff       (20)     2118 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/scan_code.py
--rw-r--r--   0 em         (501) staff       (20)     4404 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/system_debug_info.py
--rw-r--r--   0 em         (501) staff       (20)     1736 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/telemetry.py
--rw-r--r--   0 em         (501) staff       (20)     1098 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/temporary_file.py
--rw-r--r--   0 em         (501) staff       (20)      510 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.372775 blackboxai-2.9/blackboxai/interpreter/terminal_interface/
--rw-r--r--   0 em         (501) staff       (20)     2433 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.373280 blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/__init__.py
--rw-r--r--   0 em         (501) staff       (20)      611 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/base_block.py
--rw-r--r--   0 em         (501) staff       (20)     2664 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/code_block.py
--rw-r--r--   0 em         (501) staff       (20)     1386 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/message_block.py
--rw-r--r--   0 em         (501) staff       (20)     2905 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/conversation_navigator.py
--rw-r--r--   0 em         (501) staff       (20)    10586 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/magic_commands.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.373647 blackboxai-2.9/blackboxai/interpreter/terminal_interface/profiles/
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/profiles/__init__.py
--rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
--rw-r--r--   0 em         (501) staff       (20)    40533 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/profiles/profiles.py
--rw-r--r--   0 em         (501) staff       (20)     2304 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/render_past_conversation.py
--rw-r--r--   0 em         (501) staff       (20)    14917 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
--rw-r--r--   0 em         (501) staff       (20)    27494 2024-05-19 20:28:04.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.375597 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/
--rw-r--r--   0 em         (501) staff       (20)    25835 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-r--r--   0 em         (501) staff       (20)     3099 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     4954 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/agent_utils.py
--rw-r--r--   0 em         (501) staff       (20)      512 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
--rw-r--r--   0 em         (501) staff       (20)      481 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
--rw-r--r--   0 em         (501) staff       (20)      419 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/cli_input.py
--rw-r--r--   0 em         (501) staff       (20)     1939 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
--rw-r--r--   0 em         (501) staff       (20)      884 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-r--r--   0 em         (501) staff       (20)     3069 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/display_output.py
--rw-r--r--   0 em         (501) staff       (20)      459 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
--rw-r--r--   0 em         (501) staff       (20)      250 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
--rw-r--r--   0 em         (501) staff       (20)      184 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-r--r--   0 em         (501) staff       (20)      316 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
--rw-r--r--   0 em         (501) staff       (20)       79 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
--rw-r--r--   0 em         (501) staff       (20)     2887 2024-05-18 20:28:33.000000 blackboxai-2.9/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.395218 blackboxai-2.9/blackboxai.egg-info/
--rw-r--r--   0 em         (501) staff       (20)      750 2024-05-25 20:40:27.000000 blackboxai-2.9/blackboxai.egg-info/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)    12938 2024-05-25 20:40:27.000000 blackboxai-2.9/blackboxai.egg-info/SOURCES.txt
--rw-r--r--   0 em         (501) staff       (20)        1 2024-05-25 20:40:27.000000 blackboxai-2.9/blackboxai.egg-info/dependency_links.txt
--rw-r--r--   0 em         (501) staff       (20)       50 2024-05-25 20:40:27.000000 blackboxai-2.9/blackboxai.egg-info/entry_points.txt
--rw-r--r--   0 em         (501) staff       (20)       23 2024-05-25 20:40:27.000000 blackboxai-2.9/blackboxai.egg-info/top_level.txt
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.375822 blackboxai-2.9/interpreter/
--rw-rw-r--   0 em         (501) staff       (20)      652 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.377202 blackboxai-2.9/interpreter/core/
--rw-rw-r--   0 em         (501) staff       (20)     2820 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.377583 blackboxai-2.9/interpreter/core/ARCHIVE_rag/
--rw-rw-r--   0 em         (501) staff       (20)     1293 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-rw-r--   0 em         (501) staff       (20)     3138 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/ARCHIVE_rag/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     3046 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/browser.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.377782 blackboxai-2.9/interpreter/core/computer/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.378013 blackboxai-2.9/interpreter/core/computer/ai/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/ai/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     5688 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.378434 blackboxai-2.9/interpreter/core/computer/browser/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/browser/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      416 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.379070 blackboxai-2.9/interpreter/core/computer/calendar/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/calendar/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    12950 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/calendar/calendar.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.379705 blackboxai-2.9/interpreter/core/computer/clipboard/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/clipboard/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      879 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/clipboard/clipboard.py
--rw-rw-r--   0 em         (501) staff       (20)     2831 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/computer.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.380436 blackboxai-2.9/interpreter/core/computer/contacts/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/contacts/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     3293 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/contacts/contacts.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.381244 blackboxai-2.9/interpreter/core/computer/display/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/display/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    10556 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.381527 blackboxai-2.9/interpreter/core/computer/docs/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/docs/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      749 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.381756 blackboxai-2.9/interpreter/core/computer/files/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/files/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1698 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.381992 blackboxai-2.9/interpreter/core/computer/keyboard/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/keyboard/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     3553 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.382259 blackboxai-2.9/interpreter/core/computer/mail/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/mail/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     6350 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/mail/mail.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.382625 blackboxai-2.9/interpreter/core/computer/mouse/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/mouse/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    12423 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.382872 blackboxai-2.9/interpreter/core/computer/os/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/os/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     2955 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.383089 blackboxai-2.9/interpreter/core/computer/skills/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/skills/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     4535 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.383318 blackboxai-2.9/interpreter/core/computer/sms/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/sms/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1399 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/sms/sms.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.383636 blackboxai-2.9/interpreter/core/computer/terminal/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1090 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.385276 blackboxai-2.9/interpreter/core/computer/terminal/languages/
--rw-rw-r--   0 em         (501) staff       (20)     5164 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1812 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/applescript.py
--rw-rw-r--   0 em         (501) staff       (20)      858 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/html.py
--rw-rw-r--   0 em         (501) staff       (20)     1924 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/javascript.py
--rw-rw-r--   0 em         (501) staff       (20)    15287 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-rw-r--   0 em         (501) staff       (20)     2193 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/powershell.py
--rw-rw-r--   0 em         (501) staff       (20)      293 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/python.py
--rw-rw-r--   0 em         (501) staff       (20)     2360 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/r.py
--rw-rw-r--   0 em         (501) staff       (20)     2503 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/react.py
--rw-rw-r--   0 em         (501) staff       (20)     2727 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/shell.py
--rw-rw-r--   0 em         (501) staff       (20)     6715 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-rw-r--   0 em         (501) staff       (20)     4994 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.386112 blackboxai-2.9/interpreter/core/computer/utils/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     7097 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/computer_vision.py
--rw-rw-r--   0 em         (501) staff       (20)     1479 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/get_active_window.py
--rw-rw-r--   0 em         (501) staff       (20)      929 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/html_to_png_base64.py
--rw-rw-r--   0 em         (501) staff       (20)      396 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/recipient_utils.py
--rw-rw-r--   0 em         (501) staff       (20)      586 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/computer/utils/run_applescript.py
--rw-rw-r--   0 em         (501) staff       (20)    14529 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/core.py
--rw-rw-r--   0 em         (501) staff       (20)     3676 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/default_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.386959 blackboxai-2.9/interpreter/core/llm/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     7323 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/agent_llm.py
--rw-rw-r--   0 em         (501) staff       (20)    11091 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/llm.py
--rw-rw-r--   0 em         (501) staff       (20)     5052 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/run_function_calling_llm.py
--rw-rw-r--   0 em         (501) staff       (20)     3900 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.387530 blackboxai-2.9/interpreter/core/llm/utils/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/utils/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    11769 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-rw-r--   0 em         (501) staff       (20)      711 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/utils/merge_deltas.py
--rw-rw-r--   0 em         (501) staff       (20)     1800 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/utils/parse_partial_json.py
--rw-rw-r--   0 em         (501) staff       (20)      538 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/llm/vision_for_text_llms.py
--rw-rw-r--   0 em         (501) staff       (20)     1688 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/render_message.py
--rw-rw-r--   0 em         (501) staff       (20)    15395 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/respond.py
--rw-rw-r--   0 em         (501) staff       (20)      696 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/search.py
--rw-rw-r--   0 em         (501) staff       (20)     6162 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/server.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.388966 blackboxai-2.9/interpreter/core/utils/
--rw-rw-r--   0 em         (501) staff       (20)      630 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/ARCHIVE_embed.py
--rw-rw-r--   0 em         (501) staff       (20)      360 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-rw-r--   0 em         (501) staff       (20)     1096 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      920 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/lazy_import.py
--rw-rw-r--   0 em         (501) staff       (20)     2118 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/scan_code.py
--rw-rw-r--   0 em         (501) staff       (20)     4404 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/system_debug_info.py
--rw-rw-r--   0 em         (501) staff       (20)     1736 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/telemetry.py
--rw-rw-r--   0 em         (501) staff       (20)     1098 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/temporary_file.py
--rw-rw-r--   0 em         (501) staff       (20)      510 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.390377 blackboxai-2.9/interpreter/terminal_interface/
--rw-rw-r--   0 em         (501) staff       (20)     2421 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.391036 blackboxai-2.9/interpreter/terminal_interface/components/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/components/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      611 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/components/base_block.py
--rw-rw-r--   0 em         (501) staff       (20)     2664 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/components/code_block.py
--rw-rw-r--   0 em         (501) staff       (20)     1386 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/components/message_block.py
--rw-rw-r--   0 em         (501) staff       (20)     2905 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/conversation_navigator.py
--rw-rw-r--   0 em         (501) staff       (20)    10580 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/magic_commands.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.391497 blackboxai-2.9/interpreter/terminal_interface/profiles/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/profiles/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)       25 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/profiles/historical_profiles.py
--rw-rw-r--   0 em         (501) staff       (20)    40437 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/profiles/profiles.py
--rw-rw-r--   0 em         (501) staff       (20)     2304 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/render_past_conversation.py
--rw-rw-r--   0 em         (501) staff       (20)    14875 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/start_terminal_interface.py
--rw-rw-r--   0 em         (501) staff       (20)    28411 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.394047 blackboxai-2.9/interpreter/terminal_interface/utils/
--rw-rw-r--   0 em         (501) staff       (20)    25763 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-rw-r--   0 em         (501) staff       (20)     3099 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     4954 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/agent_utils.py
--rw-rw-r--   0 em         (501) staff       (20)      512 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/check_for_package.py
--rw-rw-r--   0 em         (501) staff       (20)      481 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/check_for_update.py
--rw-rw-r--   0 em         (501) staff       (20)      419 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/cli_input.py
--rw-rw-r--   0 em         (501) staff       (20)     1939 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/count_tokens.py
--rw-rw-r--   0 em         (501) staff       (20)      884 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-rw-r--   0 em         (501) staff       (20)     3069 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/display_output.py
--rw-rw-r--   0 em         (501) staff       (20)      459 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/find_image_path.py
--rw-rw-r--   0 em         (501) staff       (20)      250 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/get_conversations.py
--rw-rw-r--   0 em         (501) staff       (20)      184 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-rw-r--   0 em         (501) staff       (20)      316 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/local_storage_path.py
--rw-rw-r--   0 em         (501) staff       (20)       79 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/utils/oi_dir.py
--rw-rw-r--   0 em         (501) staff       (20)     2881 2024-05-25 19:05:34.000000 blackboxai-2.9/interpreter/terminal_interface/validate_llm_settings.py
--rw-r--r--   0 em         (501) staff       (20)     1959 2024-05-19 20:24:51.000000 blackboxai-2.9/pyproject.toml
--rw-r--r--   0 em         (501) staff       (20)       38 2024-05-25 20:40:27.395854 blackboxai-2.9/setup.cfg
--rw-r--r--   0 em         (501) staff       (20)      523 2024-05-25 20:39:59.000000 blackboxai-2.9/setup.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-25 20:40:27.394954 blackboxai-2.9/tests/
--rw-r--r--   0 em         (501) staff       (20)    21812 2024-05-18 20:28:33.000000 blackboxai-2.9/tests/test_interpreter.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.269504 blackboxai-3.0/
+-rw-rw-r--   0 em         (501) staff       (20)    33813 2024-05-10 07:30:29.000000 blackboxai-3.0/LICENSE
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 01:31:43.269287 blackboxai-3.0/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)      635 2024-05-19 15:41:33.000000 blackboxai-3.0/README.md
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.222270 blackboxai-3.0/blackboxai/
+-rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     2718 2024-05-19 20:10:15.000000 blackboxai-3.0/blackboxai/chat.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.222658 blackboxai-3.0/blackboxai/interpreter/
+-rw-r--r--   0 em         (501) staff       (20)      652 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.224816 blackboxai-3.0/blackboxai/interpreter/core/
+-rw-r--r--   0 em         (501) staff       (20)     2820 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.225489 blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/
+-rw-r--r--   0 em         (501) staff       (20)     1293 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-r--r--   0 em         (501) staff       (20)     3138 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3046 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.225740 blackboxai-3.0/blackboxai/interpreter/core/computer/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.226065 blackboxai-3.0/blackboxai/interpreter/core/computer/ai/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/ai/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     5688 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.226379 blackboxai-3.0/blackboxai/interpreter/core/computer/browser/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/browser/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      416 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.226679 blackboxai-3.0/blackboxai/interpreter/core/computer/calendar/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/calendar/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    12950 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.226971 blackboxai-3.0/blackboxai/interpreter/core/computer/clipboard/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/clipboard/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      879 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/clipboard/clipboard.py
+-rw-r--r--   0 em         (501) staff       (20)     2831 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/computer.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.227243 blackboxai-3.0/blackboxai/interpreter/core/computer/contacts/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/contacts/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3293 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.227521 blackboxai-3.0/blackboxai/interpreter/core/computer/display/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/display/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    10556 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.227819 blackboxai-3.0/blackboxai/interpreter/core/computer/docs/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/docs/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      749 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.228110 blackboxai-3.0/blackboxai/interpreter/core/computer/files/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/files/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1698 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.228458 blackboxai-3.0/blackboxai/interpreter/core/computer/keyboard/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/keyboard/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     3553 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.229763 blackboxai-3.0/blackboxai/interpreter/core/computer/mail/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/mail/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     6350 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.230070 blackboxai-3.0/blackboxai/interpreter/core/computer/mouse/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/mouse/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    12423 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.230420 blackboxai-3.0/blackboxai/interpreter/core/computer/os/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/os/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     2961 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.230791 blackboxai-3.0/blackboxai/interpreter/core/computer/skills/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/skills/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     4535 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.231072 blackboxai-3.0/blackboxai/interpreter/core/computer/sms/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/sms/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1399 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.231570 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1090 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.233954 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/
+-rw-r--r--   0 em         (501) staff       (20)     5164 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     1812 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
+-rw-r--r--   0 em         (501) staff       (20)      858 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/html.py
+-rw-r--r--   0 em         (501) staff       (20)     1924 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
+-rw-r--r--   0 em         (501) staff       (20)    15293 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-r--r--   0 em         (501) staff       (20)     2193 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
+-rw-r--r--   0 em         (501) staff       (20)      293 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/python.py
+-rw-r--r--   0 em         (501) staff       (20)     2360 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/r.py
+-rw-r--r--   0 em         (501) staff       (20)     2503 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/react.py
+-rw-r--r--   0 em         (501) staff       (20)     2727 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/shell.py
+-rw-r--r--   0 em         (501) staff       (20)     6715 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-r--r--   0 em         (501) staff       (20)     4567 2024-05-26 01:30:29.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.235027 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     7097 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/computer_vision.py
+-rw-r--r--   0 em         (501) staff       (20)     1479 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/get_active_window.py
+-rw-r--r--   0 em         (501) staff       (20)      929 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-r--r--   0 em         (501) staff       (20)      396 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/recipient_utils.py
+-rw-r--r--   0 em         (501) staff       (20)      586 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/computer/utils/run_applescript.py
+-rw-r--r--   0 em         (501) staff       (20)    14532 2024-05-19 20:28:04.000000 blackboxai-3.0/blackboxai/interpreter/core/core.py
+-rw-r--r--   0 em         (501) staff       (20)     3288 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/default_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.236021 blackboxai-3.0/blackboxai/interpreter/core/llm/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     7323 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/agent_llm.py
+-rw-r--r--   0 em         (501) staff       (20)     9084 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/llm.py
+-rw-r--r--   0 em         (501) staff       (20)     5052 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/run_function_calling_llm.py
+-rw-r--r--   0 em         (501) staff       (20)     3899 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.236650 blackboxai-3.0/blackboxai/interpreter/core/llm/utils/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)    11769 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-r--r--   0 em         (501) staff       (20)      711 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/utils/merge_deltas.py
+-rw-r--r--   0 em         (501) staff       (20)     1800 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
+-rw-r--r--   0 em         (501) staff       (20)      538 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/llm/vision_for_text_llms.py
+-rw-r--r--   0 em         (501) staff       (20)     1688 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/render_message.py
+-rw-r--r--   0 em         (501) staff       (20)    14523 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/respond.py
+-rw-r--r--   0 em         (501) staff       (20)      696 2024-05-19 20:28:05.000000 blackboxai-3.0/blackboxai/interpreter/core/search.py
+-rw-r--r--   0 em         (501) staff       (20)     6162 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/server.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.238193 blackboxai-3.0/blackboxai/interpreter/core/utils/
+-rw-r--r--   0 em         (501) staff       (20)      630 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
+-rw-r--r--   0 em         (501) staff       (20)      360 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-r--r--   0 em         (501) staff       (20)     1096 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      920 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/lazy_import.py
+-rw-r--r--   0 em         (501) staff       (20)     2118 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/scan_code.py
+-rw-r--r--   0 em         (501) staff       (20)     4404 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/system_debug_info.py
+-rw-r--r--   0 em         (501) staff       (20)     1736 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/telemetry.py
+-rw-r--r--   0 em         (501) staff       (20)     1098 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/temporary_file.py
+-rw-r--r--   0 em         (501) staff       (20)      510 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.240030 blackboxai-3.0/blackboxai/interpreter/terminal_interface/
+-rw-r--r--   0 em         (501) staff       (20)     2433 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.240647 blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)      611 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/base_block.py
+-rw-r--r--   0 em         (501) staff       (20)     2664 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/code_block.py
+-rw-r--r--   0 em         (501) staff       (20)     1386 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/message_block.py
+-rw-r--r--   0 em         (501) staff       (20)     2905 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/conversation_navigator.py
+-rw-r--r--   0 em         (501) staff       (20)    10586 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.241061 blackboxai-3.0/blackboxai/interpreter/terminal_interface/profiles/
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/profiles/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-r--r--   0 em         (501) staff       (20)    40533 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/profiles/profiles.py
+-rw-r--r--   0 em         (501) staff       (20)     2304 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/render_past_conversation.py
+-rw-r--r--   0 em         (501) staff       (20)    14917 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
+-rw-r--r--   0 em         (501) staff       (20)    27494 2024-05-19 20:28:04.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.243483 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/
+-rw-r--r--   0 em         (501) staff       (20)    25835 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-r--r--   0 em         (501) staff       (20)     3099 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-r--r--   0 em         (501) staff       (20)        0 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     4954 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/agent_utils.py
+-rw-r--r--   0 em         (501) staff       (20)      512 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
+-rw-r--r--   0 em         (501) staff       (20)      481 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
+-rw-r--r--   0 em         (501) staff       (20)      419 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/cli_input.py
+-rw-r--r--   0 em         (501) staff       (20)     1939 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
+-rw-r--r--   0 em         (501) staff       (20)      884 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-r--r--   0 em         (501) staff       (20)     3069 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/display_output.py
+-rw-r--r--   0 em         (501) staff       (20)      459 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
+-rw-r--r--   0 em         (501) staff       (20)      250 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
+-rw-r--r--   0 em         (501) staff       (20)      184 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-r--r--   0 em         (501) staff       (20)      316 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-r--r--   0 em         (501) staff       (20)       79 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
+-rw-r--r--   0 em         (501) staff       (20)     2887 2024-05-18 20:28:33.000000 blackboxai-3.0/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.269000 blackboxai-3.0/blackboxai.egg-info/
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 01:31:43.000000 blackboxai-3.0/blackboxai.egg-info/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)    12938 2024-05-26 01:31:43.000000 blackboxai-3.0/blackboxai.egg-info/SOURCES.txt
+-rw-r--r--   0 em         (501) staff       (20)        1 2024-05-26 01:31:43.000000 blackboxai-3.0/blackboxai.egg-info/dependency_links.txt
+-rw-r--r--   0 em         (501) staff       (20)       50 2024-05-26 01:31:43.000000 blackboxai-3.0/blackboxai.egg-info/entry_points.txt
+-rw-r--r--   0 em         (501) staff       (20)       23 2024-05-26 01:31:43.000000 blackboxai-3.0/blackboxai.egg-info/top_level.txt
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.243631 blackboxai-3.0/interpreter/
+-rw-rw-r--   0 em         (501) staff       (20)      652 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.246212 blackboxai-3.0/interpreter/core/
+-rw-rw-r--   0 em         (501) staff       (20)     2820 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.246752 blackboxai-3.0/interpreter/core/ARCHIVE_rag/
+-rw-rw-r--   0 em         (501) staff       (20)     1293 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     3138 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3046 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.246966 blackboxai-3.0/interpreter/core/computer/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.247470 blackboxai-3.0/interpreter/core/computer/ai/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/ai/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     5688 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.247892 blackboxai-3.0/interpreter/core/computer/browser/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/browser/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      416 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.248254 blackboxai-3.0/interpreter/core/computer/calendar/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/calendar/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12950 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.248510 blackboxai-3.0/interpreter/core/computer/clipboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/clipboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      879 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/clipboard/clipboard.py
+-rw-rw-r--   0 em         (501) staff       (20)     2831 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/computer.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.248781 blackboxai-3.0/interpreter/core/computer/contacts/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/contacts/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3293 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.249127 blackboxai-3.0/interpreter/core/computer/display/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/display/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    10556 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.249410 blackboxai-3.0/interpreter/core/computer/docs/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/docs/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      749 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.249828 blackboxai-3.0/interpreter/core/computer/files/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/files/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1698 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.250170 blackboxai-3.0/interpreter/core/computer/keyboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/keyboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3553 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.250633 blackboxai-3.0/interpreter/core/computer/mail/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/mail/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     6350 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.250925 blackboxai-3.0/interpreter/core/computer/mouse/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/mouse/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12423 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.251275 blackboxai-3.0/interpreter/core/computer/os/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/os/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     2955 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.251529 blackboxai-3.0/interpreter/core/computer/skills/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/skills/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     4535 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.251847 blackboxai-3.0/interpreter/core/computer/sms/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/sms/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1399 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.252483 blackboxai-3.0/interpreter/core/computer/terminal/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1090 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.254661 blackboxai-3.0/interpreter/core/computer/terminal/languages/
+-rw-rw-r--   0 em         (501) staff       (20)     5164 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1812 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)      858 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/html.py
+-rw-rw-r--   0 em         (501) staff       (20)     1924 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/javascript.py
+-rw-rw-r--   0 em         (501) staff       (20)    15287 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     2193 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/powershell.py
+-rw-rw-r--   0 em         (501) staff       (20)      293 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/python.py
+-rw-rw-r--   0 em         (501) staff       (20)     2360 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/r.py
+-rw-rw-r--   0 em         (501) staff       (20)     2503 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/react.py
+-rw-rw-r--   0 em         (501) staff       (20)     2727 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/shell.py
+-rw-rw-r--   0 em         (501) staff       (20)     6715 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     4994 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.255720 blackboxai-3.0/interpreter/core/computer/utils/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     7097 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/computer_vision.py
+-rw-rw-r--   0 em         (501) staff       (20)     1479 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/get_active_window.py
+-rw-rw-r--   0 em         (501) staff       (20)      929 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-rw-r--   0 em         (501) staff       (20)      396 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/recipient_utils.py
+-rw-rw-r--   0 em         (501) staff       (20)      586 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/computer/utils/run_applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)    14529 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/core.py
+-rw-rw-r--   0 em         (501) staff       (20)     3676 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/default_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.256918 blackboxai-3.0/interpreter/core/llm/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     7323 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/agent_llm.py
+-rw-rw-r--   0 em         (501) staff       (20)    11091 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     5052 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/run_function_calling_llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     3900 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.257563 blackboxai-3.0/interpreter/core/llm/utils/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    11769 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-rw-r--   0 em         (501) staff       (20)      711 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/utils/merge_deltas.py
+-rw-rw-r--   0 em         (501) staff       (20)     1800 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/utils/parse_partial_json.py
+-rw-rw-r--   0 em         (501) staff       (20)      538 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/llm/vision_for_text_llms.py
+-rw-rw-r--   0 em         (501) staff       (20)     1688 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/render_message.py
+-rw-rw-r--   0 em         (501) staff       (20)    15395 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/respond.py
+-rw-rw-r--   0 em         (501) staff       (20)      696 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/search.py
+-rw-rw-r--   0 em         (501) staff       (20)     6162 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/server.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.259571 blackboxai-3.0/interpreter/core/utils/
+-rw-rw-r--   0 em         (501) staff       (20)      630 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/ARCHIVE_embed.py
+-rw-rw-r--   0 em         (501) staff       (20)      360 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     1096 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      920 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/lazy_import.py
+-rw-rw-r--   0 em         (501) staff       (20)     2118 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/scan_code.py
+-rw-rw-r--   0 em         (501) staff       (20)     4404 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/system_debug_info.py
+-rw-rw-r--   0 em         (501) staff       (20)     1736 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/telemetry.py
+-rw-rw-r--   0 em         (501) staff       (20)     1098 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/temporary_file.py
+-rw-rw-r--   0 em         (501) staff       (20)      510 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.261130 blackboxai-3.0/interpreter/terminal_interface/
+-rw-rw-r--   0 em         (501) staff       (20)     2421 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.261965 blackboxai-3.0/interpreter/terminal_interface/components/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/components/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      611 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/components/base_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2664 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/components/code_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     1386 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/components/message_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2905 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/conversation_navigator.py
+-rw-rw-r--   0 em         (501) staff       (20)    10580 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.262479 blackboxai-3.0/interpreter/terminal_interface/profiles/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/profiles/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)       25 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)    40437 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/profiles/profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)     2304 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/render_past_conversation.py
+-rw-rw-r--   0 em         (501) staff       (20)    14875 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/start_terminal_interface.py
+-rw-rw-r--   0 em         (501) staff       (20)    28411 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.267448 blackboxai-3.0/interpreter/terminal_interface/utils/
+-rw-rw-r--   0 em         (501) staff       (20)    25763 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-rw-r--   0 em         (501) staff       (20)     3099 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     4954 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/agent_utils.py
+-rw-rw-r--   0 em         (501) staff       (20)      512 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/check_for_package.py
+-rw-rw-r--   0 em         (501) staff       (20)      481 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/check_for_update.py
+-rw-rw-r--   0 em         (501) staff       (20)      419 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/cli_input.py
+-rw-rw-r--   0 em         (501) staff       (20)     1939 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/count_tokens.py
+-rw-rw-r--   0 em         (501) staff       (20)      884 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-rw-r--   0 em         (501) staff       (20)     3069 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/display_output.py
+-rw-rw-r--   0 em         (501) staff       (20)      459 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/find_image_path.py
+-rw-rw-r--   0 em         (501) staff       (20)      250 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/get_conversations.py
+-rw-rw-r--   0 em         (501) staff       (20)      184 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-rw-r--   0 em         (501) staff       (20)      316 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-rw-r--   0 em         (501) staff       (20)       79 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/utils/oi_dir.py
+-rw-rw-r--   0 em         (501) staff       (20)     2881 2024-05-25 19:05:34.000000 blackboxai-3.0/interpreter/terminal_interface/validate_llm_settings.py
+-rw-r--r--   0 em         (501) staff       (20)     1959 2024-05-19 20:24:51.000000 blackboxai-3.0/pyproject.toml
+-rw-r--r--   0 em         (501) staff       (20)       38 2024-05-26 01:31:43.269585 blackboxai-3.0/setup.cfg
+-rw-r--r--   0 em         (501) staff       (20)      523 2024-05-26 01:31:02.000000 blackboxai-3.0/setup.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 01:31:43.268537 blackboxai-3.0/tests/
+-rw-r--r--   0 em         (501) staff       (20)    21812 2024-05-18 20:28:33.000000 blackboxai-3.0/tests/test_interpreter.py
```

### Comparing `blackboxai-2.9/LICENSE` & `blackboxai-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/PKG-INFO` & `blackboxai-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.9
+Version: 3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
```

### Comparing `blackboxai-2.9/README.md` & `blackboxai-3.0/README.md`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/chat.py` & `blackboxai-3.0/blackboxai/chat.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/__init__.py` & `blackboxai-3.0/blackboxai/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-3.0/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/browser.py` & `blackboxai-3.0/blackboxai/interpreter/core/browser.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/ai/ai.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/calendar/calendar.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/computer.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/computer.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/contacts/contacts.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/contacts/contacts.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/display/display.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/display/display.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/docs/docs.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/files/files.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/mail/mail.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/mail/mail.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/mouse/mouse.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/os/os.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/skills/skills.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/skills/skills.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/sms/sms.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/sms/sms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/base_language.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/terminal/terminal.py` & `blackboxai-3.0/interpreter/core/computer/terminal/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             if not self.computer._has_imported_computer_api:
                 self.computer._has_imported_computer_api = True
                 # Give it access to the computer via Python
                 self.computer.run(
                     language="python",
                     code="import time\nfrom interpreter import interpreter\ncomputer = interpreter.computer",  # We ask it to use time, so
                     display=self.computer.verbose,
-                )
+                )   
 
         if stream == False:
             # If stream == False, *pull* from _streaming_run.
             output_messages = []
             for chunk in self._streaming_run(language, code, display=display):
                 if chunk.get("format") != "active_line":
                     # Should we append this to the last message, or make a new one?
@@ -70,15 +70,15 @@
             return self._streaming_run(language, code, display=display)
 
     def _streaming_run(self, language, code, display=False):
         if language not in self._active_languages:
             # Get the language. Pass in self.computer *if it takes a single argument*
             # but pass in nothing if not. This makes custom languages easier to add / understand.
             lang_class = self.get_language(language)
-            if lang_class.__init__.__code__.co_argcount > 1:
+            if "e2b" not in lang_class.__name__.lower() and lang_class.__init__.__code__.co_argcount > 1:
                 self._active_languages[language] = lang_class(self.computer)
             else:
                 self._active_languages[language] = lang_class()
         try:
             for chunk in self._active_languages[language].run(code):
                 # self.format_to_recipient can format some messages as having a certain recipient.
                 # Here we add that to the LMC messages:
```

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/computer/utils/run_applescript.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/utils/run_applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/core.py` & `blackboxai-3.0/blackboxai/interpreter/core/core.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/default_system_message.py` & `blackboxai-3.0/blackboxai/interpreter/core/default_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/agent_llm.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/agent_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/llm.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/run_text_llm.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/run_text_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-3.0/blackboxai/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/render_message.py` & `blackboxai-3.0/blackboxai/interpreter/core/render_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/respond.py` & `blackboxai-3.0/blackboxai/interpreter/core/respond.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/search.py` & `blackboxai-3.0/blackboxai/interpreter/core/search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/server.py` & `blackboxai-3.0/blackboxai/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/lazy_import.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/scan_code.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/system_debug_info.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/telemetry.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/core/utils/temporary_file.py` & `blackboxai-3.0/blackboxai/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/base_block.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/code_block.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/components/message_block.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/magic_commands.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/profiles/profiles.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/agent_utils.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-3.0/blackboxai/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/blackboxai.egg-info/PKG-INFO` & `blackboxai-3.0/blackboxai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.9
+Version: 3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
```

### Comparing `blackboxai-2.9/blackboxai.egg-info/SOURCES.txt` & `blackboxai-3.0/blackboxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/__init__.py` & `blackboxai-3.0/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-3.0/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-3.0/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-3.0/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/browser.py` & `blackboxai-3.0/interpreter/core/browser.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/ai/ai.py` & `blackboxai-3.0/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/calendar/calendar.py` & `blackboxai-3.0/interpreter/core/computer/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-3.0/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/computer.py` & `blackboxai-3.0/interpreter/core/computer/computer.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/contacts/contacts.py` & `blackboxai-3.0/interpreter/core/computer/contacts/contacts.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/display/display.py` & `blackboxai-3.0/interpreter/core/computer/display/display.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/docs/docs.py` & `blackboxai-3.0/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/files/files.py` & `blackboxai-3.0/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-3.0/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/mail/mail.py` & `blackboxai-3.0/interpreter/core/computer/mail/mail.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/mouse/mouse.py` & `blackboxai-3.0/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/os/os.py` & `blackboxai-3.0/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/skills/skills.py` & `blackboxai-3.0/interpreter/core/computer/skills/skills.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/sms/sms.py` & `blackboxai-3.0/interpreter/core/computer/sms/sms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/base_language.py` & `blackboxai-3.0/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-3.0/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/terminal/terminal.py` & `blackboxai-3.0/blackboxai/interpreter/core/computer/terminal/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .languages.html import HTML
 from .languages.javascript import JavaScript
 from .languages.powershell import PowerShell
 from .languages.python import Python
 from .languages.r import R
 from .languages.react import React
 from .languages.shell import Shell
+import inspect
 
 # Should this be renamed to OS or System?
 
 
 class Terminal:
     def __init__(self, computer):
         self.computer = computer
@@ -43,15 +44,15 @@
             if not self.computer._has_imported_computer_api:
                 self.computer._has_imported_computer_api = True
                 # Give it access to the computer via Python
                 self.computer.run(
                     language="python",
                     code="import time\nfrom interpreter import interpreter\ncomputer = interpreter.computer",  # We ask it to use time, so
                     display=self.computer.verbose,
-                )   
+                )
 
         if stream == False:
             # If stream == False, *pull* from _streaming_run.
             output_messages = []
             for chunk in self._streaming_run(language, code, display=display):
                 if chunk.get("format") != "active_line":
                     # Should we append this to the last message, or make a new one?
@@ -67,48 +68,45 @@
 
         elif stream == True:
             # If stream == True, replace this with _streaming_run.
             return self._streaming_run(language, code, display=display)
 
     def _streaming_run(self, language, code, display=False):
         if language not in self._active_languages:
-            # Get the language. Pass in self.computer *if it takes a single argument*
-            # but pass in nothing if not. This makes custom languages easier to add / understand.
             lang_class = self.get_language(language)
-            if "e2b" not in lang_class.__name__.lower() and lang_class.__init__.__code__.co_argcount > 1:
+            init_args = inspect.getfullargspec(lang_class.__init__).args
+            if len(init_args) > 1:
                 self._active_languages[language] = lang_class(self.computer)
             else:
                 self._active_languages[language] = lang_class()
         try:
             for chunk in self._active_languages[language].run(code):
-                # self.format_to_recipient can format some messages as having a certain recipient.
-                # Here we add that to the LMC messages:
                 if chunk["type"] == "console" and chunk.get("format") == "output":
                     recipient, content = parse_for_recipient(chunk["content"])
                     if recipient:
                         chunk["recipient"] = recipient
                         chunk["content"] = content
 
-                    # Sometimes, we want to hide the traceback to preserve tokens.
-                    # (is this a good idea?)
                     if "@@@HIDE_TRACEBACK@@@" in content:
                         chunk["content"] = (
                             "Stopping execution.\n\n"
                             + content.split("@@@HIDE_TRACEBACK@@@")[-1].strip()
                         )
 
                 yield chunk
 
-                # Print it also if display = True
                 if (
                     display
-                    and chunk.get("format") != "active_line"
+                    and chunk.get("format")!= "active_line"
                     and chunk.get("content")
                 ):
                     print(chunk["content"])
+        except Exception as e:
+            print(f"An error occurred: {e}")
+
 
         except GeneratorExit:
             self.stop()
 
     def stop(self):
         for language in self._active_languages.values():
             language.stop()
```

### Comparing `blackboxai-2.9/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-3.0/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-3.0/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-3.0/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/computer/utils/run_applescript.py` & `blackboxai-3.0/interpreter/core/computer/utils/run_applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/core.py` & `blackboxai-3.0/interpreter/core/core.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/default_system_message.py` & `blackboxai-3.0/interpreter/core/default_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/agent_llm.py` & `blackboxai-3.0/interpreter/core/llm/agent_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/llm.py` & `blackboxai-3.0/interpreter/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-3.0/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/run_text_llm.py` & `blackboxai-3.0/interpreter/core/llm/run_text_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-3.0/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-3.0/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-3.0/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-3.0/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/render_message.py` & `blackboxai-3.0/interpreter/core/render_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/respond.py` & `blackboxai-3.0/interpreter/core/respond.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/search.py` & `blackboxai-3.0/interpreter/core/search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/server.py` & `blackboxai-3.0/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-3.0/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-3.0/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/lazy_import.py` & `blackboxai-3.0/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/scan_code.py` & `blackboxai-3.0/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/system_debug_info.py` & `blackboxai-3.0/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/telemetry.py` & `blackboxai-3.0/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/core/utils/temporary_file.py` & `blackboxai-3.0/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-3.0/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/components/base_block.py` & `blackboxai-3.0/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/components/code_block.py` & `blackboxai-3.0/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/components/message_block.py` & `blackboxai-3.0/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-3.0/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/magic_commands.py` & `blackboxai-3.0/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/profiles/profiles.py` & `blackboxai-3.0/interpreter/terminal_interface/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-3.0/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-3.0/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-3.0/interpreter/terminal_interface/terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/agent_utils.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-3.0/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-3.0/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/pyproject.toml` & `blackboxai-3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboxai-2.9/setup.py` & `blackboxai-3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="blackboxai",
-    version="2.9",
+    version="3.0",
     packages=find_packages(),
     package_dir = {'': '.'},
     include_package_data=True,
     setup_requires= ['requests'],
     entry_points={
         "console_scripts": [
             "blackboxai = blackboxai:runChat"
```

### Comparing `blackboxai-2.9/tests/test_interpreter.py` & `blackboxai-3.0/tests/test_interpreter.py`

 * *Files identical despite different names*

