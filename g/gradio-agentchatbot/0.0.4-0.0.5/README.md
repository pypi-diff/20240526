# Comparing `tmp/gradio_agentchatbot-0.0.4.tar.gz` & `tmp/gradio_agentchatbot-0.0.5.tar.gz`

## Comparing `gradio_agentchatbot-0.0.4.tar` & `gradio_agentchatbot-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/__init__.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.py
--rw-r--r--   0        0        0    17172 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.pyi
--rw-r--r--   0        0        0    33305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/chat_interface.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/utils.py
--rw-r--r--   0        0        0   775853 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/index.js
--rw-r--r--   0        0        0  1484417 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/style.css
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/app.py
--rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/docs.md
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_agent_demo.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_chatinterface.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/hf_stream_demo.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/langchain_agent_demo.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/open_ai_function_calling_demo.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/openai_stream_demo.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/requirements.txt
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/demo/templates/index.html
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/Index.svelte
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/gradio.config.js
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/main.ts
--rw-r--r--   0        0        0   208073 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/package-lock.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/package.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/types.ts
--rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ChatBot.svelte
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Copy.svelte
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ErrorMessage.svelte
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/LikeDislike.svelte
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Pending.svelte
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/Tool.svelte
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/ToolMessage.svelte
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/autorender.d.ts
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/frontend/shared/utils.ts
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/LICENSE
--rw-r--r--   0        0        0    14674 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    15764 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/agentchatbot.py
+-rw-r--r--   0        0        0    17172 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/agentchatbot.pyi
+-rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/chat_interface.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/utils.py
+-rw-r--r--   0        0        0   775853 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/index.js
+-rw-r--r--   0        0        0  1484417 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/style.css
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/app.py
+-rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/docs.md
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/hf_agent_demo.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/hf_chatinterface.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/hf_stream_demo.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/langchain_agent_demo.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/open_ai_function_calling_demo.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/openai_stream_demo.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/requirements.txt
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/transformers_local.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/demo/templates/index.html
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/Index.svelte
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/gradio.config.js
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/main.ts
+-rw-r--r--   0        0        0   208073 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/package-lock.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/types.ts
+-rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/ChatBot.svelte
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/Copy.svelte
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/ErrorMessage.svelte
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/LikeDislike.svelte
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/Pending.svelte
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/Tool.svelte
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/ToolMessage.svelte
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/autorender.d.ts
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/LICENSE
+-rw-r--r--   0        0        0    14674 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    15764 2020-02-02 00:00:00.000000 gradio_agentchatbot-0.0.5/PKG-INFO
```

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.py` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/agentchatbot.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/agentchatbot.pyi` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/agentchatbot.pyi`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/chat_interface.py` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/chat_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,14 @@
             new_response = response.model_dump()
         elif isinstance(response, str):
             assert current_response is not None and isinstance(
                 current_response["content"], str
             )
             current_response["content"] += response
             new_response = current_response
-            print("new_response", new_response)
         else:
             new_response = response
         return cast(MessageDict, new_response)
 
     async def _submit_fn(
         self,
         message: str | MultimodalData,
@@ -644,15 +643,14 @@
             else:
                 update = history + [{"role": "user", "content": message}]
                 yield update, update
         async for response in generator:
             new_response = self.response_as_dict(
                 response, current_response=current_response
             )
-            print("NEW RESPONSE", new_response)
             if self.multimodal and isinstance(message, MultimodalData):
                 update = history + [
                     {"role": "user", "content": message.text},
                     new_response,
                 ]
                 yield update, update
             else:
@@ -678,34 +676,34 @@
 
     async def _api_stream_fn(
         self, message: str, history: list[list[str | None]], request: Request, *args
     ) -> AsyncGenerator:
         inputs, _, _ = special_args(
             self.fn, inputs=[message, history, *args], request=request
         )
-
+        current_response = {"role": "assistant", "content": ""}
         if self.is_async:
             generator = self.fn(*inputs)
         else:
             generator = await anyio.to_thread.run_sync(
                 self.fn, *inputs, limiter=self.limiter
             )
             generator = SyncToAsyncIterator(generator, self.limiter)
         try:
-            first_response = self.response_as_dict(await async_iteration(generator))
+            first_response = self.response_as_dict(await async_iteration(generator), current_response=current_response)
             yield (
                 first_response,
                 history + [{"role": "user", "content": message}, first_response],
             )
         except StopIteration:
             yield None, history + [[message, None]]
         async for response in generator:
-            new_response = self.response_as_dict(response)
+            new_response = self.response_as_dict(response, current_response=current_response)
             yield (
-                response,
+                new_response,
                 history
                 + history
                 + [{"role": "user", "content": message}, new_response],
             )
 
     async def _examples_fn(self, message: str, *args) -> list[list[str | None]]:
         inputs, _, _ = special_args(self.fn, inputs=[message, [], *args], request=None)
@@ -748,9 +746,9 @@
             remove_input = (
                 len(message.files) + 1
                 if message.text is not None
                 else len(message.files)
             )
             history = history[:-remove_input]
         else:
-            history = history[:-1]
+            history = history[:-2]
         return history, message or "", history
```

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/utils.py` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/index.js` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/style.css` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js` & `gradio_agentchatbot-0.0.5/backend/gradio_agentchatbot/templates/component/assets/worker-lPYB70QI.js`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/docs.md` & `gradio_agentchatbot-0.0.5/demo/docs.md`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/hf_agent_demo.py` & `gradio_agentchatbot-0.0.5/demo/hf_agent_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from transformers import load_tool, ReactCodeAgent, HfEngine, Tool
 from gradio_agentchatbot import (
     AgentChatbot,
     stream_from_transformers_agent,
     Message,
 )
 from dotenv import load_dotenv
-from langchain.agents import load_tools
+from langchain_community.tools.tavily_search import TavilySearchResults
 from pathlib import Path
 
 current_dir = Path(__file__).parent
 
 load_dotenv()
 
 image_generation_tool = load_tool("m-ric/text-to-image")
 
-search_tool = Tool.from_langchain(load_tools(["serpapi"])[0])
+search_tool = TavilySearchResults()
 
 llm_engine = HfEngine("meta-llama/Meta-Llama-3-70B-Instruct")
 # Initialize the agent with both tools
 agent = ReactCodeAgent(
     tools=[image_generation_tool, search_tool], llm_engine=llm_engine
 )
```

### Comparing `gradio_agentchatbot-0.0.4/demo/hf_chatinterface.py` & `gradio_agentchatbot-0.0.5/demo/hf_chatinterface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from huggingface_hub import InferenceClient
-from gradio_agentchatbot import ChatInterface
+from gradio_agentchatbot import ChatInterface, AgentChatbot
 import gradio as gr
 
 client = InferenceClient("HuggingFaceH4/zephyr-7b-beta")
 
 
 def respond(
     message,
@@ -18,14 +18,15 @@
         stream=True,
     ):
         yield chunk.choices[0].delta.content
 
 
 chat = ChatInterface(
     respond,
+    chatbot=AgentChatbot(height=500),
     additional_inputs=[
         gr.Textbox(value="You are a friendly Chatbot.", label="System message"),
     ],
 )
 
 with gr.Blocks() as demo:
     gr.Markdown("# ChatInterface with Hugging Face Zephyr 7b 🤗")
```

### Comparing `gradio_agentchatbot-0.0.4/demo/hf_stream_demo.py` & `gradio_agentchatbot-0.0.5/demo/hf_stream_demo.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/langchain_agent_demo.py` & `gradio_agentchatbot-0.0.5/demo/langchain_agent_demo.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/open_ai_function_calling_demo.py` & `gradio_agentchatbot-0.0.5/demo/open_ai_function_calling_demo.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/openai_stream_demo.py` & `gradio_agentchatbot-0.0.5/demo/openai_stream_demo.py`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/demo/templates/index.html` & `gradio_agentchatbot-0.0.5/demo/templates/index.html`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/Index.svelte` & `gradio_agentchatbot-0.0.5/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/package-lock.json` & `gradio_agentchatbot-0.0.5/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/package.json` & `gradio_agentchatbot-0.0.5/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/ChatBot.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/ChatBot.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/Copy.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/Copy.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/ErrorMessage.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/ErrorMessage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/LikeDislike.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/LikeDislike.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/Pending.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/Pending.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/Tool.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/Tool.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/ToolMessage.svelte` & `gradio_agentchatbot-0.0.5/frontend/shared/ToolMessage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/frontend/shared/utils.ts` & `gradio_agentchatbot-0.0.5/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/LICENSE` & `gradio_agentchatbot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/README.md` & `gradio_agentchatbot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gradio_agentchatbot-0.0.4/pyproject.toml` & `gradio_agentchatbot-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_agentchatbot"
-version = "0.0.4"
+version = "0.0.5"
 description = "Chat with agents 🤖 and see the tools they use 🛠️"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Chatbot", "chatbot", "agents", "streaming", "tools"]
 # Add dependencies here
```

### Comparing `gradio_agentchatbot-0.0.4/PKG-INFO` & `gradio_agentchatbot-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_agentchatbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Chat with agents 🤖 and see the tools they use 🛠️
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: agents,chatbot,gradio-custom-component,gradio-template-Chatbot,streaming,tools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

