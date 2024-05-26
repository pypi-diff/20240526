# Comparing `tmp/pydantic_prompter-0.1.8.tar.gz` & `tmp/pydantic_prompter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_prompter-0.1.8.tar", last modified: Thu Aug 31 06:17:06 2023, max compression
+gzip compressed data, was "pydantic_prompter-0.1.9.tar", last modified: Thu Aug 31 21:12:08 2023, max compression
```

## Comparing `pydantic_prompter-0.1.8.tar` & `pydantic_prompter-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     8522 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/./docs/index.md
--rw-r--r--   0        0        0      961 2023-08-31 06:17:06.635114 pydantic_prompter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       46 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/src/pydatic_prompter/__init__.py
--rw-r--r--   0        0        0      245 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/src/pydatic_prompter/exceptions.py
--rw-r--r--   0        0        0     5101 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/src/pydatic_prompter/prompter.py
--rw-r--r--   0        0        0        0 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1328 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/tests/gpt_tests.py
--rw-r--r--   0        0        0      203 2023-08-31 06:16:56.923056 pydantic_prompter-0.1.8/tests/settings.py
--rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 pydantic_prompter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     8516 2023-08-31 21:11:57.676999 pydantic_prompter-0.1.9/./docs/index.md
+-rw-r--r--   0        0        0      961 2023-08-31 21:12:08.841140 pydantic_prompter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/src/pydatic_prompter/__init__.py
+-rw-r--r--   0        0        0      245 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/src/pydatic_prompter/exceptions.py
+-rw-r--r--   0        0        0     4713 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/src/pydatic_prompter/prompter.py
+-rw-r--r--   0        0        0        0 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1323 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/tests/gpt_tests.py
+-rw-r--r--   0        0        0      329 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/tests/sanity.py
+-rw-r--r--   0        0        0      203 2023-08-31 21:11:57.680999 pydantic_prompter-0.1.9/tests/settings.py
+-rw-r--r--   0        0        0     9129 1970-01-01 00:00:00.000000 pydantic_prompter-0.1.9/PKG-INFO
```

### Comparing `pydantic_prompter-0.1.8/./docs/index.md` & `pydantic_prompter-0.1.9/./docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,26 +32,26 @@
     
 
 @Prompter(llm="openai", jinja=True, model_name="gpt-3.5-turbo-16k")
 def rank_recommendation_entries(
         json_entries, user_query
 ) -> RecommendationResults:
     """
-    >> system: You are a movie ranking expert
-    >> user: >
+    - system: You are a movie ranking expert
+    - user: >
         Which of the following JSON entries fit best to the query. 
         order by best fit descending
         Base your answer ONLY on the given YML entries, 
         if you are not sure, or there are no entries
 
-    >> user: >
+    - user: >
         The JSON entries:
         {{ json_entries }}
 
-    >> user: "query: {{ user_query }}"
+    - user: "query: {{ user_query }}"
 
     """
 
 my_entries = "[{\"text\": \"Description: Four everyday suburban guys come together as a ...."
 print(rank_recommendation_entries(json_entries=my_entries, user_query="Romantic comedy"))
 
 ```
@@ -78,18 +78,18 @@
 class RecommendationTitleResponse(BaseModel):
     title: str = Field(description="4 to 6 words title")
 
 
 @Prompter(llm="openai", jinja=True, model_name="gpt-3.5-turbo-16k")
 def recommendation_title(json_entries) -> RecommendationTitleResponse:
     """
-    >> user: >
+    - user: >
         Based on the JSON entries, suggest a minimum 4 words and maximum 6 words title
 
-    >> user: >
+    - user: >
         The JSON entries:
         {{ json_entries }}
 
     """
 
 ```
 Don't do this
```

### Comparing `pydantic_prompter-0.1.8/pyproject.toml` & `pydantic_prompter-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydantic-prompter"
-version = "0.1.8"
+version = "0.1.9"
 description = "This library helps you build prompts easily using Pydantic and OpenAi function calling API"
 authors = [
     { name = "Ofer Helman", email = "helmanofer@gmail.com" },
 ]
 readme = "./docs/index.md"
 dependencies = [
     "jinja2>=3.1.2",
```

### Comparing `pydantic_prompter-0.1.8/src/pydatic_prompter/prompter.py` & `pydantic_prompter-0.1.9/src/pydatic_prompter/prompter.py`

 * *Files 11% similar despite different names*

```diff
@@ -122,41 +122,24 @@
             raise
 
     def build_string(self, **inputs):
         msgs = self.build_prompt(**inputs)
         return "\n".join(map(str, msgs))
 
     def build_prompt(self, **inputs) -> List[Message]:
-        if self.jinja:
-            template = Template(self.function.__doc__, keep_trailing_newline=True)
-            y = template.render(**inputs)
-        else:
-            y = self.function.__doc__.format(**inputs)
-
-        line = ""
-        try:
-            y_list = []
-            for line in y.split(">> "):
-                line = line.strip()
-                if line:
-                    y_list.append(yaml.safe_load(line))
-        except Exception:
-            msg = f"\n\nFailed to parse prompt:\n{y}\nBad line:\n{line}\n"
-            logger.error(msg)
-            raise FailedToParsePromptError(msg)
-
-        messages = [
-            Message(
-                **{
-                    "role": list(item.keys())[0],
-                    "content": json.dumps(list(item.values())[0]),
-                }
-            )
-            for item in y_list
-        ]
+        y = yaml.safe_load(self.function.__doc__)
+        messages = []
+        for role_content in y:
+            role, content_template = list(role_content.items())[0]
+            if self.jinja:
+                template = Template(content_template, keep_trailing_newline=True)
+                content = template.render(**inputs)
+            else:
+                content = content_template.format(**inputs)
+            messages.append(Message(role=role, content=content))
         return messages
 
     def call_llm(self, messages: List[Message]):
         return_scheme_llm_str = self.parser.llm_schema()
 
         ret_str = self.llm.call(messages, return_scheme_llm_str)
         return self.parser.cast_result(ret_str)
```

### Comparing `pydantic_prompter-0.1.8/tests/gpt_tests.py` & `pydantic_prompter-0.1.9/tests/gpt_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     children: List[str] = Field(description="list of my children")
 
 
 def test_pydantic():
     @Prompter(jinja=True, llm="openai", model_name="gpt-3.5-turbo")
     def bbb(name) -> Hey:
         """
-        >> system: you are a writer
-        >> user: hi, my name is {{ name }} and my children are called, aa, bb, cc
-        >> user: |
+        - system: you are a writer
+        - user: hi, my name is {{ name }} and my children are called, aa, bb, cc
+        - user: |
             what is my name and my children name
         """
 
     res: Hey = bbb(name="Ofer")
     assert isinstance(res, Hey)
     assert res.name == "Ofer"
 
@@ -36,16 +36,16 @@
     children_names: List[str]
 
 
 def test_generic():
     @Prompter(llm="openai", model_name="gpt-3.5-turbo")
     def aaa(name) -> MyChildren:
         """
-        >> user: hi, my name is {name}  and my children are called, aa, bb, cc
-        >> user: |
+        - user: hi, my name is {name}  and my children are called, aa, bb, cc
+        - user: |
             how many children do I have
         """
 
     res: MyChildren = aaa(name="Ofer")
     assert isinstance(res, MyChildren)
     assert res.num_of_children == 3
     assert res.children_names == ["aa", "bb", "cc"]
```

### Comparing `pydantic_prompter-0.1.8/PKG-INFO` & `pydantic_prompter-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-prompter
-Version: 0.1.8
+Version: 0.1.9
 Summary: This library helps you build prompts easily using Pydantic and OpenAi function calling API
 Author-Email: Ofer Helman <helmanofer@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/helmanofer/pydantic-prompter
 Project-URL: Docs, https://helmanofer.github.io/pydantic-prompter/
 Requires-Python: >=3.10
 Requires-Dist: jinja2>=3.1.2
@@ -49,26 +49,26 @@
     
 
 @Prompter(llm="openai", jinja=True, model_name="gpt-3.5-turbo-16k")
 def rank_recommendation_entries(
         json_entries, user_query
 ) -> RecommendationResults:
     """
-    >> system: You are a movie ranking expert
-    >> user: >
+    - system: You are a movie ranking expert
+    - user: >
         Which of the following JSON entries fit best to the query. 
         order by best fit descending
         Base your answer ONLY on the given YML entries, 
         if you are not sure, or there are no entries
 
-    >> user: >
+    - user: >
         The JSON entries:
         {{ json_entries }}
 
-    >> user: "query: {{ user_query }}"
+    - user: "query: {{ user_query }}"
 
     """
 
 my_entries = "[{\"text\": \"Description: Four everyday suburban guys come together as a ...."
 print(rank_recommendation_entries(json_entries=my_entries, user_query="Romantic comedy"))
 
 ```
@@ -95,18 +95,18 @@
 class RecommendationTitleResponse(BaseModel):
     title: str = Field(description="4 to 6 words title")
 
 
 @Prompter(llm="openai", jinja=True, model_name="gpt-3.5-turbo-16k")
 def recommendation_title(json_entries) -> RecommendationTitleResponse:
     """
-    >> user: >
+    - user: >
         Based on the JSON entries, suggest a minimum 4 words and maximum 6 words title
 
-    >> user: >
+    - user: >
         The JSON entries:
         {{ json_entries }}
 
     """
 
 ```
 Don't do this
```

