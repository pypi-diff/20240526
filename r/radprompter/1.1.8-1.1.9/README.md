# Comparing `tmp/radprompter-1.1.8.tar.gz` & `tmp/radprompter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.1.8.tar` & `radprompter-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3179 2024-05-20 13:29:10.318934 radprompter-1.1.8/.gitignore
--rw-r--r--   0        0        0    35149 2024-05-22 15:01:58.548435 radprompter-1.1.8/LICENSE
--rw-r--r--   0        0        0     3574 2024-05-20 18:02:28.892553 radprompter-1.1.8/README.md
--rw-r--r--   0        0        0    91362 2024-05-19 21:36:28.548393 radprompter-1.1.8/logo.png
--rw-r--r--   0        0        0      704 2024-05-22 15:01:24.749407 radprompter-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      244 2024-05-20 18:02:28.893874 radprompter-1.1.8/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-22 15:01:36.269039 radprompter-1.1.8/radprompter/__version__.py
--rw-r--r--   0        0        0      146 2024-05-20 02:33:21.208331 radprompter-1.1.8/radprompter/clients/__init__.py
--rw-r--r--   0        0        0      586 2024-05-19 22:16:28.933183 radprompter-1.1.8/radprompter/clients/clients.py
--rw-r--r--   0        0        0     3231 2024-05-20 18:02:28.894660 radprompter-1.1.8/radprompter/clients/huggingface/clients.py
--rw-r--r--   0        0        0     3022 2024-05-19 22:09:18.270492 radprompter-1.1.8/radprompter/clients/openai/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.8/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9976 2024-05-20 18:02:28.895187 radprompter-1.1.8/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     7303 2024-05-20 18:02:28.895411 radprompter-1.1.8/radprompter/radprompter.py
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.8/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.8/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.8/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0    16815 2024-05-20 18:02:28.895704 radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    17861 2024-05-20 18:02:28.896056 radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
--rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.toml
--rw-r--r--   0        0        0    19275 2024-05-20 18:02:28.896577 radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
--rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
--rw-r--r--   0        0        0    27143 2024-05-20 18:02:28.896937 radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.toml
--rw-r--r--   0        0        0    24106 2024-05-20 18:02:28.897096 radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb
--rw-r--r--   0        0        0     3277 2024-05-20 18:02:28.897513 radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml
--rw-r--r--   0        0        0    18209 2024-05-20 18:02:28.897622 radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb
--rw-r--r--   0        0        0     1922 2024-05-20 18:02:28.897715 radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml
--rw-r--r--   0        0        0     1825 2024-05-20 18:02:28.897911 radprompter-1.1.8/tutorials/README.md
--rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 radprompter-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3179 2024-05-20 13:29:10.318934 radprompter-1.1.9/.gitignore
+-rw-r--r--   0        0        0    35149 2024-05-22 15:01:58.548435 radprompter-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3574 2024-05-20 18:02:28.892553 radprompter-1.1.9/README.md
+-rw-r--r--   0        0        0    91362 2024-05-19 21:36:28.548393 radprompter-1.1.9/logo.png
+-rw-r--r--   0        0        0      704 2024-05-22 15:01:24.749407 radprompter-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-20 18:02:28.893874 radprompter-1.1.9/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-22 15:10:49.825209 radprompter-1.1.9/radprompter/__version__.py
+-rw-r--r--   0        0        0      146 2024-05-20 02:33:21.208331 radprompter-1.1.9/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-19 22:16:28.933183 radprompter-1.1.9/radprompter/clients/clients.py
+-rw-r--r--   0        0        0     3231 2024-05-20 18:02:28.894660 radprompter-1.1.9/radprompter/clients/huggingface/clients.py
+-rw-r--r--   0        0        0     3022 2024-05-19 22:09:18.270492 radprompter-1.1.9/radprompter/clients/openai/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.9/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9976 2024-05-20 18:02:28.895187 radprompter-1.1.9/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7381 2024-05-22 15:10:37.775485 radprompter-1.1.9/radprompter/radprompter.py
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.9/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.9/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.9/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0    16815 2024-05-20 18:02:28.895704 radprompter-1.1.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17861 2024-05-20 18:02:28.896056 radprompter-1.1.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.9/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19275 2024-05-20 18:02:28.896577 radprompter-1.1.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    27143 2024-05-20 18:02:28.896937 radprompter-1.1.9/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    24106 2024-05-20 18:02:28.897096 radprompter-1.1.9/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb
+-rw-r--r--   0        0        0     3277 2024-05-20 18:02:28.897513 radprompter-1.1.9/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml
+-rw-r--r--   0        0        0    18209 2024-05-20 18:02:28.897622 radprompter-1.1.9/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb
+-rw-r--r--   0        0        0     1922 2024-05-20 18:02:28.897715 radprompter-1.1.9/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml
+-rw-r--r--   0        0        0     1825 2024-05-20 18:02:28.897911 radprompter-1.1.9/tutorials/README.md
+-rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 radprompter-1.1.9/PKG-INFO
```

### Comparing `radprompter-1.1.8/.gitignore` & `radprompter-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/LICENSE` & `radprompter-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/README.md` & `radprompter-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/logo.png` & `radprompter-1.1.9/logo.png`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/pyproject.toml` & `radprompter-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/radprompter/clients/clients.py` & `radprompter-1.1.9/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/radprompter/clients/huggingface/clients.py` & `radprompter-1.1.9/radprompter/clients/huggingface/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/radprompter/clients/openai/clients.py` & `radprompter-1.1.9/radprompter/clients/openai/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/radprompter/prompts/prompts.py` & `radprompter-1.1.9/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/radprompter/radprompter.py` & `radprompter-1.1.9/radprompter/radprompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         messages = [
             {"role": "system", "content": prompt.system_prompt},
         ]
         item_response = []
         for schema in prompt.schemas.schemas:
             schema_response = []
             prompt_with_schema = deepcopy(prompt)
-            prompt_with_schema.replace_placeholders(schema | item)
+            merged_dict = deepcopy(schema)
+            merged_dict.update(item)
+            prompt_with_schema.replace_placeholders(merged_dict)
         
             for i in range(prompt.num_turns):
                 messages.append({"role": "user", "content": prompt_with_schema.user_prompts[i]})
                 if prompt.response_templates[i] != "":
                     messages.append({"role": "assistant", "content": prompt_with_schema.response_templates[i]})
                 
                 response, messages = self.client.ask_model(messages, prompt_with_schema.stop_tags[i])
```

### Comparing `radprompter-1.1.8/sample_reports/sample_report_1.txt` & `radprompter-1.1.9/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/sample_reports/sample_report_2.txt` & `radprompter-1.1.9/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/sample_reports/sample_report_3.txt` & `radprompter-1.1.9/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.1.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb` & `radprompter-1.1.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.toml` & `radprompter-1.1.9/tutorials/02_RDP-Templating/02_RDP-Templating.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb` & `radprompter-1.1.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml` & `radprompter-1.1.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb` & `radprompter-1.1.9/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.toml` & `radprompter-1.1.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb` & `radprompter-1.1.9/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml` & `radprompter-1.1.9/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb` & `radprompter-1.1.9/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml` & `radprompter-1.1.9/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/tutorials/README.md` & `radprompter-1.1.9/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.8/PKG-INFO` & `radprompter-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.1.8
+Version: 1.1.9
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pandas
```

