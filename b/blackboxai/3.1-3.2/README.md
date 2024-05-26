# Comparing `tmp/blackboxai-3.1.tar.gz` & `tmp/blackboxai-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxai-3.1.tar", last modified: Sun May 26 03:08:08 2024, max compression
+gzip compressed data, was "blackboxai-3.2.tar", last modified: Sun May 26 03:49:54 2024, max compression
```

## Comparing `blackboxai-3.1.tar` & `blackboxai-3.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.732331 blackboxai-3.1/
--rw-rw-r--   0 em         (501) staff       (20)    33813 2024-05-10 07:30:29.000000 blackboxai-3.1/LICENSE
--rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 03:08:08.732095 blackboxai-3.1/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)      635 2024-05-19 15:41:33.000000 blackboxai-3.1/README.md
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.703473 blackboxai-3.1/blackboxai/
--rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-3.1/blackboxai/__init__.py
--rw-r--r--   0 em         (501) staff       (20)     2718 2024-05-19 20:10:15.000000 blackboxai-3.1/blackboxai/chat.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.703814 blackboxai-3.1/blackboxai/interpreter/
--rw-rw-r--   0 em         (501) staff       (20)      633 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.709575 blackboxai-3.1/blackboxai/interpreter/core/
--rw-rw-r--   0 em         (501) staff       (20)     2820 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.710076 blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/
--rw-rw-r--   0 em         (501) staff       (20)     1293 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-rw-r--   0 em         (501) staff       (20)     3138 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.710282 blackboxai-3.1/blackboxai/interpreter/core/computer/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.710812 blackboxai-3.1/blackboxai/interpreter/core/computer/ai/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/ai/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     5688 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.711073 blackboxai-3.1/blackboxai/interpreter/core/computer/browser/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/browser/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      416 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.711337 blackboxai-3.1/blackboxai/interpreter/core/computer/calendar/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/calendar/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    12950 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/calendar/calendar.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.711617 blackboxai-3.1/blackboxai/interpreter/core/computer/clipboard/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/clipboard/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      879 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/clipboard/clipboard.py
--rw-rw-r--   0 em         (501) staff       (20)     2831 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/computer.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.712005 blackboxai-3.1/blackboxai/interpreter/core/computer/contacts/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/contacts/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     3293 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/contacts/contacts.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.712427 blackboxai-3.1/blackboxai/interpreter/core/computer/display/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/display/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    10556 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.712707 blackboxai-3.1/blackboxai/interpreter/core/computer/docs/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/docs/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      749 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.713089 blackboxai-3.1/blackboxai/interpreter/core/computer/files/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/files/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1698 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.713358 blackboxai-3.1/blackboxai/interpreter/core/computer/keyboard/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/keyboard/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     3553 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.714817 blackboxai-3.1/blackboxai/interpreter/core/computer/mail/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/mail/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     6350 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/mail/mail.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.715263 blackboxai-3.1/blackboxai/interpreter/core/computer/mouse/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/mouse/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)    12423 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.715749 blackboxai-3.1/blackboxai/interpreter/core/computer/os/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/os/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     2955 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.715950 blackboxai-3.1/blackboxai/interpreter/core/computer/skills/
--rw-rw-r--   0 em         (501) staff       (20)     4535 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.716377 blackboxai-3.1/blackboxai/interpreter/core/computer/sms/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/sms/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1399 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/sms/sms.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.716970 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1090 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.720627 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/
--rw-rw-r--   0 em         (501) staff       (20)     5164 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     1812 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
--rw-rw-r--   0 em         (501) staff       (20)      858 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/html.py
--rw-rw-r--   0 em         (501) staff       (20)     1924 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
--rw-rw-r--   0 em         (501) staff       (20)    15287 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-rw-r--   0 em         (501) staff       (20)     2193 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
--rw-rw-r--   0 em         (501) staff       (20)      293 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/python.py
--rw-rw-r--   0 em         (501) staff       (20)     2360 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/r.py
--rw-rw-r--   0 em         (501) staff       (20)     2503 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/react.py
--rw-rw-r--   0 em         (501) staff       (20)     2727 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/shell.py
--rw-rw-r--   0 em         (501) staff       (20)     6715 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-rw-r--   0 em         (501) staff       (20)     4946 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.721496 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/
--rw-rw-r--   0 em         (501) staff       (20)     7097 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/computer_vision.py
--rw-rw-r--   0 em         (501) staff       (20)     1479 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/get_active_window.py
--rw-rw-r--   0 em         (501) staff       (20)      929 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
--rw-rw-r--   0 em         (501) staff       (20)      396 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/recipient_utils.py
--rw-rw-r--   0 em         (501) staff       (20)      586 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/computer/utils/run_applescript.py
--rw-rw-r--   0 em         (501) staff       (20)    14297 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/core.py
--rw-rw-r--   0 em         (501) staff       (20)     3282 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/default_system_message.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.722338 blackboxai-3.1/blackboxai/interpreter/core/llm/
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)     8752 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/llm.py
--rw-rw-r--   0 em         (501) staff       (20)     5052 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/run_function_calling_llm.py
--rw-rw-r--   0 em         (501) staff       (20)     2616 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.722913 blackboxai-3.1/blackboxai/interpreter/core/llm/utils/
--rw-rw-r--   0 em         (501) staff       (20)     9479 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-rw-r--   0 em         (501) staff       (20)      711 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/utils/merge_deltas.py
--rw-rw-r--   0 em         (501) staff       (20)     1800 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
--rw-rw-r--   0 em         (501) staff       (20)      538 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/llm/vision_for_text_llms.py
--rw-rw-r--   0 em         (501) staff       (20)     1688 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/render_message.py
--rw-rw-r--   0 em         (501) staff       (20)    13491 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/respond.py
--rw-rw-r--   0 em         (501) staff       (20)     6162 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/server.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.725309 blackboxai-3.1/blackboxai/interpreter/core/utils/
--rw-rw-r--   0 em         (501) staff       (20)      630 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
--rw-rw-r--   0 em         (501) staff       (20)      360 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-rw-r--   0 em         (501) staff       (20)     1096 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/__init__.py
--rw-rw-r--   0 em         (501) staff       (20)      920 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/lazy_import.py
--rw-rw-r--   0 em         (501) staff       (20)     2118 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/scan_code.py
--rw-rw-r--   0 em         (501) staff       (20)     4404 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/system_debug_info.py
--rw-rw-r--   0 em         (501) staff       (20)     1736 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/telemetry.py
--rw-rw-r--   0 em         (501) staff       (20)     1098 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/temporary_file.py
--rw-rw-r--   0 em         (501) staff       (20)      510 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.727296 blackboxai-3.1/blackboxai/interpreter/terminal_interface/
--rw-rw-r--   0 em         (501) staff       (20)     2421 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.727902 blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/
--rw-rw-r--   0 em         (501) staff       (20)      611 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/base_block.py
--rw-rw-r--   0 em         (501) staff       (20)     2664 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/code_block.py
--rw-rw-r--   0 em         (501) staff       (20)     1386 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/message_block.py
--rw-rw-r--   0 em         (501) staff       (20)     2905 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/conversation_navigator.py
--rw-rw-r--   0 em         (501) staff       (20)    10580 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/magic_commands.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.728211 blackboxai-3.1/blackboxai/interpreter/terminal_interface/profiles/
--rw-rw-r--   0 em         (501) staff       (20)       25 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
--rw-rw-r--   0 em         (501) staff       (20)    40437 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/profiles/profiles.py
--rw-rw-r--   0 em         (501) staff       (20)     2304 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/render_past_conversation.py
--rw-rw-r--   0 em         (501) staff       (20)    14875 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
--rw-rw-r--   0 em         (501) staff       (20)    20287 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.730548 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/
--rw-rw-r--   0 em         (501) staff       (20)    25763 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-rw-r--   0 em         (501) staff       (20)     3099 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-rw-r--   0 em         (501) staff       (20)      512 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
--rw-rw-r--   0 em         (501) staff       (20)      481 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
--rw-rw-r--   0 em         (501) staff       (20)      419 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/cli_input.py
--rw-rw-r--   0 em         (501) staff       (20)     1939 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
--rw-rw-r--   0 em         (501) staff       (20)      884 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-rw-r--   0 em         (501) staff       (20)     3069 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/display_output.py
--rw-rw-r--   0 em         (501) staff       (20)      459 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
--rw-rw-r--   0 em         (501) staff       (20)      250 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
--rw-rw-r--   0 em         (501) staff       (20)      184 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-rw-r--   0 em         (501) staff       (20)      316 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
--rw-rw-r--   0 em         (501) staff       (20)       79 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
--rw-rw-r--   0 em         (501) staff       (20)     2881 2024-04-10 12:14:24.000000 blackboxai-3.1/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.731803 blackboxai-3.1/blackboxai.egg-info/
--rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 03:08:08.000000 blackboxai-3.1/blackboxai.egg-info/PKG-INFO
--rw-r--r--   0 em         (501) staff       (20)     6685 2024-05-26 03:08:08.000000 blackboxai-3.1/blackboxai.egg-info/SOURCES.txt
--rw-r--r--   0 em         (501) staff       (20)        1 2024-05-26 03:08:08.000000 blackboxai-3.1/blackboxai.egg-info/dependency_links.txt
--rw-r--r--   0 em         (501) staff       (20)       50 2024-05-26 03:08:08.000000 blackboxai-3.1/blackboxai.egg-info/entry_points.txt
--rw-r--r--   0 em         (501) staff       (20)       11 2024-05-26 03:08:08.000000 blackboxai-3.1/blackboxai.egg-info/top_level.txt
--rw-r--r--   0 em         (501) staff       (20)     1959 2024-05-19 20:24:51.000000 blackboxai-3.1/pyproject.toml
--rw-r--r--   0 em         (501) staff       (20)       38 2024-05-26 03:08:08.732377 blackboxai-3.1/setup.cfg
--rw-r--r--   0 em         (501) staff       (20)      523 2024-05-26 03:07:55.000000 blackboxai-3.1/setup.py
-drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:08:08.731354 blackboxai-3.1/tests/
--rw-r--r--   0 em         (501) staff       (20)    21812 2024-05-18 20:28:33.000000 blackboxai-3.1/tests/test_interpreter.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.749520 blackboxai-3.2/
+-rw-rw-r--   0 em         (501) staff       (20)    33813 2024-05-10 07:30:29.000000 blackboxai-3.2/LICENSE
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 03:49:54.749272 blackboxai-3.2/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)      635 2024-05-19 15:41:33.000000 blackboxai-3.2/README.md
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.731119 blackboxai-3.2/blackboxai/
+-rw-r--r--   0 em         (501) staff       (20)       25 2024-05-18 20:28:33.000000 blackboxai-3.2/blackboxai/__init__.py
+-rw-r--r--   0 em         (501) staff       (20)     2718 2024-05-19 20:10:15.000000 blackboxai-3.2/blackboxai/chat.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.731465 blackboxai-3.2/blackboxai/interpreter/
+-rw-rw-r--   0 em         (501) staff       (20)      633 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.733136 blackboxai-3.2/blackboxai/interpreter/core/
+-rw-rw-r--   0 em         (501) staff       (20)     2820 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.733591 blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/
+-rw-rw-r--   0 em         (501) staff       (20)     1293 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     3138 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.733795 blackboxai-3.2/blackboxai/interpreter/core/computer/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.734034 blackboxai-3.2/blackboxai/interpreter/core/computer/ai/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/ai/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     5688 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.734265 blackboxai-3.2/blackboxai/interpreter/core/computer/browser/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/browser/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      416 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.734514 blackboxai-3.2/blackboxai/interpreter/core/computer/calendar/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/calendar/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12950 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/calendar/calendar.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.734787 blackboxai-3.2/blackboxai/interpreter/core/computer/clipboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/clipboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      879 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/clipboard/clipboard.py
+-rw-rw-r--   0 em         (501) staff       (20)     2831 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/computer.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.735028 blackboxai-3.2/blackboxai/interpreter/core/computer/contacts/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/contacts/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3293 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/contacts/contacts.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.735265 blackboxai-3.2/blackboxai/interpreter/core/computer/display/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/display/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    10556 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.735498 blackboxai-3.2/blackboxai/interpreter/core/computer/docs/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/docs/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      749 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.735721 blackboxai-3.2/blackboxai/interpreter/core/computer/files/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/files/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1698 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.735969 blackboxai-3.2/blackboxai/interpreter/core/computer/keyboard/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/keyboard/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     3553 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.736204 blackboxai-3.2/blackboxai/interpreter/core/computer/mail/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/mail/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     6350 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/mail/mail.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.736456 blackboxai-3.2/blackboxai/interpreter/core/computer/mouse/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/mouse/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)    12423 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.736681 blackboxai-3.2/blackboxai/interpreter/core/computer/os/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/os/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     2955 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.736997 blackboxai-3.2/blackboxai/interpreter/core/computer/skills/
+-rw-rw-r--   0 em         (501) staff       (20)     4535 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.737455 blackboxai-3.2/blackboxai/interpreter/core/computer/sms/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/sms/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1399 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/sms/sms.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.737930 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1090 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.739740 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/
+-rw-rw-r--   0 em         (501) staff       (20)     5164 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     1812 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)      858 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/html.py
+-rw-rw-r--   0 em         (501) staff       (20)     1924 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
+-rw-rw-r--   0 em         (501) staff       (20)    15287 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     2193 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
+-rw-rw-r--   0 em         (501) staff       (20)      293 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/python.py
+-rw-rw-r--   0 em         (501) staff       (20)     2360 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/r.py
+-rw-rw-r--   0 em         (501) staff       (20)     2503 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/react.py
+-rw-rw-r--   0 em         (501) staff       (20)     2727 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/shell.py
+-rw-rw-r--   0 em         (501) staff       (20)     6715 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-rw-r--   0 em         (501) staff       (20)     4946 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.740358 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/
+-rw-rw-r--   0 em         (501) staff       (20)     7097 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/computer_vision.py
+-rw-rw-r--   0 em         (501) staff       (20)     1479 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/get_active_window.py
+-rw-rw-r--   0 em         (501) staff       (20)      929 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-rw-r--   0 em         (501) staff       (20)      396 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/recipient_utils.py
+-rw-rw-r--   0 em         (501) staff       (20)      586 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/computer/utils/run_applescript.py
+-rw-rw-r--   0 em         (501) staff       (20)    14297 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/core.py
+-rw-rw-r--   0 em         (501) staff       (20)     3282 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/default_system_message.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.741660 blackboxai-3.2/blackboxai/interpreter/core/llm/
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)     8752 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     5052 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/run_function_calling_llm.py
+-rw-rw-r--   0 em         (501) staff       (20)     2616 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.742162 blackboxai-3.2/blackboxai/interpreter/core/llm/utils/
+-rw-rw-r--   0 em         (501) staff       (20)     9479 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-rw-r--   0 em         (501) staff       (20)      711 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/utils/merge_deltas.py
+-rw-rw-r--   0 em         (501) staff       (20)     1800 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
+-rw-rw-r--   0 em         (501) staff       (20)      538 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/llm/vision_for_text_llms.py
+-rw-rw-r--   0 em         (501) staff       (20)     1688 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/render_message.py
+-rw-rw-r--   0 em         (501) staff       (20)    13491 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/respond.py
+-rw-rw-r--   0 em         (501) staff       (20)     6162 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/server.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.743381 blackboxai-3.2/blackboxai/interpreter/core/utils/
+-rw-rw-r--   0 em         (501) staff       (20)      630 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
+-rw-rw-r--   0 em         (501) staff       (20)      360 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-rw-r--   0 em         (501) staff       (20)     1096 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/__init__.py
+-rw-rw-r--   0 em         (501) staff       (20)      920 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/lazy_import.py
+-rw-rw-r--   0 em         (501) staff       (20)     2118 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/scan_code.py
+-rw-rw-r--   0 em         (501) staff       (20)     4404 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/system_debug_info.py
+-rw-rw-r--   0 em         (501) staff       (20)     1736 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/telemetry.py
+-rw-rw-r--   0 em         (501) staff       (20)     1098 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/temporary_file.py
+-rw-rw-r--   0 em         (501) staff       (20)      510 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.744889 blackboxai-3.2/blackboxai/interpreter/terminal_interface/
+-rw-rw-r--   0 em         (501) staff       (20)     2421 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)        0 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.745284 blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/
+-rw-rw-r--   0 em         (501) staff       (20)      611 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/base_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2664 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/code_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     1386 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/message_block.py
+-rw-rw-r--   0 em         (501) staff       (20)     2905 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/conversation_navigator.py
+-rw-rw-r--   0 em         (501) staff       (20)    10580 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/magic_commands.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.745534 blackboxai-3.2/blackboxai/interpreter/terminal_interface/profiles/
+-rw-rw-r--   0 em         (501) staff       (20)       25 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)    40437 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/profiles/profiles.py
+-rw-rw-r--   0 em         (501) staff       (20)     2304 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/render_past_conversation.py
+-rw-rw-r--   0 em         (501) staff       (20)    14875 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
+-rw-rw-r--   0 em         (501) staff       (20)    20287 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.747526 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/
+-rw-rw-r--   0 em         (501) staff       (20)    25763 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-rw-r--   0 em         (501) staff       (20)     3099 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-rw-r--   0 em         (501) staff       (20)      512 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
+-rw-rw-r--   0 em         (501) staff       (20)      481 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
+-rw-rw-r--   0 em         (501) staff       (20)      419 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/cli_input.py
+-rw-rw-r--   0 em         (501) staff       (20)     1939 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
+-rw-rw-r--   0 em         (501) staff       (20)      884 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-rw-r--   0 em         (501) staff       (20)     3069 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/display_output.py
+-rw-rw-r--   0 em         (501) staff       (20)      459 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
+-rw-rw-r--   0 em         (501) staff       (20)      250 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
+-rw-rw-r--   0 em         (501) staff       (20)      184 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-rw-r--   0 em         (501) staff       (20)      316 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-rw-r--   0 em         (501) staff       (20)       79 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
+-rw-rw-r--   0 em         (501) staff       (20)     2881 2024-04-10 12:14:24.000000 blackboxai-3.2/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.749005 blackboxai-3.2/blackboxai.egg-info/
+-rw-r--r--   0 em         (501) staff       (20)      750 2024-05-26 03:49:54.000000 blackboxai-3.2/blackboxai.egg-info/PKG-INFO
+-rw-r--r--   0 em         (501) staff       (20)     6685 2024-05-26 03:49:54.000000 blackboxai-3.2/blackboxai.egg-info/SOURCES.txt
+-rw-r--r--   0 em         (501) staff       (20)        1 2024-05-26 03:49:54.000000 blackboxai-3.2/blackboxai.egg-info/dependency_links.txt
+-rw-r--r--   0 em         (501) staff       (20)       50 2024-05-26 03:49:54.000000 blackboxai-3.2/blackboxai.egg-info/entry_points.txt
+-rw-r--r--   0 em         (501) staff       (20)       11 2024-05-26 03:49:54.000000 blackboxai-3.2/blackboxai.egg-info/top_level.txt
+-rw-r--r--   0 em         (501) staff       (20)     1959 2024-05-19 20:24:51.000000 blackboxai-3.2/pyproject.toml
+-rw-r--r--   0 em         (501) staff       (20)       38 2024-05-26 03:49:54.749604 blackboxai-3.2/setup.cfg
+-rw-r--r--   0 em         (501) staff       (20)      523 2024-05-26 03:49:35.000000 blackboxai-3.2/setup.py
+drwxr-xr-x   0 em         (501) staff       (20)        0 2024-05-26 03:49:54.748260 blackboxai-3.2/tests/
+-rw-r--r--   0 em         (501) staff       (20)    21812 2024-05-18 20:28:33.000000 blackboxai-3.2/tests/test_interpreter.py
```

### Comparing `blackboxai-3.1/LICENSE` & `blackboxai-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/PKG-INFO` & `blackboxai-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 3.1
+Version: 3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
```

### Comparing `blackboxai-3.1/README.md` & `blackboxai-3.2/README.md`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/chat.py` & `blackboxai-3.2/blackboxai/chat.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/__init__.py` & `blackboxai-3.2/blackboxai/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-3.2/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/ai/ai.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/calendar/calendar.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/computer.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/computer.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/contacts/contacts.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/contacts/contacts.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/display/display.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/display/display.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/docs/docs.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/files/files.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/mail/mail.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/mail/mail.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/mouse/mouse.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/os/os.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/skills/skills.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/skills/skills.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/sms/sms.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/sms/sms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/base_language.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/terminal/terminal.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/computer/utils/run_applescript.py` & `blackboxai-3.2/blackboxai/interpreter/core/computer/utils/run_applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/core.py` & `blackboxai-3.2/blackboxai/interpreter/core/core.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/default_system_message.py` & `blackboxai-3.2/blackboxai/interpreter/core/default_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/llm.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/run_text_llm.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/run_text_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-3.2/blackboxai/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/render_message.py` & `blackboxai-3.2/blackboxai/interpreter/core/render_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/respond.py` & `blackboxai-3.2/blackboxai/interpreter/core/respond.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/server.py` & `blackboxai-3.2/blackboxai/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/lazy_import.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/scan_code.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/system_debug_info.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/telemetry.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/core/utils/temporary_file.py` & `blackboxai-3.2/blackboxai/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/base_block.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/code_block.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/components/message_block.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/magic_commands.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/profiles/profiles.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-3.2/blackboxai/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/blackboxai.egg-info/PKG-INFO` & `blackboxai-3.2/blackboxai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 3.1
+Version: 3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
 
 ### Step1: Install
 ```shell
```

### Comparing `blackboxai-3.1/blackboxai.egg-info/SOURCES.txt` & `blackboxai-3.2/blackboxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/pyproject.toml` & `blackboxai-3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboxai-3.1/setup.py` & `blackboxai-3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="blackboxai",
-    version="3.1",
+    version="3.2",
     packages=find_packages(),
     package_dir = {'': '.'},
     include_package_data=True,
     setup_requires= ['requests'],
     entry_points={
         "console_scripts": [
             "blackboxai = blackboxai:runChat"
```

### Comparing `blackboxai-3.1/tests/test_interpreter.py` & `blackboxai-3.2/tests/test_interpreter.py`

 * *Files identical despite different names*

