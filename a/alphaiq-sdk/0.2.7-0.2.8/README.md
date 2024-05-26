# Comparing `tmp/alphaiq-sdk-0.2.7.tar.gz` & `tmp/alphaiq_sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaiq-sdk-0.2.7.tar", last modified: Sun Apr  7 21:52:30 2024, max compression
+gzip compressed data, was "alphaiq_sdk-0.2.8.tar", last modified: Sun May 26 02:44:38 2024, max compression
```

## Comparing `alphaiq-sdk-0.2.7.tar` & `alphaiq_sdk-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.962014 alphaiq-sdk-0.2.7/
--rw-rw-rw-   0        0        0     7865 2024-04-07 21:52:30.961016 alphaiq-sdk-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     7293 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.944016 alphaiq-sdk-0.2.7/alphaiq_sdk/
--rw-rw-rw-   0        0        0       37 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/__init__.py
--rw-rw-rw-   0        0        0      520 2024-04-04 16:33:26.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/client.py
--rw-rw-rw-   0        0        0     1578 2024-04-07 21:50:10.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/generative.py
--rw-rw-rw-   0        0        0     2538 2024-04-07 21:50:10.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/mapping.py
--rw-rw-rw-   0        0        0     1595 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/models.py
--rw-rw-rw-   0        0        0     1840 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.961016 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/
--rw-rw-rw-   0        0        0     7865 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      735 2024-04-07 21:52:07.000000 alphaiq-sdk-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 21:52:30.963014 alphaiq-sdk-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.960018 alphaiq-sdk-0.2.7/test/
--rw-rw-rw-   0        0        0     2025 2024-04-04 15:51:38.000000 alphaiq-sdk-0.2.7/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 02:44:38.070098 alphaiq_sdk-0.2.8/
+-rw-rw-rw-   0        0        0     7907 2024-05-26 02:44:38.065444 alphaiq_sdk-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7293 2024-03-28 23:57:31.000000 alphaiq_sdk-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 02:44:37.998843 alphaiq_sdk-0.2.8/alphaiq_sdk/
+-rw-rw-rw-   0        0        0       37 2024-03-28 23:57:31.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/__init__.py
+-rw-rw-rw-   0        0        0      519 2024-05-26 02:43:56.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/client.py
+-rw-rw-rw-   0        0        0     1067 2024-05-25 21:26:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/generative.py
+-rw-rw-rw-   0        0        0     2489 2024-05-25 18:49:30.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/mapping.py
+-rw-rw-rw-   0        0        0     1526 2024-05-25 21:18:21.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/models.py
+-rw-rw-rw-   0        0        0     1696 2024-05-25 19:28:50.000000 alphaiq_sdk-0.2.8/alphaiq_sdk/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-26 02:44:38.065444 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/
+-rw-rw-rw-   0        0        0     7907 2024-05-26 02:44:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-26 02:44:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 02:44:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-26 02:44:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 02:44:37.000000 alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      777 2024-05-25 16:19:03.000000 alphaiq_sdk-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 02:44:38.070555 alphaiq_sdk-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 02:44:38.056696 alphaiq_sdk-0.2.8/test/
+-rw-rw-rw-   0        0        0     1854 2024-05-25 21:30:54.000000 alphaiq_sdk-0.2.8/test/test.py
```

### Comparing `alphaiq-sdk-0.2.7/PKG-INFO` & `alphaiq_sdk-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphaiq-sdk
-Version: 0.2.7
-Summary: Access AlphaIQ quantitative linguistics signals and generative content
+Version: 0.2.8
+Summary: Access AlphaIQ's generative insights, explainable investment signals, and the Corporate Transparency Score model
 Author-email: AlphaIQ <contact@alphaiq.ai>
 Project-URL: GitHub, https://github.com/alphaiq-ai/python-sdk
 Keywords: risk,AI,fintech,investing,NLP,GenAI
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=14.05.14
```

### Comparing `alphaiq-sdk-0.2.7/README.md` & `alphaiq_sdk-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk/client.py` & `alphaiq_sdk-0.2.8/alphaiq_sdk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from alphaiq_sdk.mapping import Mapping
 from alphaiq_sdk.generative import Generative
 
 class AlphaIQ(Signals, Models, Mapping, Generative):
 
     def __init__(self, token):
         self.token = token
-        self.host_url = "https://data.app.alphaiq.ai/api/v1/"
+        self.host_url = "https://data.app.alphaiq.ai/api/v1"
         self.headers = {'Authorization': f'Bearer {token}'}
         super().__init__(self.host_url, self.headers)
 
 def client(token):
     return AlphaIQ(token)
```

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk/generative.py` & `alphaiq_sdk-0.2.8/alphaiq_sdk/generative.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 import requests
 
 class Generative:
     def __init__(self, host_url, headers):
         self.host_url = host_url
         self.headers = headers
 
-    def get_spinsights_explorer_spindex_summary(self, ticker: str):
+    def get_signal_explanations(self, ticker: str):
 
-        url = self.host_url + f"/generative/company/spinsights/explorerContent/{ticker}"
+        url = self.host_url + f"/generative/company/signal_explanation/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response
-     
-    def get_spinsights_report_content(self, ticker: str):
 
-        url = self.host_url + f"/generative/company/spinsights/reportContent/{ticker}"
-
-        response = requests.get(url, headers=self.headers).json()
-        return response 
-
-    def get_spinsights_report_pdf(self, ticker: str):
-
-        url = self.host_url + f"/pdf/spinsights/{ticker}"
-
-        response = requests.get(url, headers=self.headers).json()
-        return response 
-
-    def get_compass_explorer_question_answer(self, ticker: str):
+    def get_question_answer(self, ticker: str):
 
         url = self.host_url + f"/generative/company/compass/questionContent/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response 
 
-    def get_compass_report_content(self, ticker: str):
+    def get_trending_content(self, ticker: str):
 
         url = self.host_url + f"/generative/company/compass/reportContent/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response 
     
     def get_compass_report_pdf(self, ticker: str):
```

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk/mapping.py` & `alphaiq_sdk-0.2.8/alphaiq_sdk/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         optional_args = {
             'consilienceId': kwargs.get('consilienceId', None),
             'ticker': kwargs.get('ticker', None),
             'cik': kwargs.get('cik', None),
             'lei': kwargs.get('lei', None),
             'isin': kwargs.get('isin', None),
             'cusip': kwargs.get('cusip', None),
-            'sedol': kwargs.get('sedol', None),
             'figi': kwargs.get('figi',None),
             'compositeFigi': kwargs.get('compositeFigi',None),
             'shareClassFigi': kwargs.get('shareClassFigi',None)
         }
 
         # Checking if at least one optional argument is present
         if not any(optional_args.values()):
```

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk/models.py` & `alphaiq_sdk-0.2.8/alphaiq_sdk/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import requests
 
 class Models:
     def __init__(self, host_url, headers):
         self.host_url = host_url
         self.headers = headers
 
-    def get_models_spindex(self, rawSmoothFlag: str, startDate: str, endDate: str, **kwargs):
+    def get_models_corporate_transparency(self, modelVariation: str, startDate: str, endDate: str, **kwargs):
         optional_args = {
             'consilience_id': kwargs.get('consilience_id', None),
             'ticker': kwargs.get('ticker', None),
             'cik': kwargs.get('cik', None),
             'lei': kwargs.get('lei', None),
             'isin': kwargs.get('isin', None),
-            'cusip': kwargs.get('cusip', None),
-            'sedol': kwargs.get('sedol', None)
+            'cusip': kwargs.get('cusip', None)
         }
 
         # Checking if at least one optional argument is present
         if not any(optional_args.values()):
             raise ValueError("One and only one company identifier argument must be provided.")
 
-        url = self.host_url + "/models/spindex?"
+        url = self.host_url + "/models/corporateTransparency?"
         
         # Constructing URL based on provided optional arguments
         for key, value in optional_args.items():
             if value is not None:
                 url += f"{key}={value}&"
 
         # Adding mandatory arguments to the URL
-        url += f"rawSmoothFlag={rawSmoothFlag}&startDate={startDate}&endDate={endDate}"
+        url += f"modelVariation={modelVariation}&startDate={startDate}&endDate={endDate}"
 
         response = requests.get(url, headers=self.headers).json()
         return response
     
-    def get_bulk_model(self, rawSmoothFlag: str, model_name: str):
+    def get_bulk_model(self, modelName: str):
 
-        url = self.host_url + f"/bulk/models?rawSmoothFlag={rawSmoothFlag}&modelName={model_name}"
+        url = self.host_url + f"/bulk/models?modelName={modelName}"
 
         response = requests.get(url, headers=self.headers).json()
         return response
```

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk/signals.py` & `alphaiq_sdk-0.2.8/alphaiq_sdk/signals.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import requests
 
 class Signals:
     def __init__(self, host_url, headers):
         self.host_url = host_url
         self.headers = headers
 
-    def get_quant_linguistics_signals(self, startDate: str, endDate: str, **kwargs):
+    def get_quant_linguistics_signals(self, signalVariation: str, startDate: str, endDate: str, **kwargs):
         optional_args = {
             'consilienceId': kwargs.get('consilience_id', None),
             'ticker': kwargs.get('ticker', None),
             'cik': kwargs.get('cik', None),
             'lei': kwargs.get('lei', None),
             'isin': kwargs.get('isin', None),
-            'cusip': kwargs.get('cusip', None),
-            'sedol': kwargs.get('sedol', None)
+            'cusip': kwargs.get('cusip', None)
         }
 
         # Checking if at least one optional argument is present
         if not any(optional_args.values()):
             raise ValueError("One and only one company identifier argument must be provided.")
 
         url = self.host_url + "/signals/quantLinguistics?"
         
         # Constructing URL based on provided optional arguments
         for key, value in optional_args.items():
             if value is not None:
                 url += f"{key}={value}&"
 
         # Adding mandatory arguments to the URL
-        url += f"startDate={startDate}&endDate={endDate}"
+        url += f"signalVariation={signalVariation}&startDate={startDate}&endDate={endDate}"
 
         response = requests.get(url, headers=self.headers).json()
         return response
     
-    def get_bulk_signals(self, strategyType: str):
+    def get_bulk_signals_all(self):
 
-        url = self.host_url + f"/bulk/signals?strategyType={strategyType}"
+        url = self.host_url + f"/bulk/signals/all"
 
         response = requests.get(url, headers=self.headers).json()
         return response
     
-    def get_bulk_signals_yearly(self, strategyType: str, alphaHorizon: str, year: int):
+    def get_bulk_signals_top_level(self):
 
-        url = self.host_url + f"/bulk/signals/yearly?strategyType={strategyType}&alphaHorizon={alphaHorizon}&year={year}"
+        url = self.host_url + f"/bulk/signals/topLevel"
 
         response = requests.get(url, headers=self.headers).json()
         return response
```

### Comparing `alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/PKG-INFO` & `alphaiq_sdk-0.2.8/alphaiq_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphaiq-sdk
-Version: 0.2.7
-Summary: Access AlphaIQ quantitative linguistics signals and generative content
+Version: 0.2.8
+Summary: Access AlphaIQ's generative insights, explainable investment signals, and the Corporate Transparency Score model
 Author-email: AlphaIQ <contact@alphaiq.ai>
 Project-URL: GitHub, https://github.com/alphaiq-ai/python-sdk
 Keywords: risk,AI,fintech,investing,NLP,GenAI
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=14.05.14
```

### Comparing `alphaiq-sdk-0.2.7/pyproject.toml` & `alphaiq_sdk-0.2.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphaiq-sdk"
-version = "0.2.7"
-description = "Access AlphaIQ quantitative linguistics signals and generative content"
+version = "0.2.8"
+description = "Access AlphaIQ's generative insights, explainable investment signals, and the Corporate Transparency Score model"
 readme = "README.md"
 authors = [{ name = "AlphaIQ", email = "contact@alphaiq.ai" }]
 
 classifiers = [
     "Programming Language :: Python",
 ]
 keywords = ["risk", "AI", "fintech", "investing","NLP", "GenAI"]
```

### Comparing `alphaiq-sdk-0.2.7/test/test.py` & `alphaiq_sdk-0.2.8/test/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,35 +13,31 @@
 
         writer.writeheader()
         for check in output_checks:
             writer.writerow(check)
 
 function_list = [
     aiq.get_quant_linguistics_signals(),
-    aiq.get_bulk_signals(),
-    aiq.get_bulk_signals_yearly(),
-    aiq.get_models_spindex(),
+    aiq.get_bulk_signals_all(),
+    aiq.get_bulk_signals_top_level(),
+    aiq.get_models_corporate_transparency(),
     aiq.get_bulk_model(),
     aiq.get_company_identifiers_map_compositeFigi(),
     aiq.get_company_identifiers_map_cik(),
     aiq.get_company_identifiers_map_consilienceId(),
     aiq.get_company_identifiers_map_cusip(),
     aiq.get_company_identifiers_map_figi(),
     aiq.get_company_identifiers_map_isin(),
     aiq.get_company_identifiers_map_lei(),
     aiq.get_company_identifiers_map_shareClassFigi(),
     aiq.get_company_identifiers_map_ticker(),
-    aiq.get_spindex_factors_map(),
     aiq.get_bulk_mapping(),
-    aiq.get_compass_questions_map(),
-    aiq.get_spinsights_explorer_spindex_summary(),
-    aiq.get_spinsights_report_content(),
-    aiq.get_spinsights_report_pdf(),
-    aiq.get_compass_explorer_question_answer(),
-    aiq.get_compass_report_content(),
+    aiq.get_signal_explanations(),
+    aiq.get_question_answer(),
+    aiq.get_trending_content(),
     aiq.get_compass_report_pdf()
 ]
 
 output_checks= []
 i=0
 for function in function_list:
     i+=1
```

