# Comparing `tmp/chainlite-0.1.7.tar.gz` & `tmp/chainlite-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.7.tar", last modified: Sat May 25 17:14:12 2024, max compression
+gzip compressed data, was "chainlite-0.1.8.tar", last modified: Sun May 26 00:33:12 2024, max compression
```

## Comparing `chainlite-0.1.7.tar` & `chainlite-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 17:14:08.000000 chainlite-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-25 17:14:12.572204 chainlite-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-25 17:14:08.000000 chainlite-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.568204 chainlite-0.1.7/chainlite/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/llm_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/load_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-25 17:14:08.000000 chainlite-0.1.7/chainlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/chainlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 17:14:12.000000 chainlite-0.1.7/chainlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-25 17:14:08.000000 chainlite-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 17:14:12.572204 chainlite-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-25 17:14:08.000000 chainlite-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 17:14:08.000000 chainlite-0.1.7/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-25 17:14:08.000000 chainlite-0.1.7/tasks/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:14:12.572204 chainlite-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-25 17:14:08.000000 chainlite-0.1.7/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 00:32:57.000000 chainlite-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 00:33:12.102709 chainlite-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-26 00:32:57.000000 chainlite-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.098709 chainlite-0.1.8/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 00:32:57.000000 chainlite-0.1.8/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 00:33:12.000000 chainlite-0.1.8/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 00:32:57.000000 chainlite-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:33:12.102709 chainlite-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 00:32:57.000000 chainlite-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 00:32:57.000000 chainlite-0.1.8/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 00:32:57.000000 chainlite-0.1.8/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:33:12.102709 chainlite-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-26 00:32:57.000000 chainlite-0.1.8/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.7/LICENSE` & `chainlite-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.7/PKG-INFO` & `chainlite-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.7/README.md` & `chainlite-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.7/chainlite/llm_config.py` & `chainlite-0.1.8/chainlite/llm_config.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.7/chainlite/llm_generate.py` & `chainlite-0.1.8/chainlite/llm_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             should_skip = False
             for t in GlobalVars.prompts_to_skip_for_debugging:
                 if is_same_prompt(t, item["template_name"]):
                     should_skip = True
                     break
             if should_skip:
                 continue
+            if "output" not in item:
+                # happens if the code crashes in the middle of a an LLM call
+                continue
             f.write(
                 json.dumps(
                     {
                         key: item[key]
                         for key in [
                             "template_name",
                             "instruction",
@@ -208,27 +211,29 @@
 def llm_generation_chain(
     template_file: str,
     engine: str,
     max_tokens: int,
     temperature: float = 0.0,
     stop_tokens: Optional[list[str]] = None,
     top_p: float = 0.9,
+    keep_indentation: bool = False,
     postprocess: bool = False,
     bind_prompt_values: dict = {},
 ) -> Runnable:
     """
     Constructs a LangChain generation chain for LLM response utilizing LLM APIs prescribed in the ChainLite config file.
 
     Parameters:
         template_file (str): The path to the generation template file. Must be a .prompt file.
         engine (str): The language model engine to employ. An engine represents the left-hand value of an `engine_map` in the ChainLite config file.
         max_tokens (int): The upper limit of tokens the LLM can generate.
         temperature (float, optional): Dictates the randomness in the generation. Must be >= 0.0. Defaults to 0.0 (deterministic).
         stop_tokens (list[str], optional): The list of tokens causing the LLM to stop generating. Defaults to None.
         top_p (float, optional): The max cumulative probability for nucleus sampling, must be within 0.0 - 1.0. Defaults to 0.9.
+        keep_indentation (bool, optional): If True, will keep indentations at the beginning of each line in the template_file
         postprocess (bool, optional): If true, postprocessing deletes incomplete sentences from the end of the generation. Defaults to False.
         bind_prompt_values (dict, optional): A dictionary containing {Variable: str : Value}. Binds values to the prompt. Additional variables can be provided when the chain is called. Defaults to {}.
 
     Returns:
         Runnable: The language model generation chain
 
     Raises:
@@ -273,15 +278,15 @@
         if temperature == 0:
             model_kwargs["top_p"] = 1
 
     is_distilled = (
         "prompt_format" in llm_resource and llm_resource["prompt_format"] == "distilled"
     )
     prompt, distillation_instruction = load_fewshot_prompt_template(
-        template_file, is_distilled=is_distilled
+        template_file, is_distilled=is_distilled, keep_indentation=keep_indentation
     )
 
     llm = ChatLiteLLM(
         model_kwargs=model_kwargs,
         api_base=llm_resource["api_base"] if "api_base" in llm_resource else None,
         api_key=llm_resource["api_key"] if "api_key" in llm_resource else None,
         cache=(temperature == 0),
```

### Comparing `chainlite-0.1.7/chainlite/load_prompt.py` & `chainlite-0.1.8/chainlite/load_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,26 @@
         loader=loader,
         trim_blocks=True,
         lstrip_blocks=True,
     )
 
 
 @lru_cache()
-def load_template_file(template_file: str) -> str:
+def load_template_file(template_file: str, keep_indentation: bool) -> str:
     """
     This function is here just so that we can cache the templates and not have to read from disk every time.
     Also removes comment blocks and white space at the beginning and end of each line. These are usually added to make prompt templates more readable.
     We remove comment blocks first, so that we can get rid of extra lines before or after them.
     """
     raw_template = jinja_environment.loader.get_source(
         jinja_environment, template_file
     )[0]
     raw_template = re.sub(jinja2_comment_pattern, "", raw_template)
-    raw_template = "\n".join([line.strip() for line in raw_template.split("\n")])
+    if not keep_indentation:
+        raw_template = "\n".join([line.strip() for line in raw_template.split("\n")])
     raw_template = re.sub(
         r"%}\s*", "%}", raw_template
     )  # remove the white space after {% for ... %} tags etc.
 
     return raw_template
 
 
@@ -183,17 +184,17 @@
         )  # distillation prompts should not contain any variables other than template constants like {{today}}
         # print("distillation_instruction = ", distillation_instruction)
 
     return chat_prompt_template, distillation_instruction
 
 
 def load_fewshot_prompt_template(
-    template_file: str, is_distilled: bool
+    template_file: str, is_distilled: bool, keep_indentation: bool
 ) -> tuple[ChatPromptTemplate, str | None]:
-    fp = load_template_file(template_file)
+    fp = load_template_file(template_file, keep_indentation)
     blocks = _split_prompt_to_blocks(fp)
     # pprint(blocks)
     chat_prompt_template, distillation_instruction = _prompt_blocks_to_chat_messages(
         blocks, is_distilled
     )
 
     return chat_prompt_template, distillation_instruction
```

### Comparing `chainlite-0.1.7/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.8/chainlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.7/setup.py` & `chainlite-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.7",
+    version="0.1.8",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
```

### Comparing `chainlite-0.1.7/tasks/main.py` & `chainlite-0.1.8/tasks/main.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.7/tests/test_llm_generate.py` & `chainlite-0.1.8/tests/test_llm_generate.py`

 * *Files identical despite different names*

