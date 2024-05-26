# Comparing `tmp/ollama_chat-0.9.4.tar.gz` & `tmp/ollama_chat-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_chat-0.9.4.tar", last modified: Fri May 24 18:45:04 2024, max compression
+gzip compressed data, was "ollama_chat-0.9.5.tar", last modified: Sun May 26 20:11:52 2024, max compression
```

## Comparing `ollama_chat-0.9.4.tar` & `ollama_chat-0.9.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 18:45:04.006984 ollama_chat-0.9.4/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.4/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     3373 2024-05-24 18:45:04.006922 ollama_chat-0.9.4/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     2515 2024-05-24 18:42:15.000000 ollama_chat-0.9.4/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.4/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1039 2024-05-24 18:45:04.007242 ollama_chat-0.9.4/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 18:45:04.003804 ollama_chat-0.9.4/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 18:45:04.005271 ollama_chat-0.9.4/src/ollama_chat/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.4/src/ollama_chat/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.4/src/ollama_chat/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9562 2024-05-24 18:16:51.000000 ollama_chat-0.9.4/src/ollama_chat/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2900 2024-05-24 18:33:46.000000 ollama_chat-0.9.4/src/ollama_chat/main.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2659 2024-05-22 20:43:32.000000 ollama_chat-0.9.4/src/ollama_chat/ollama.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 18:45:04.006456 ollama_chat-0.9.4/src/ollama_chat/static/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.4/src/ollama_chat/static/index.html
--rw-r--r--   0 craighobbs   (501) staff       (20)    17665 2024-05-24 18:38:01.000000 ollama_chat-0.9.4/src/ollama_chat/static/ollamaChat.bare
--rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.4/src/ollama_chat/static/ollamaChat.smd
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 18:45:04.006622 ollama_chat-0.9.4/src/ollama_chat.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3373 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      518 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-24 18:45:03.000000 ollama_chat-0.9.4/src/ollama_chat.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:11:52.461179 ollama_chat-0.9.5/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.5/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3375 2024-05-26 20:11:52.461118 ollama_chat-0.9.5/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2517 2024-05-26 18:14:23.000000 ollama_chat-0.9.5/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.5/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1039 2024-05-26 20:11:52.461435 ollama_chat-0.9.5/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:11:52.458138 ollama_chat-0.9.5/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:11:52.459144 ollama_chat-0.9.5/src/ollama_chat/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.5/src/ollama_chat/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.5/src/ollama_chat/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    12030 2024-05-24 19:11:33.000000 ollama_chat-0.9.5/src/ollama_chat/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3113 2024-05-26 18:10:53.000000 ollama_chat-0.9.5/src/ollama_chat/main.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:11:52.460692 ollama_chat-0.9.5/src/ollama_chat/static/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.5/src/ollama_chat/static/index.html
+-rw-r--r--   0 craighobbs   (501) staff       (20)    17665 2024-05-24 18:38:01.000000 ollama_chat-0.9.5/src/ollama_chat/static/ollamaChat.bare
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.5/src/ollama_chat/static/ollamaChat.smd
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-26 20:11:52.460865 ollama_chat-0.9.5/src/ollama_chat.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3375 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      492 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-26 20:11:52.000000 ollama_chat-0.9.5/src/ollama_chat.egg-info/top_level.txt
```

### Comparing `ollama_chat-0.9.4/LICENSE` & `ollama_chat-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.4/PKG-INFO` & `ollama_chat-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.4
+Version: 0.9.5
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,40 +64,41 @@
 
 ~~~
 ollama-chat
 ~~~
 
 A web browser is launched and opens the Ollama Chat web application.
 
-By default, a configuration file, "ollama-chat.json", is created in the current directory to save
-your conversations.
+By default, a configuration file, "ollama-chat.json", is created in the user's home directory.
 
 
 ## Start Conversation from CLI
 
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
 ## Future
 
-- Prompts part 1
-  - Prompts config collection (name, title, prompt)
-  - Index links start new conversation with current model
-  - `-p` command-line argument starts prompt by name
+- Multi-line text input
+
+- Save conversation as Markdown file
+  - Save link on index/conversation page
 
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
-- Save conversation as Markdown file
-  - Save link on index/conversation page
+- Prompts part 1
+  - Prompts config collection (name, title, prompt)
+  - Index links start new conversation with current model
+  - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
```

### Comparing `ollama_chat-0.9.4/README.md` & `ollama_chat-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,40 +39,41 @@
 
 ~~~
 ollama-chat
 ~~~
 
 A web browser is launched and opens the Ollama Chat web application.
 
-By default, a configuration file, "ollama-chat.json", is created in the current directory to save
-your conversations.
+By default, a configuration file, "ollama-chat.json", is created in the user's home directory.
 
 
 ## Start Conversation from CLI
 
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
 ## Future
 
-- Prompts part 1
-  - Prompts config collection (name, title, prompt)
-  - Index links start new conversation with current model
-  - `-p` command-line argument starts prompt by name
+- Multi-line text input
+
+- Save conversation as Markdown file
+  - Save link on index/conversation page
 
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
-- Save conversation as Markdown file
-  - Save link on index/conversation page
+- Prompts part 1
+  - Prompts config collection (name, title, prompt)
+  - Index links start new conversation with current model
+  - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
```

### Comparing `ollama_chat-0.9.4/setup.cfg` & `ollama_chat-0.9.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ollama-chat
-version = 0.9.4
+version = 0.9.5
 url = https://github.com/craigahobbs/ollama-chat
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = ollama-chat
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `ollama_chat-0.9.4/src/ollama_chat/app.py` & `ollama_chat-0.9.5/src/ollama_chat/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,17 @@
 import threading
 import uuid
 
 import chisel
 import ollama
 import schema_markdown
 
-from .ollama import OllamaChat, config_conversation
-
 
+# The ollama-chat back-end API WSGI application class
 class OllamaChatApplication(chisel.Application):
-    """
-    The ollama-chat back-end API WSGI application class
-    """
-
     __slots__ = ('config', 'chats')
 
 
     def __init__(self, config_path):
         super().__init__()
         self.config = ConfigManager(config_path)
         self.chats = {}
@@ -72,14 +67,15 @@
                 content_type=content_type,
                 urls=urls,
                 doc=doc,
                 doc_group='Ollama Chat Statics'
             ))
 
 
+# The ollama-chat configuration context manager
 class ConfigManager:
     __slots__ = ('config_path', 'config_lock', 'config')
 
 
     DEFAULT_MODEL = 'llama3:latest'
 
 
@@ -115,15 +111,84 @@
                 with open(self.config_path, 'w', encoding='utf-8') as fh_config:
                     json.dump(self.config, fh_config, indent=4, sort_keys = True)
         finally:
             # Release the config lock
             self.config_lock.release()
 
 
-# The Ollama Chat type model
+# The ollama chat manager class
+class OllamaChat():
+    __slots__ = ('app', 'conversation_id', 'stop')
+
+
+    def __init__(self, app, conversation_id):
+        self.app = app
+        self.conversation_id = conversation_id
+        self.stop = False
+
+        # Start the chat thread
+        chat_thread = threading.Thread(target=OllamaChat.chat_thread_fn, args=(self,))
+        chat_thread.daemon = True
+        chat_thread.start()
+
+
+    @staticmethod
+    def chat_thread_fn(chat):
+        try:
+            # Create the Ollama messages from the conversation
+            messages = []
+            with chat.app.config() as config:
+                conversation = config_conversation(config, chat.conversation_id)
+                model = conversation['model']
+                for exchange in conversation['exchanges']:
+                    messages.append({'role': 'user', 'content': exchange['user']})
+                    if exchange['model'] != '':
+                        messages.append({'role': 'assistant', 'content': exchange['model']})
+
+            # Start the chat
+            stream = ollama.chat(model=model, messages=messages, stream=True)
+
+            # Stream the chat response
+            for chunk in stream:
+                # If stopped, return immediately. The chat is deleted by the stopper.
+                if chat.stop:
+                    stream.close()
+                    break
+
+                # Update the conversation
+                with chat.app.config() as config:
+                    conversation = config_conversation(config, chat.conversation_id)
+                    exchange = conversation['exchanges'][-1]
+                    exchange['model'] += chunk['message']['content']
+
+        except Exception as exc: # pylint: disable=broad-exception-caught
+            # Communicate the error
+            with chat.app.config() as config:
+                conversation = config_conversation(config, chat.conversation_id)
+                exchange = conversation['exchanges'][-1]
+                exchange['model'] += f'\n**ERROR:** {exc}'
+
+        # Save the conversation
+        with chat.app.config(save=True):
+            # Delete the application's chat entry
+            if chat.conversation_id in chat.app.chats:
+                del chat.app.chats[chat.conversation_id]
+
+
+# Helper to find a conversation by ID
+def config_conversation(config, id_):
+    return next((conv for conv in config['conversations'] if conv['id'] == id_), None)
+
+
+#
+# The Ollama Chat API
+#
+
+
+# The Ollama Chat API type model
 with pkg_resources.open_text('ollama_chat.static', 'ollamaChat.smd') as cm_smd:
     OLLAMA_CHAT_TYPES = schema_markdown.parse_schema_markdown(cm_smd.read())
 
 
 @chisel.action(name='getModels', types=OLLAMA_CHAT_TYPES)
 def get_models(unused_ctx, unused_req):
     return {
```

### Comparing `ollama_chat-0.9.4/src/ollama_chat/main.py` & `ollama_chat-0.9.5/src/ollama_chat/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,21 +55,25 @@
     # Launch the web browser on a thread so the WSGI application can startup first
     if not args.no_browser:
         webbrowser_thread = threading.Thread(target=webbrowser.open, args=(url,))
         webbrowser_thread.daemon = True
         webbrowser_thread.start()
 
     # Determine the config path
-    if args.config is None:
-        args.config = os.getenv(CONFIG_ENVIRONMENT)
-        if args.config is None:
-            args.config = os.path.join(os.path.expanduser('~'), CONFIG_FILENAME)
+    config_path = args.config or os.getenv(CONFIG_ENVIRONMENT)
+    if config_path is None:
+        if os.path.isfile(CONFIG_FILENAME):
+            config_path = CONFIG_FILENAME
+        else:
+            config_path = os.path.join(os.path.expanduser('~'), CONFIG_FILENAME)
+    elif config_path.endswith(os.sep) or os.path.isdir(config_path):
+        config_path = os.path.join(config_path, CONFIG_FILENAME)
 
     # Create the WSGI application
-    wsgiapp = OllamaChatApplication(args.config)
+    wsgiapp = OllamaChatApplication(config_path)
 
     # Wrap the WSGI application and the start_response function so we can log status and environ
     def wsgiapp_wrap(environ, start_response):
         def log_start_response(status, response_headers):
             if not args.quiet:
                 print(f'ollama-chat: {status[0:3]} {environ["REQUEST_METHOD"]} {environ["PATH_INFO"]} {environ["QUERY_STRING"]}')
             return start_response(status, response_headers)
```

### Comparing `ollama_chat-0.9.4/src/ollama_chat/static/index.html` & `ollama_chat-0.9.5/src/ollama_chat/static/index.html`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.4/src/ollama_chat/static/ollamaChat.bare` & `ollama_chat-0.9.5/src/ollama_chat/static/ollamaChat.bare`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.4/src/ollama_chat/static/ollamaChat.smd` & `ollama_chat-0.9.5/src/ollama_chat/static/ollamaChat.smd`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.4/src/ollama_chat.egg-info/PKG-INFO` & `ollama_chat-0.9.5/src/ollama_chat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.4
+Version: 0.9.5
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,40 +64,41 @@
 
 ~~~
 ollama-chat
 ~~~
 
 A web browser is launched and opens the Ollama Chat web application.
 
-By default, a configuration file, "ollama-chat.json", is created in the current directory to save
-your conversations.
+By default, a configuration file, "ollama-chat.json", is created in the user's home directory.
 
 
 ## Start Conversation from CLI
 
 To start a conversation from the command line, use the `-m` argument:
 
 ~~~
 ollama-chat -m "Why is the sky blue?"
 ~~~
 
 
 ## Future
 
-- Prompts part 1
-  - Prompts config collection (name, title, prompt)
-  - Index links start new conversation with current model
-  - `-p` command-line argument starts prompt by name
+- Multi-line text input
+
+- Save conversation as Markdown file
+  - Save link on index/conversation page
 
 - Auto-title task on start conversation
   - Update conversation title API
   - Update title link on index/conversation page
 
-- Save conversation as Markdown file
-  - Save link on index/conversation page
+- Prompts part 1
+  - Prompts config collection (name, title, prompt)
+  - Index links start new conversation with current model
+  - `-t` command-line argument starts prompt by name
 
 - File / Directory / URL text inclusion in prompt
 
 - Prompts part 2
   - Prompt editor
   - Create link on index page
   - Delete links on index page
```

