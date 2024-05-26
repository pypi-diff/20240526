# Comparing `tmp/GPTPlugins4All-1.0.8.tar.gz` & `tmp/GPTPlugins4All-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTPlugins4All-1.0.8.tar", last modified: Fri Dec 29 00:27:56 2023, max compression
+gzip compressed data, was "GPTPlugins4All-1.0.9.tar", last modified: Sat Jan 13 02:15:29 2024, max compression
```

## Comparing `GPTPlugins4All-1.0.8.tar` & `GPTPlugins4All-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2023-12-29 00:27:56.075442 GPTPlugins4All-1.0.8/
-drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2023-12-29 00:27:56.071443 GPTPlugins4All-1.0.8/GPTPlugins4All/
--rw-rw-r--   0 trevor    (1001) trevor    (1001)        0 2023-11-18 23:59:58.000000 GPTPlugins4All-1.0.8/GPTPlugins4All/__init__.py
--rw-rw-r--   0 trevor    (1001) trevor    (1001)    12070 2023-12-28 19:25:37.000000 GPTPlugins4All-1.0.8/GPTPlugins4All/assistant.py
--rw-rw-r--   0 trevor    (1001) trevor    (1001)     2405 2023-12-15 19:13:43.000000 GPTPlugins4All-1.0.8/GPTPlugins4All/cli.py
--rw-rw-r--   0 trevor    (1001) trevor    (1001)    19062 2023-12-29 00:26:54.000000 GPTPlugins4All-1.0.8/GPTPlugins4All/config.py
-drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2023-12-29 00:27:56.075442 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/
--rw-r--r--   0 trevor    (1001) trevor    (1001)     5662 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/PKG-INFO
--rw-rw-r--   0 trevor    (1001) trevor    (1001)      358 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/SOURCES.txt
--rw-rw-r--   0 trevor    (1001) trevor    (1001)        1 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/dependency_links.txt
--rw-rw-r--   0 trevor    (1001) trevor    (1001)       61 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/entry_points.txt
--rw-rw-r--   0 trevor    (1001) trevor    (1001)       56 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/requires.txt
--rw-rw-r--   0 trevor    (1001) trevor    (1001)       15 2023-12-29 00:27:56.000000 GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/top_level.txt
--rw-rw-r--   0 trevor    (1001) trevor    (1001)     1080 2023-12-16 06:37:27.000000 GPTPlugins4All-1.0.8/LICENSE
--rw-r--r--   0 trevor    (1001) trevor    (1001)     5662 2023-12-29 00:27:56.075442 GPTPlugins4All-1.0.8/PKG-INFO
--rw-rw-r--   0 trevor    (1001) trevor    (1001)     4848 2023-12-16 06:25:40.000000 GPTPlugins4All-1.0.8/README.md
--rw-rw-r--   0 trevor    (1001) trevor    (1001)       38 2023-12-29 00:27:56.075442 GPTPlugins4All-1.0.8/setup.cfg
--rw-rw-r--   0 trevor    (1001) trevor    (1001)     1104 2023-12-29 00:27:38.000000 GPTPlugins4All-1.0.8/setup.py
+drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2024-01-13 02:15:29.091484 GPTPlugins4All-1.0.9/
+drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2024-01-13 02:15:29.091484 GPTPlugins4All-1.0.9/GPTPlugins4All/
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)        0 2023-11-18 23:59:58.000000 GPTPlugins4All-1.0.9/GPTPlugins4All/__init__.py
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)    14110 2024-01-13 01:38:58.000000 GPTPlugins4All-1.0.9/GPTPlugins4All/assistant.py
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)     2405 2023-12-15 19:13:43.000000 GPTPlugins4All-1.0.9/GPTPlugins4All/cli.py
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)    19062 2023-12-29 00:26:54.000000 GPTPlugins4All-1.0.9/GPTPlugins4All/config.py
+drwxrwxr-x   0 trevor    (1001) trevor    (1001)        0 2024-01-13 02:15:29.091484 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/
+-rw-r--r--   0 trevor    (1001) trevor    (1001)     5662 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/PKG-INFO
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)      358 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/SOURCES.txt
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)        1 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/dependency_links.txt
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)       61 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/entry_points.txt
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)       56 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/requires.txt
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)       15 2024-01-13 02:15:29.000000 GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/top_level.txt
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)     1080 2023-12-16 06:37:27.000000 GPTPlugins4All-1.0.9/LICENSE
+-rw-r--r--   0 trevor    (1001) trevor    (1001)     5662 2024-01-13 02:15:29.091484 GPTPlugins4All-1.0.9/PKG-INFO
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)     4848 2023-12-16 06:25:40.000000 GPTPlugins4All-1.0.9/README.md
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)       38 2024-01-13 02:15:29.091484 GPTPlugins4All-1.0.9/setup.cfg
+-rw-rw-r--   0 trevor    (1001) trevor    (1001)     1104 2024-01-13 02:15:21.000000 GPTPlugins4All-1.0.9/setup.py
```

### Comparing `GPTPlugins4All-1.0.8/GPTPlugins4All/assistant.py` & `GPTPlugins4All-1.0.9/GPTPlugins4All/assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,63 @@
 import os
 import time
 import json
 from dotenv import load_dotenv
 
 load_dotenv()
+from langchain.tools import tool
+from langchain.tools import BaseTool
+
+from langchain.pydantic_v1 import BaseModel, Field
+from typing import Optional
+from langchain.callbacks.manager import CallbackManagerForToolRun
+
+# Define the input schema for the API tool
+class APIToolInput(BaseModel):
+    operation_id: str = Field(description="Operation ID for the API call")
+    params: dict = Field(description="Parameters for the API call")
+    api_key: str = Field(description="API key for authentication")
+
+# Define the API tool
+class APITool(BaseTool):
+    name = "api_tool"
+    description = "Custom API tool for making external calls"
+    args_schema = APIToolInput
+
+    def _run(
+        self, 
+        operation_id: str, 
+        params: dict, 
+        api_key: str, 
+        run_manager: Optional[CallbackManagerForToolRun] = None
+    ) -> dict:
+        # Logic to make API call and process response
+        response = make_api_call(operation_id, params, api_key)  # Replace with actual function
+        return response
+
+# Function to make an API call (replace with your actual implementation)
+def make_api_call(operation_id: str, params: dict, api_key: str) -> dict:
+    # Implement the API call logic here
+    return {"response": "API response"}
 
 class Assistant:
-    def __init__(self, configs, name, instructions, model, assistant_id=None, thread_id=None, event_listener=None, openai_key=None, files=None,code_interpreter=False, retrieval=False, is_json=None):
+    class APIToolInput(BaseModel):
+        operation_id: str = Field(description="Operation ID for the API call")
+        params: dict = Field(description="Parameters for the API call")
+
+    class APITool(BaseTool):
+        name = "api_tool"
+        description = "Custom API tool for making external calls"
+        args_schema = APIToolInput
+
+        def _run(self, operation_id: str, params: dict, run_manager: Optional[CallbackManagerForToolRun] = None) -> dict:
+            # Use the existing execute_function method to make API calls
+            return self.execute_function(operation_id, json.dumps(params))
+
+    def __init__(self, configs, name, instructions, model, assistant_id=None, thread_id=None, event_listener=None, openai_key=None, files=None,code_interpreter=False, retrieval=False, is_json=None, old_mode=False):
         try:
             from openai import OpenAI
         except ImportError:
             OpenAI = None
 
         if OpenAI is None:
             raise ImportError("The OpenAI library is required to use this functionality. Please install it with `pip install GPTPlugins4All[openai]`.")
@@ -28,15 +75,21 @@
         self.thread_id = thread_id
         if is_json is not None:
             self.is_json = is_json
         if openai_key is None:
             self.openai_client = OpenAI()
         else:
             self.openai_client = OpenAI(api_key=openai_key)
-        self.assistant, self.thread = self.create_assistant_and_thread(files=files, code_interpreter=code_interpreter, retrieval=retrieval)
+        if old_mode:
+            self.assistant = None
+            self.thread = None
+            self.use_langchain = True
+            pass
+        else:
+            self.assistant, self.thread = self.create_assistant_and_thread(files=files, code_interpreter=code_interpreter, retrieval=retrieval)
 
     # Create an OpenAI assistant and a thread for interactions
     def create_assistant_and_thread(self, files=None, code_interpreter=False, retrieval=False):
         # Extract tools from the configs
         tools = []
         model_descriptions = []
         valid_descriptions = []
@@ -105,14 +158,15 @@
             self.assistant_id = assistant.id
             thread = self.openai_client.beta.threads.create()
             self.thread_id = thread.id
             #print("Thread ID: save this for persistence: "+thread.id)
 
         # Create a thread for the assistant
         return assistant, thread
+
     def modify_tools_for_config(self, config):
         if self.multiple_configs:
             modified_tools = []
             for tool in config.generate_tools_representation():
                 if self.multiple_configs:
                     tool['function']['name'] = config.name + '-' + tool['function']['name']
                 modified_tools.append(tool)
@@ -167,15 +221,15 @@
                         }
                         #print(output)
                         #put output to event listener if there is one
                         if self.event_listener is not None:
                             self.event_listener(output)
                         tool_outputs.append(output)
                 run__ = self.openai_client.beta.threads.runs.submit_tool_outputs(thread_id=self.thread.id, run_id=run.id, tool_outputs=tool_outputs)
-            time.sleep(5)
+            time.sleep(1)
         run_ = self.openai_client.beta.threads.runs.retrieve(thread_id=self.thread.id, run_id=run.id)
         messages = self.openai_client.beta.threads.messages.list(thread_id=self.thread.id)
         print(messages.data[0].content[0].text.value)
         return messages.data[0].content[0].text.value
     def get_entire_conversation(self):
         messages = self.openai_client.beta.threads.messages.list(thread_id=self.thread.id)
         return messages.data
```

### Comparing `GPTPlugins4All-1.0.8/GPTPlugins4All/cli.py` & `GPTPlugins4All-1.0.9/GPTPlugins4All/cli.py`

 * *Files identical despite different names*

### Comparing `GPTPlugins4All-1.0.8/GPTPlugins4All/config.py` & `GPTPlugins4All-1.0.9/GPTPlugins4All/config.py`

 * *Files identical despite different names*

### Comparing `GPTPlugins4All-1.0.8/GPTPlugins4All.egg-info/PKG-INFO` & `GPTPlugins4All-1.0.9/GPTPlugins4All.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTPlugins4All
-Version: 1.0.8
+Version: 1.0.9
 Summary: GPT Plugins for 4all
 Home-page: https://github.com/DataStreams-Solutions/GPTPlugins4All
 Author-email: trevor@gptplugins4all.com
 Project-URL: Bug Tracker, https://github.com/DataStreams-Solutions/GPTPlugins4All/issues
 Project-URL: Documentation, https://github.com/DataStreams-Solutions/GPTPlugins4All#readme
 Project-URL: Source Code, https://github.com/DataStreams-Solutions/GPTPlugins4All
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPTPlugins4All-1.0.8/LICENSE` & `GPTPlugins4All-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GPTPlugins4All-1.0.8/PKG-INFO` & `GPTPlugins4All-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTPlugins4All
-Version: 1.0.8
+Version: 1.0.9
 Summary: GPT Plugins for 4all
 Home-page: https://github.com/DataStreams-Solutions/GPTPlugins4All
 Author-email: trevor@gptplugins4all.com
 Project-URL: Bug Tracker, https://github.com/DataStreams-Solutions/GPTPlugins4All/issues
 Project-URL: Documentation, https://github.com/DataStreams-Solutions/GPTPlugins4All#readme
 Project-URL: Source Code, https://github.com/DataStreams-Solutions/GPTPlugins4All
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPTPlugins4All-1.0.8/README.md` & `GPTPlugins4All-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `GPTPlugins4All-1.0.8/setup.py` & `GPTPlugins4All-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GPTPlugins4All',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     description='GPT Plugins for 4all',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author_email='trevor@gptplugins4all.com',
     url='https://github.com/DataStreams-Solutions/GPTPlugins4All',
     project_urls={
```

