# Comparing `tmp/llm_axe-1.1.1.tar.gz` & `tmp/llm_axe-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-1.1.1.tar", last modified: Sun May 19 20:29:45 2024, max compression
+gzip compressed data, was "llm_axe-1.1.2.tar", last modified: Sun May 26 18:39:44 2024, max compression
```

## Comparing `llm_axe-1.1.1.tar` & `llm_axe-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.616440 llm_axe-1.1.1/
--rw-rw-rw-   0        0        0     3914 2024-05-19 20:29:45.615441 llm_axe-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.575940 llm_axe-1.1.1/llm_axe/
--rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.1.1/llm_axe/__init__.py
--rw-rw-rw-   0        0        0    27219 2024-05-19 20:27:16.000000 llm_axe-1.1.1/llm_axe/agents.py
--rw-rw-rw-   0        0        0     6486 2024-05-19 20:27:25.000000 llm_axe-1.1.1/llm_axe/core.py
--rw-rw-rw-   0        0        0      640 2024-05-18 05:10:13.000000 llm_axe-1.1.1/llm_axe/models.py
--rw-rw-rw-   0        0        0     9689 2024-05-19 15:56:00.000000 llm_axe-1.1.1/llm_axe/system_prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.614439 llm_axe-1.1.1/llm_axe.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 20:29:45.616440 llm_axe-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4619 2024-05-19 20:26:57.000000 llm_axe-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:44.475548 llm_axe-1.1.2/
+-rw-rw-rw-   0        0        0     3914 2024-05-26 18:39:44.475049 llm_axe-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:44.418547 llm_axe-1.1.2/llm_axe/
+-rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.1.2/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    27260 2024-05-26 18:23:40.000000 llm_axe-1.1.2/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     6798 2024-05-26 18:29:19.000000 llm_axe-1.1.2/llm_axe/core.py
+-rw-rw-rw-   0        0        0      927 2024-05-26 16:35:29.000000 llm_axe-1.1.2/llm_axe/models.py
+-rw-rw-rw-   0        0        0     9689 2024-05-19 15:56:00.000000 llm_axe-1.1.2/llm_axe/system_prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:44.474549 llm_axe-1.1.2/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-26 18:39:44.000000 llm_axe-1.1.2/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-26 18:39:44.000000 llm_axe-1.1.2/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:39:44.000000 llm_axe-1.1.2/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2024-05-26 18:39:44.000000 llm_axe-1.1.2/llm_axe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 18:39:44.000000 llm_axe-1.1.2/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:39:44.476046 llm_axe-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     4619 2024-05-26 18:39:33.000000 llm_axe-1.1.2/setup.py
```

### Comparing `llm_axe-1.1.1/PKG-INFO` & `llm_axe-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_axe
-Version: 1.1.1
+Version: 1.1.2
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.1.1/llm_axe/agents.py` & `llm_axe-1.1.2/llm_axe/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf, make_prompt, llm_has_ask
 
 
 class Agent:
     """
     Basic agent that can use premade or custom system prompts.
+    Custom system prompt will override any premade prompts.
     """
     def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None, format:str="", temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object with an ask function.
             agent_type (AgentType, optional): The type of agent to use. Choose from AgentType enum. Defaults to None.
             additional_system_instructions (str, optional): Additional system instructions to include in the premade system prompt. Defaults to "".
@@ -39,29 +40,31 @@
         Args:
             question (str): The question to get the prompt for.
         """
         user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
         return prompts
 
-    def ask(self, prompt, history:list=None):
+    def ask(self, prompt, images:list=None, history:list=None):
         """
-        Ask a question based on the given prompt.
+        Ask a question based on the given prompt or images.
+        Images require a multimodal LLM.
         Args:
-            prompt (str): The prompt to use for the question. Will only use system_prompt if prompt is None.
+            prompt (str): The prompt to use for the question.
+            images (list, optional): The images to include in the prompt. Each image must be a path to an image or base64 data. Defaults to None.
             history (list, optional): The history of the conversation. Defaults to None.
         """
         if llm_has_ask(self.llm) is False:
             return None
         
         prompts = [self.system_prompt]
         if history is not None:
             prompts.extend(history)
 
-        prompts.append(make_prompt("user", prompt))
+        prompts.append(make_prompt("user", prompt, images))
         response = self.llm.ask(prompts, temperature=self.temperature, format=self.format)
     
         self.chat_history.append(prompts[-1])
         self.chat_history.append(make_prompt("assistant", response))
         return response
 
 
@@ -90,34 +93,33 @@
         """
         Detects objects in an image.
         If given a list of objects, only the objects in the list will be detected.
         If a detection_criteria is given instead, it will detect according to the criteria's instructions. 
         Args:
             images (list): The images to detect objects in. List of string paths or byte data.
             objects (list, optional): An optional list of objects to detect. Defaults to None.
-            detection_criteria (str, optional): An opetional detection criteria to give.
+            detection_criteria (str, optional): An optional detection criteria to give.
         """
         if llm_has_ask(self.vision_llm) is False or llm_has_ask(self.text_llm) is False:
             return None
         
         prompts = make_prompt("user", "Detect all objects in this image", images=images)
         detected_objects = self.vision_llm.ask([self.__system_prompt, prompts], temperature=self.vision_temperature)
         prompts = self.__get_prompt(images, detected_objects, objects, detection_criteria)
         response = self.text_llm.ask(prompts, format="json", temperature=self.text_temperature)
 
         return response
         
-    def __get_prompt(self, images:list, detected_objects:list, objects:list=None, detection_criteria:str=None):
+    def __get_prompt(self, detected_objects:list, objects:list=None, detection_criteria:str=None):
         """
         Get the prompt for the given objects and detection_prompt.
         Args:
-            images (list): The images to detect objects in. List of string paths or byte data.
             detected_objects (list): The detected objects in the images.
             objects (list, optional): An optional list of objects to detect. Defaults to None.
-            detection_criteria (str, optional): An opetional detection criteria to give.
+            detection_criteria (str, optional): An optional detection criteria to give.
         """
         prompt = ""
         sys_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ObjectFilterer"))
 
         if objects is not None and detection_criteria is not None:
             raise ValueError("You cannot provide both an object list and a detection_prompt.")
         else:
@@ -131,15 +133,15 @@
             prompt = prompt + "\n Only return the objects that fit my interests"
             prompt = make_prompt("user", prompt)
             return [sys_prompt, prompt]
 
 
 class PythonAgent():
     """
-    A PytonAgent agent is used to solve problems by writing Python code.
+    A PythonAgent agent is used to solve problems by writing Python code.
     It will provide code to execute and the imports used in the code.
     IMPORTANT!!: Code should ALWAYS be executed in a virtual or isolated environment.
     """
     def __init__(self, llm:object, temperature:float=0.8):
         """
         Initializes a new PythonAgent object.
 
@@ -153,15 +155,15 @@
         self.library_extractor_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ImportExtractor"))
         self.temperature = temperature
 
     def ask(self, prompt, history:list=None):
         """
         Ask a question based on the given prompt.
         Args:
-            prompt (str): The prompt to use for the question. Will only use system_prompt if prompt is None.
+            prompt (str): The prompt to use for the question.
             history (list, optional): A list of previous chat messages in openai format. Defaults to None.
         Returns:
             dict: A dictionary containing the "code" and "imports" keys.
                 "code": The code to execute. In string format. WARNING!:CODE SHOULD NEVER BE EXECUTED OUTSIDE OF A VIRTUAL OR ISOLATED ENVIRONMENT.
                 "libraries": The imports used in the code. In json list format.
         """
         if llm_has_ask(self.llm) is False:
@@ -233,26 +235,27 @@
         return [self.system_prompt, make_prompt("user", prompt)]
     
     def ask(self, info:str, data_points:list=[]):
         """
         Ask a question based on the given content.
         Args:
             info (str): The content to extract information from.
-            data_points (list, optional): A string list of data points to extract. Defaults to None.
+            data_points (list, optional): A string list of data points to extract. 
+            Example: ["name", "age", "city"] Defaults to None.
         """
         prompts = self.get_prompt(info, data_points)
         resp = self.llm.ask(self.get_prompt(info, data_points), temperature=self.temperature)
         self.chat_history.append(prompts[1])
         self.chat_history.append(make_prompt("assistant", resp))
         return resp
     
 
 class PdfReader():
     """
-    A PdfReader agent is used to answer questions based on information from given PDF files.
+    An Agent used to answer questions based on information from given PDF files.
     """
 
     def __init__(self, llm:object, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):
         """
         Initializes a new PdfReader.
         Args:
             llm (object): An object that implements the ask() method.
@@ -294,15 +297,15 @@
         return response
     
     def get_prompt(self, question, pdf_files:list=None):
         """
         Generates the prompt for the LLM.
         args:
             question (str): The question to ask.
-            pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file. 
+            pdf_files (list): A list of PDF files to read. Each file should be a string path to the PDF file. 
         """
         pdf_text = ""
         for pdf_file in pdf_files:
             pdf_text += f"Contents of document {os.path.basename(pdf_file)} :\n"
             pdf_text += read_pdf(pdf_file) + "\n\n"
         
         if self.custom_system_prompt is None:
@@ -327,18 +330,18 @@
     """
 
     def __init__(self, llm:object, functions:list, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):            
         """
         Initializes a new Function Caller.
 
         Args:
-            llm (object, optional): An LLM object. Must have an ask method. Defaults to None.
-            functions (list, optional): A list of functions. Defaults to None.
-            additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
-            custom_system_prompt (str, optional): A custom system prompt. Will override the default. Defaults to None.
+            llm (object, optional): An LLM object. Must have an ask method.
+            functions (list, optional): A list of functions.
+            additional_system_instructions (str, optional): Instructions in addition to the default system prompt. Defaults to "".
+            custom_system_prompt (str, optional): A custom system prompt to override the default function picking prompt. Defaults to None.
             temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.chat_history = []
         self.llm = llm
         self.functions_dict = {func.__name__: func for func in functions}
         self.additional_instructions = additional_system_instructions
         self.schema = generate_schema(functions)
@@ -432,22 +435,21 @@
         user_prompt = make_prompt("user", question)
         prompts = [self.system_prompt, user_prompt]
         return prompts
 
 
 class WebsiteReaderAgent:
     """
-    An agent that can will read a website and answer questions based on it.
+    An agent that will read a specificwebsite and answer questions based on it.
     """
 
     def __init__(self, llm:object, additional_system_instructions:str="", custom_site_reader:callable=None, temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object. Must have an ask method.
-            url (str): The url of the website to read.
             additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
             custom_site_reader (function, optional): A custom online site reader function. The site reader function must take a URL and return a string representation of the site.
             temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.llm = llm
         self.chat_history = []
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "WebsiteReader")
```

### Comparing `llm_axe-1.1.1/llm_axe/core.py` & `llm_axe-1.1.2/llm_axe/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,21 @@
     PLANNER = "Planner"
     SUMMARIZER = "Summarizer"
     GENERIC_RESPONDER = "GenericResponder"
     VALIDATOR = "Validator"
 
 
 def llm_has_ask(llm):
+    """
+    Checks if the llm object has an ask function
+    Args:
+        llm (object): The object to check
+    Returns:
+        bool: True if the llm object has an ask function, False otherwise
+    """
     if not hasattr(llm, "ask"):
             warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
             return False
     return True
 
 
 def make_prompt(role:str, content:str, images:list=None):
@@ -105,17 +112,17 @@
         schema[func_name] = {'description': doc.short_description, 'parameters': params}
 
     return json.dumps(schema)
 
 
 def safe_read_json(response):
     """
-    Reads the response as json and checks if it is a valid json.
+    Reads the string as json and checks if it is a valid json.
     Args:
-        response (str): The response from the LLM.
+        response (str): The string response from the LLM.
     """
     response_json = None
     try:
             response_json = json.loads(response)
     except json.decoder.JSONDecodeError:
             try:
                 response_json = json.loads(clean_json_response(response))
@@ -125,15 +132,15 @@
     return response_json
 
 
 def clean_json_response(response):
     """
     Removes unnecessary characters from the json response.
     Args:
-        response (str): The response from the LLM.
+        response (str): The string response from the LLM.
     """
     brace_count = 0
     start = None
 
     for i, char in enumerate(response):
         if char == '{':
             if brace_count == 0:
@@ -146,15 +153,15 @@
                 return response[start:i+1]
     return ""
 
 
 def internet_search(query):
     """
     Searches the internet for a query.
-    Returns top 10 results.
+    Returns top 5 results.
     Args:
         query (str): The query to search for.
     """
     urls = list(search(query, tld="co.in", num=5, stop=10, pause=2))
     urls_detailed = []
 
     for url in urls:
@@ -163,14 +170,17 @@
     return urls_detailed
 
 def read_website(url):
     """
     Reads and returns the body of the website at the given url.
     Args:
         url (str): The url of the website to read.
+    Returns:
+        str: The body of the website.
+        None: If the request fails.
     """
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
     response = requests.get(url, headers=headers)
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, 'html.parser')
         body = soup.body        
         body_text = body.get_text(strip=True)
```

### Comparing `llm_axe-1.1.1/llm_axe/models.py` & `llm_axe-1.1.2/llm_axe/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,9 +8,15 @@
                                 example: OllamaChat(model='llama3:instruct')''')
 
         self._host = host
         self._model = model
         self._ollama = Client(host)
 
     def ask(self, prompts:list, format:str="", temperature:float=0.8):
+        """
+        Args:
+            prompts (list): A list of prompts to ask.
+            format (str, optional): The format of the response. Use "json" for json. Defaults to "".
+            temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
+        """
         return self._ollama.chat(model=self._model, messages=prompts, format=format, options={"temperature": temperature})["message"]["content"]
```

### Comparing `llm_axe-1.1.1/llm_axe/system_prompts.yaml` & `llm_axe-1.1.2/llm_axe/system_prompts.yaml`

 * *Files identical despite different names*

### Comparing `llm_axe-1.1.1/llm_axe.egg-info/PKG-INFO` & `llm_axe-1.1.2/llm_axe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-axe
-Version: 1.1.1
+Version: 1.1.2
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.1.1/setup.py` & `llm_axe-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.1' 
+VERSION = '1.1.2' 
 DESCRIPTION = 'A toolkit for quickly implementing llm powered functionalities.'
 LONG_DESCRIPTION = '''
 # llm-axe 🪓
 
 <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/llm-axe"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/llm-axe">
 <img alt="Static Badge" src="https://img.shields.io/badge/clones-63/month-purple"> <img alt="GitHub forks" src="https://img.shields.io/github/forks/emirsahin1/llm-axe?style=flat">
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Femirsahin1%2Fllm-axe&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/emirsahin1/llm-axe)
```

