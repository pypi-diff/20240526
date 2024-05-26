# Comparing `tmp/dendrite_python_sdk-0.1.0.tar.gz` & `tmp/dendrite_python_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dendrite_python_sdk-0.1.0.tar", max compression
+gzip compressed data, was "dendrite_python_sdk-1.0.0.tar", max compression
```

## Comparing `dendrite_python_sdk-0.1.0.tar` & `dendrite_python_sdk-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,73 @@
--rw-r--r--   0        0        0     1074 2024-02-02 14:20:43.049218 dendrite_python_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0     2466 2024-02-04 12:28:04.382995 dendrite_python_sdk-0.1.0/README.md
--rw-r--r--   0        0        0     3140 2024-02-04 15:58:17.415809 dendrite_python_sdk-0.1.0/dendrite_python_sdk/DendriteAPI.py
--rw-r--r--   0        0        0      499 2024-02-04 10:27:39.192650 dendrite_python_sdk-0.1.0/dendrite_python_sdk/InteractionTypes.py
--rw-r--r--   0        0        0        0 2024-02-02 14:19:13.740803 dendrite_python_sdk-0.1.0/dendrite_python_sdk/__init__.py
--rw-r--r--   0        0        0     2916 2024-02-04 16:42:27.331461 dendrite_python_sdk-0.1.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc
--rw-r--r--   0        0        0     3830 2024-02-04 16:47:29.348788 dendrite_python_sdk-0.1.0/dendrite_python_sdk/examples/agent.py
--rw-r--r--   0        0        0      219 2024-02-04 09:02:32.807278 dendrite_python_sdk-0.1.0/dendrite_python_sdk/models.py
--rw-r--r--   0        0        0     5932 2024-02-04 15:50:25.261983 dendrite_python_sdk-0.1.0/dendrite_python_sdk/openai_tools.py
--rw-r--r--   0        0        0      583 2024-02-04 12:30:29.702291 dendrite_python_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 dendrite_python_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-02-02 14:20:43.049218 dendrite_python_sdk-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6707 2024-05-26 16:58:56.466954 dendrite_python_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0       62 2024-05-15 17:53:47.139877 dendrite_python_sdk-1.0.0/dendrite_python_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 08:59:27.558957 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-20 09:08:52.601223 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4434 2024-05-26 16:15:03.183234 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/__pycache__/generate_text.cpython-312.pyc
+-rw-r--r--   0        0        0     2898 2024-05-26 16:15:03.183642 dendrite_python_sdk-1.0.0/dendrite_python_sdk/ai_util/generate_text.py
+-rw-r--r--   0        0        0     2361 2024-05-17 11:11:36.767261 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ActivePageManager.py
+-rw-r--r--   0        0        0     4580 2024-05-26 16:15:03.184074 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteBrowser.py
+-rw-r--r--   0        0        0     4849 2024-05-17 11:39:53.139850 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendriteLocator.py
+-rw-r--r--   0        0        0     6384 2024-05-26 16:58:56.468040 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/DendritePage.py
+-rw-r--r--   0        0        0     1620 2024-05-26 16:15:03.184385 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/ScreenshotManager.py
+-rw-r--r--   0        0        0     4301 2024-05-17 11:13:52.699998 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ActivePageManager.cpython-312.pyc
+-rw-r--r--   0        0        0     1748 2024-05-04 14:41:16.918373 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-310.pyc
+-rw-r--r--   0        0        0     3509 2024-05-15 11:35:02.885586 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupBrowser.cpython-312.pyc
+-rw-r--r--   0        0        0     2767 2024-05-04 14:41:16.919019 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-310.pyc
+-rw-r--r--   0        0        0     5965 2024-05-15 17:42:22.652233 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/AgentSoupPage.cpython-312.pyc
+-rw-r--r--   0        0        0     7400 2024-05-26 16:58:56.468580 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteBrowser.cpython-312.pyc
+-rw-r--r--   0        0        0     7192 2024-05-17 11:39:57.460426 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendriteLocator.cpython-312.pyc
+-rw-r--r--   0        0        0     9365 2024-05-26 17:08:20.406737 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/DendritePage.cpython-312.pyc
+-rw-r--r--   0        0        0     3222 2024-05-26 16:58:56.469429 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/ScreenshotManager.cpython-312.pyc
+-rw-r--r--   0        0        0     2919 2024-05-04 14:41:16.985071 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3778 2024-05-26 17:08:20.551411 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0      301 2024-05-16 06:48:31.744669 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/common/__pycache__/status.cpython-312.pyc
+-rw-r--r--   0        0        0       67 2024-05-16 06:25:40.442424 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/common/status.py
+-rw-r--r--   0        0        0     2732 2024-05-26 16:58:56.470225 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dendrite_browser/utils.py
+-rw-r--r--   0        0        0      280 2024-05-05 13:50:00.924479 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/GetInteractionDTO.py
+-rw-r--r--   0        0        0      386 2024-05-16 16:51:31.204276 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/GoogleSearchDTO.py
+-rw-r--r--   0        0        0      507 2024-05-15 11:04:30.884398 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/MakeInteractionDTO.py
+-rw-r--r--   0        0        0      382 2024-05-16 06:52:15.213330 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/ScrapePageDTO.py
+-rw-r--r--   0        0        0      661 2024-05-05 13:42:28.637321 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2024-05-05 13:50:13.259879 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GetInteractionDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      853 2024-05-16 16:55:29.849995 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/GoogleSearchDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      465 2024-05-05 13:42:28.638500 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfig.cpython-312.pyc
+-rw-r--r--   0        0        0      441 2024-05-05 13:42:28.639036 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      471 2024-05-05 13:42:28.639549 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/LLMConfigDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      992 2024-05-15 12:50:08.193062 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/MakeInteractionDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      909 2024-05-05 13:42:28.639943 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      816 2024-05-05 13:42:28.640332 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-310.pyc
+-rw-r--r--   0        0        0      915 2024-05-05 13:42:28.640720 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/PageInformationDTO.cpython-312.pyc
+-rw-r--r--   0        0        0      847 2024-05-16 06:52:50.171794 dendrite_python_sdk-1.0.0/dendrite_python_sdk/dto/__pycache__/ScrapePageDTO.cpython-312.pyc
+-rw-r--r--   0        0        0     2916 2024-02-04 16:42:27.331461 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc
+-rw-r--r--   0        0        0      784 2024-05-26 16:15:03.185863 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/get_steam_reviews.py
+-rw-r--r--   0        0        0     3028 2024-05-26 16:15:03.186113 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/review_sentiment.py
+-rw-r--r--   0        0        0     1426 2024-05-26 17:16:58.148127 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/send_discord_message.py
+-rw-r--r--   0        0        0      843 2024-05-26 16:58:56.470925 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/simple_example.py
+-rw-r--r--   0        0        0     1449 2024-05-24 13:38:38.546988 dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/yc.py
+-rw-r--r--   0        0        0     1244 2024-05-17 11:21:44.603429 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/DendriteException.py
+-rw-r--r--   0        0        0      142 2024-05-14 09:02:04.165589 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/IncorrectOutcomeException.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:02:01.998750 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     2526 2024-05-17 11:32:52.852813 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/DendriteException.cpython-312.pyc
+-rw-r--r--   0        0        0      504 2024-05-17 11:02:51.328702 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/IncorrectOutcomeException.cpython-312.pyc
+-rw-r--r--   0        0        0      199 2024-05-17 11:02:51.327921 dendrite_python_sdk-1.0.0/dendrite_python_sdk/exceptions/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0       85 2024-05-05 13:42:28.647626 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/LLMConfig.py
+-rw-r--r--   0        0        0      208 2024-05-05 13:50:08.291916 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/PageDeltaInformation.py
+-rw-r--r--   0        0        0      329 2024-05-05 13:49:28.012120 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/PageInformation.py
+-rw-r--r--   0        0        0        0 2024-05-05 13:42:28.648634 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-05 13:49:39.105411 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/LLMConfig.cpython-312.pyc
+-rw-r--r--   0        0        0      602 2024-05-15 11:35:03.288900 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageDeltaInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      934 2024-05-05 13:49:39.042358 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/PageInformation.cpython-312.pyc
+-rw-r--r--   0        0        0      195 2024-05-05 13:49:39.041818 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      219 2024-02-04 09:02:32.807278 dendrite_python_sdk-1.0.0/dendrite_python_sdk/models.py
+-rw-r--r--   0        0        0     2405 2024-05-26 16:15:03.186638 dendrite_python_sdk-1.0.0/dendrite_python_sdk/request_handler.py
+-rw-r--r--   0        0        0      210 2024-05-16 14:47:58.502176 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/GoogleSearchResponse.py
+-rw-r--r--   0        0        0      205 2024-05-16 06:26:28.003675 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/InteractionResponse.py
+-rw-r--r--   0        0        0      219 2024-05-16 07:41:52.278090 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/ScrapePageResponse.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:26:48.741213 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__init__.py
+-rw-r--r--   0        0        0      782 2024-05-16 16:55:29.851232 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/GoogleSearchResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      636 2024-05-16 06:48:31.795856 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/InteractionResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      661 2024-05-16 07:43:56.074864 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/ScrapePageResponse.cpython-312.pyc
+-rw-r--r--   0        0        0      198 2024-05-15 12:50:08.234795 dendrite_python_sdk-1.0.0/dendrite_python_sdk/responses/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      694 2024-05-26 18:07:19.190359 dendrite_python_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7414 1970-01-01 00:00:00.000000 dendrite_python_sdk-1.0.0/PKG-INFO
```

### Comparing `dendrite_python_sdk-0.1.0/LICENSE` & `dendrite_python_sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-0.1.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc` & `dendrite_python_sdk-1.0.0/dendrite_python_sdk/examples/__pycache__/agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dendrite_python_sdk-0.1.0/pyproject.toml` & `dendrite_python_sdk-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 [tool.poetry]
 name = "dendrite-python-sdk"
-version = "0.1.0"
+version = "1.0.0"
 description = ""
 authors = ["Charles Maddock <charles@dendrite.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.12"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 pydantic = "^2.6.0"
 openai = "^1.11.0"
+playwright = "^1.43.0"
+bs4 = "^0.0.2"
+lxml = "^5.2.1"
+backoff = "^2.2.1"
+pandas = "^2.2.2"
+openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.4"
 
 [build-system]
 requires = ["poetry-core", "requests", "python-dotenv", "pydantic"]
 build-backend = "poetry.core.masonry.api"
```

