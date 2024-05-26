# Comparing `tmp/languru-0.8.0.tar.gz` & `tmp/languru-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languru-0.8.0.tar", max compression
+gzip compressed data, was "languru-0.9.0.tar", max compression
```

## Comparing `languru-0.8.0.tar` & `languru-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,74 @@
--rw-r--r--   0        0        0    11357 2024-02-01 11:42:52.861485 languru-0.8.0/LICENSE
--rw-r--r--   0        0        0    10182 2024-04-02 11:20:24.107511 languru-0.8.0/README.md
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861665 languru-0.8.0/languru/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.580590 languru-0.8.0/languru/action/__init__.py
--rw-r--r--   0        0        0     8883 2024-04-09 05:41:11.395565 languru-0.8.0/languru/action/anthropic.py
--rw-r--r--   0        0        0     6062 2024-05-02 11:28:26.551743 languru-0.8.0/languru/action/base.py
--rw-r--r--   0        0        0     7655 2024-03-19 05:31:55.754602 languru-0.8.0/languru/action/google.py
--rw-r--r--   0        0        0     2816 2024-03-27 09:02:07.247643 languru-0.8.0/languru/action/groq.py
--rw-r--r--   0        0        0    18777 2024-03-19 05:31:55.754961 languru-0.8.0/languru/action/hf.py
--rw-r--r--   0        0        0    11336 2024-05-02 11:28:26.552129 languru-0.8.0/languru/action/openai.py
--rw-r--r--   0        0        0     2999 2024-03-27 09:02:07.249387 languru-0.8.0/languru/action/pplx.py
--rw-r--r--   0        0        0     1105 2024-03-22 10:50:29.684729 languru-0.8.0/languru/action/utils.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861745 languru-0.8.0/languru/cli/__init__.py
--rw-r--r--   0        0        0     3327 2024-03-22 10:21:59.204779 languru-0.8.0/languru/cli/main.py
--rw-r--r--   0        0        0      221 2024-02-07 08:19:21.426236 languru-0.8.0/languru/config.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755531 languru-0.8.0/languru/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755648 languru-0.8.0/languru/examples/return_values/__init__.py
--rw-r--r--   0        0        0     9704 2024-03-19 05:31:55.755827 languru-0.8.0/languru/examples/return_values/_openai.py
--rw-r--r--   0        0        0       41 2024-02-15 01:55:28.093981 languru-0.8.0/languru/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582508 languru-0.8.0/languru/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582657 languru-0.8.0/languru/resources/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582788 languru-0.8.0/languru/resources/model/__init__.py
--rw-r--r--   0        0        0     4394 2024-03-09 09:50:32.758650 languru-0.8.0/languru/resources/model/discovery.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861878 languru-0.8.0/languru/server/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 02:00:42.777707 languru-0.8.0/languru/server/api/__init__.py
--rw-r--r--   0        0        0      977 2024-05-02 11:28:26.552436 languru-0.8.0/languru/server/api/v1/__init__.py
--rw-r--r--   0        0        0    13646 2024-05-02 11:50:59.857764 languru-0.8.0/languru/server/api/v1/audio.py
--rw-r--r--   0        0        0     7533 2024-04-26 10:50:57.406091 languru-0.8.0/languru/server/api/v1/chat.py
--rw-r--r--   0        0        0     5796 2024-03-22 10:07:39.202848 languru-0.8.0/languru/server/api/v1/completions.py
--rw-r--r--   0        0        0     4423 2024-03-22 10:07:39.203160 languru-0.8.0/languru/server/api/v1/embeddings.py
--rw-r--r--   0        0        0    12851 2024-05-03 10:19:03.656272 languru-0.8.0/languru/server/api/v1/images.py
--rw-r--r--   0        0        0     9679 2024-03-19 05:31:55.756461 languru-0.8.0/languru/server/api/v1/model.py
--rw-r--r--   0        0        0     4353 2024-03-22 10:07:39.203389 languru-0.8.0/languru/server/api/v1/moderations.py
--rw-r--r--   0        0        0     5950 2024-05-02 11:52:33.822371 languru-0.8.0/languru/server/api/v1/test_audio.py
--rw-r--r--   0        0        0     5020 2024-03-19 05:31:55.756725 languru-0.8.0/languru/server/api/v1/test_chat.py
--rw-r--r--   0        0        0     4807 2024-03-19 05:31:55.756818 languru-0.8.0/languru/server/api/v1/test_completions.py
--rw-r--r--   0        0        0     2475 2024-03-19 05:31:55.756905 languru-0.8.0/languru/server/api/v1/test_embeddings.py
--rw-r--r--   0        0        0     6347 2024-05-03 10:19:01.498146 languru-0.8.0/languru/server/api/v1/test_images.py
--rw-r--r--   0        0        0     3501 2024-03-19 05:31:55.757121 languru-0.8.0/languru/server/api/v1/test_model.py
--rw-r--r--   0        0        0     2263 2024-03-19 05:31:55.757219 languru-0.8.0/languru/server/api/v1/test_moderations.py
--rw-r--r--   0        0        0     6958 2024-03-27 09:02:07.250950 languru-0.8.0/languru/server/config.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757554 languru-0.8.0/languru/server/deps/__init__.py
--rw-r--r--   0        0        0      429 2024-03-19 05:31:55.757647 languru-0.8.0/languru/server/deps/common.py
--rw-r--r--   0        0        0     5166 2024-04-30 11:04:16.965702 languru-0.8.0/languru/server/main.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757760 languru-0.8.0/languru/server/utils/__init__.py
--rw-r--r--   0        0        0     1270 2024-03-19 05:31:55.758226 languru-0.8.0/languru/server/utils/common.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585801 languru-0.8.0/languru/types/__init__.py
--rw-r--r--   0        0        0     7400 2024-05-02 11:28:26.554544 languru-0.8.0/languru/types/audio.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585941 languru-0.8.0/languru/types/chat/__init__.py
--rw-r--r--   0        0        0     2059 2024-04-09 05:41:11.396468 languru-0.8.0/languru/types/chat/anthropic.py
--rw-r--r--   0        0        0     3094 2024-04-09 05:41:11.397143 languru-0.8.0/languru/types/chat/completions.py
--rw-r--r--   0        0        0     2895 2024-03-19 05:31:55.758398 languru-0.8.0/languru/types/completions.py
--rw-r--r--   0        0        0      603 2024-02-15 01:55:28.096416 languru-0.8.0/languru/types/embeddings.py
--rw-r--r--   0        0        0     7693 2024-05-02 11:28:26.554852 languru-0.8.0/languru/types/images.py
--rw-r--r--   0        0        0      158 2024-02-07 06:54:11.803747 languru-0.8.0/languru/types/model/__init__.py
--rw-r--r--   0        0        0      454 2024-02-07 07:01:30.525620 languru-0.8.0/languru/types/model/orm.py
--rw-r--r--   0        0        0      403 2024-02-15 01:55:28.096482 languru-0.8.0/languru/types/moderations.py
--rw-r--r--   0        0        0        0 2024-02-15 01:55:28.096547 languru-0.8.0/languru/utils/__init__.py
--rw-r--r--   0        0        0     1622 2024-02-18 04:18:45.843584 languru-0.8.0/languru/utils/calculation.py
--rw-r--r--   0        0        0     2796 2024-04-26 07:07:31.295222 languru-0.8.0/languru/utils/common.py
--rw-r--r--   0        0        0     2328 2024-03-08 08:14:03.711878 languru-0.8.0/languru/utils/device.py
--rw-r--r--   0        0        0     3213 2024-03-11 03:18:17.779132 languru-0.8.0/languru/utils/hf.py
--rw-r--r--   0        0        0     1666 2024-03-19 05:31:55.758527 languru-0.8.0/languru/utils/http.py
--rw-r--r--   0        0        0     1163 2024-02-15 01:55:28.096890 languru-0.8.0/languru/utils/socket.py
--rw-r--r--   0        0        0     2854 2024-04-03 03:38:53.649106 languru-0.8.0/languru/utils/xml.py
--rw-r--r--   0        0        0       63 2024-05-03 10:30:00.748588 languru-0.8.0/languru/version.py
--rw-r--r--   0        0        0     4427 2024-05-03 10:29:48.106401 languru-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    13127 1970-01-01 00:00:00.000000 languru-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-29 14:01:08.176794 languru-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10388 2024-05-04 12:43:00.882169 languru-0.9.0/README.md
+-rw-r--r--   0        0        0     1035 2024-05-04 12:25:34.197403 languru-0.9.0/languru/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:57:47.271478 languru-0.9.0/languru/action/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-06 08:43:25.015213 languru-0.9.0/languru/action/anthropic.py
+-rw-r--r--   0        0        0     6062 2024-04-28 06:59:01.966486 languru-0.9.0/languru/action/base.py
+-rw-r--r--   0        0        0     7655 2024-03-26 14:02:44.546930 languru-0.9.0/languru/action/google.py
+-rw-r--r--   0        0        0     2816 2024-03-26 14:02:44.547223 languru-0.9.0/languru/action/groq.py
+-rw-r--r--   0        0        0    18777 2024-03-26 14:02:44.547591 languru-0.9.0/languru/action/hf.py
+-rw-r--r--   0        0        0    11336 2024-04-28 01:12:08.948392 languru-0.9.0/languru/action/openai.py
+-rw-r--r--   0        0        0     2999 2024-03-26 14:02:44.549070 languru-0.9.0/languru/action/pplx.py
+-rw-r--r--   0        0        0     1105 2024-03-26 14:02:44.549471 languru-0.9.0/languru/action/utils.py
+-rw-r--r--   0        0        0        0 2024-01-30 14:23:22.088837 languru-0.9.0/languru/cli/__init__.py
+-rw-r--r--   0        0        0     3327 2024-03-26 14:02:44.549872 languru-0.9.0/languru/cli/main.py
+-rw-r--r--   0        0        0      274 2024-05-04 13:35:54.769769 languru-0.9.0/languru/config.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.549916 languru-0.9.0/languru/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.550015 languru-0.9.0/languru/examples/return_values/__init__.py
+-rw-r--r--   0        0        0     9704 2024-03-26 14:02:44.550369 languru-0.9.0/languru/examples/return_values/_openai.py
+-rw-r--r--   0        0        0       41 2024-02-10 12:12:53.654103 languru-0.9.0/languru/exceptions.py
+-rw-r--r--   0        0        0       67 2024-05-04 04:43:43.511205 languru-0.9.0/languru/models/__init__.py
+-rw-r--r--   0        0        0     2802 2024-05-04 13:41:39.387134 languru-0.9.0/languru/models/base.py
+-rw-r--r--   0        0        0       78 2024-05-04 08:24:48.268314 languru-0.9.0/languru/prompts/__init__.py
+-rw-r--r--   0        0        0     4193 2024-05-04 13:22:35.763487 languru-0.9.0/languru/prompts/base.py
+-rw-r--r--   0        0        0        0 2024-05-04 09:14:37.589501 languru-0.9.0/languru/prompts/repositories/__init__.py
+-rw-r--r--   0        0        0     2011 2024-05-04 10:07:15.715665 languru-0.9.0/languru/prompts/repositories/data_model.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:10:03.421778 languru-0.9.0/languru/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:19:09.963208 languru-0.9.0/languru/resources/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:18:35.609130 languru-0.9.0/languru/resources/model/__init__.py
+-rw-r--r--   0        0        0     4394 2024-03-26 14:02:44.551182 languru-0.9.0/languru/resources/model/discovery.py
+-rw-r--r--   0        0        0        0 2024-01-29 14:28:54.637050 languru-0.9.0/languru/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 14:35:12.034189 languru-0.9.0/languru/server/api/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-02 15:41:44.495640 languru-0.9.0/languru/server/api/v1/__init__.py
+-rw-r--r--   0        0        0    13646 2024-05-04 03:31:50.094299 languru-0.9.0/languru/server/api/v1/audio.py
+-rw-r--r--   0        0        0     7533 2024-03-26 14:02:44.552014 languru-0.9.0/languru/server/api/v1/chat.py
+-rw-r--r--   0        0        0     5796 2024-03-26 14:02:44.552963 languru-0.9.0/languru/server/api/v1/completions.py
+-rw-r--r--   0        0        0     4423 2024-03-26 14:02:44.553833 languru-0.9.0/languru/server/api/v1/embeddings.py
+-rw-r--r--   0        0        0    12851 2024-05-04 03:31:50.094535 languru-0.9.0/languru/server/api/v1/images.py
+-rw-r--r--   0        0        0     9679 2024-03-26 14:02:44.554362 languru-0.9.0/languru/server/api/v1/model.py
+-rw-r--r--   0        0        0     4353 2024-03-26 14:02:44.555146 languru-0.9.0/languru/server/api/v1/moderations.py
+-rw-r--r--   0        0        0     5950 2024-05-04 03:31:50.095290 languru-0.9.0/languru/server/api/v1/test_audio.py
+-rw-r--r--   0        0        0     5020 2024-03-26 14:02:44.555947 languru-0.9.0/languru/server/api/v1/test_chat.py
+-rw-r--r--   0        0        0     4807 2024-03-26 14:02:44.556765 languru-0.9.0/languru/server/api/v1/test_completions.py
+-rw-r--r--   0        0        0     2475 2024-03-26 14:02:44.557059 languru-0.9.0/languru/server/api/v1/test_embeddings.py
+-rw-r--r--   0        0        0     6347 2024-05-04 03:31:50.095871 languru-0.9.0/languru/server/api/v1/test_images.py
+-rw-r--r--   0        0        0     3501 2024-03-26 14:02:44.557249 languru-0.9.0/languru/server/api/v1/test_model.py
+-rw-r--r--   0        0        0     2263 2024-03-26 14:02:44.557524 languru-0.9.0/languru/server/api/v1/test_moderations.py
+-rw-r--r--   0        0        0     6958 2024-03-26 14:02:44.558328 languru-0.9.0/languru/server/config.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.558372 languru-0.9.0/languru/server/deps/__init__.py
+-rw-r--r--   0        0        0      429 2024-03-26 14:02:44.558691 languru-0.9.0/languru/server/deps/common.py
+-rw-r--r--   0        0        0     5166 2024-03-26 14:02:44.559416 languru-0.9.0/languru/server/main.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.559457 languru-0.9.0/languru/server/utils/__init__.py
+-rw-r--r--   0        0        0     1270 2024-03-26 14:02:44.559762 languru-0.9.0/languru/server/utils/common.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:58:36.094265 languru-0.9.0/languru/types/__init__.py
+-rw-r--r--   0        0        0     7400 2024-05-02 15:41:44.498794 languru-0.9.0/languru/types/audio.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:59:16.654501 languru-0.9.0/languru/types/chat/__init__.py
+-rw-r--r--   0        0        0     2059 2024-04-06 07:12:32.577046 languru-0.9.0/languru/types/chat/anthropic.py
+-rw-r--r--   0        0        0     3094 2024-04-06 05:54:42.711490 languru-0.9.0/languru/types/chat/completions.py
+-rw-r--r--   0        0        0     2895 2024-03-26 14:02:44.560212 languru-0.9.0/languru/types/completions.py
+-rw-r--r--   0        0        0      603 2024-02-09 09:22:56.989013 languru-0.9.0/languru/types/embeddings.py
+-rw-r--r--   0        0        0     7693 2024-05-02 15:41:44.499621 languru-0.9.0/languru/types/images.py
+-rw-r--r--   0        0        0      158 2024-02-07 11:22:07.653430 languru-0.9.0/languru/types/model/__init__.py
+-rw-r--r--   0        0        0      454 2024-02-07 11:22:07.653586 languru-0.9.0/languru/types/model/orm.py
+-rw-r--r--   0        0        0      403 2024-02-10 12:09:30.949805 languru-0.9.0/languru/types/moderations.py
+-rw-r--r--   0        0        0        0 2024-02-13 08:54:51.563321 languru-0.9.0/languru/utils/__init__.py
+-rw-r--r--   0        0        0     1622 2024-02-18 07:12:00.382248 languru-0.9.0/languru/utils/calculation.py
+-rw-r--r--   0        0        0     5480 2024-05-04 13:46:48.528178 languru-0.9.0/languru/utils/common.py
+-rw-r--r--   0        0        0     2328 2024-03-06 14:06:53.434085 languru-0.9.0/languru/utils/device.py
+-rw-r--r--   0        0        0     3213 2024-03-26 14:02:44.560917 languru-0.9.0/languru/utils/hf.py
+-rw-r--r--   0        0        0     1666 2024-03-26 14:02:44.561210 languru-0.9.0/languru/utils/http.py
+-rw-r--r--   0        0        0     1163 2024-02-13 12:38:09.199703 languru-0.9.0/languru/utils/socket.py
+-rw-r--r--   0        0        0     2854 2024-04-06 04:19:40.336504 languru-0.9.0/languru/utils/xml.py
+-rw-r--r--   0        0        0       63 2024-05-04 14:06:16.013025 languru-0.9.0/languru/version.py
+-rw-r--r--   0        0        0     4467 2024-05-04 14:06:05.084081 languru-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13410 1970-01-01 00:00:00.000000 languru-0.9.0/PKG-INFO
```

### Comparing `languru-0.8.0/LICENSE` & `languru-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/README.md` & `languru-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Languru
 
 The general-purpose LLM app stacks deploy AI services quickly and (stupidly) simply.
 
+```txt
+ _
+| |    __ _ _ __   __ _ _   _ _ __ _   _
+| |   / _` | '_ \ / _` | | | | '__| | | |
+| |__| (_| | | | | (_| | |_| | |  | |_| |
+|_____\__,_|_| |_|\__, |\__,_|_|   \__,_|
+                  |___/
+```
+
 [![image](https://img.shields.io/pypi/v/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/l/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/pyversions/languru.svg)](https://pypi.python.org/pypi/languru)
 [![PytestCI](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml)
 [![codecov](https://codecov.io/gh/dockhardman/languru/graph/badge.svg?token=OFX6C8Z31C)](https://codecov.io/gh/dockhardman/languru)
 
 Documentation: [Github Pages](https://dockhardman.github.io/languru/)
```

### Comparing `languru-0.8.0/languru/action/anthropic.py` & `languru-0.9.0/languru/action/anthropic.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/base.py` & `languru-0.9.0/languru/action/base.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/google.py` & `languru-0.9.0/languru/action/google.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/groq.py` & `languru-0.9.0/languru/action/groq.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/hf.py` & `languru-0.9.0/languru/action/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/openai.py` & `languru-0.9.0/languru/action/openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/pplx.py` & `languru-0.9.0/languru/action/pplx.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/action/utils.py` & `languru-0.9.0/languru/action/utils.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/cli/main.py` & `languru-0.9.0/languru/cli/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/examples/return_values/_openai.py` & `languru-0.9.0/languru/examples/return_values/_openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/resources/model/discovery.py` & `languru-0.9.0/languru/resources/model/discovery.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/__init__.py` & `languru-0.9.0/languru/server/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/audio.py` & `languru-0.9.0/languru/server/api/v1/audio.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/chat.py` & `languru-0.9.0/languru/server/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/completions.py` & `languru-0.9.0/languru/server/api/v1/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/embeddings.py` & `languru-0.9.0/languru/server/api/v1/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/images.py` & `languru-0.9.0/languru/server/api/v1/images.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/model.py` & `languru-0.9.0/languru/server/api/v1/model.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/moderations.py` & `languru-0.9.0/languru/server/api/v1/moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_audio.py` & `languru-0.9.0/languru/server/api/v1/test_audio.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_chat.py` & `languru-0.9.0/languru/server/api/v1/test_chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_completions.py` & `languru-0.9.0/languru/server/api/v1/test_completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_embeddings.py` & `languru-0.9.0/languru/server/api/v1/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_images.py` & `languru-0.9.0/languru/server/api/v1/test_images.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_model.py` & `languru-0.9.0/languru/server/api/v1/test_model.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/api/v1/test_moderations.py` & `languru-0.9.0/languru/server/api/v1/test_moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/config.py` & `languru-0.9.0/languru/server/config.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/main.py` & `languru-0.9.0/languru/server/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/server/utils/common.py` & `languru-0.9.0/languru/server/utils/common.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/audio.py` & `languru-0.9.0/languru/types/audio.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/chat/anthropic.py` & `languru-0.9.0/languru/types/chat/anthropic.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/chat/completions.py` & `languru-0.9.0/languru/types/chat/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/completions.py` & `languru-0.9.0/languru/types/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/embeddings.py` & `languru-0.9.0/languru/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/types/images.py` & `languru-0.9.0/languru/types/images.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/calculation.py` & `languru-0.9.0/languru/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/device.py` & `languru-0.9.0/languru/utils/device.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/hf.py` & `languru-0.9.0/languru/utils/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/http.py` & `languru-0.9.0/languru/utils/http.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/socket.py` & `languru-0.9.0/languru/utils/socket.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/languru/utils/xml.py` & `languru-0.9.0/languru/utils/xml.py`

 * *Files identical despite different names*

### Comparing `languru-0.8.0/pyproject.toml` & `languru-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,38 @@
 description = "The general purpose LLM app stacks."
 documentation = "https://dockhardman.github.io/languru/"
 homepage = "https://github.com/dockhardman/languru"
 license = "Apache-2.0 license"
 name = "languru"
 readme = "README.md"
 repository = "https://github.com/dockhardman/languru"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 accelerate = { version = "^0.27.2", optional = true, markers = "sys_platform == 'linux'" }
 aiohttp = "^3.9.3"
 anthropic = { version = "<1,>0.21", optional = true }
 bitsandbytes = { version = "^0.42", optional = true, markers = "sys_platform == 'linux'" }
 click = "^8.1.7"
 colorama = "^0.4.6"
 einops = { version = "^0.7.0", optional = true }
+email-validator = "^2"
 fastapi = { extras = ["all"], version = "^0.109.0", optional = true }
 flash-attn = { version = "^2", optional = true, markers = "sys_platform == 'linux'" }
 google-cloud-aiplatform = { version = "^1.38", optional = true }
 google-generativeai = { version = "^0.3.2", optional = true }
 groq = { version = "<1,>=0.4.2", optional = true }
 ninja = { version = "^1.11.1.1", optional = true }
 nvgpu = { version = "^0.10.0", optional = true, markers = "sys_platform == 'linux'" }
 openai = "^1.10.0"
 packaging = "^23.2"
-pyassorted = "^0.8.0"
+pyassorted = "^0.9.0"
 pydantic = "^2"
 pydantic-settings = "^2"
+pyjson5 = "^1.6"
 python = ">=3.10,<4.0"
 python-dotenv = "^1"
 pytz = "^2024.1"
 rich = "^13.7.0"
 sentencepiece = { version = "^0.1.99", optional = true }
 sqlalchemy = "^2.0.25"
 torch = { version = "^2.2.0", optional = true }
```

### Comparing `languru-0.8.0/PKG-INFO` & `languru-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languru
-Version: 0.8.0
+Version: 0.9.0
 Summary: The general purpose LLM app stacks.
 Home-page: https://github.com/dockhardman/languru
 License: Apache-2.0 license
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -24,26 +24,28 @@
 Requires-Dist: accelerate (>=0.27.2,<0.28.0) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: anthropic (>0.21,<1) ; extra == "all" or extra == "anthropic"
 Requires-Dist: bitsandbytes (>=0.42,<0.43) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0) ; extra == "all" or extra == "huggingface"
+Requires-Dist: email-validator (>=2,<3)
 Requires-Dist: fastapi[all] (>=0.109.0,<0.110.0) ; extra == "all" or extra == "server"
 Requires-Dist: flash-attn (>=2,<3) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: google-cloud-aiplatform (>=1.38,<2.0) ; extra == "all" or extra == "google"
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0) ; extra == "all" or extra == "google"
 Requires-Dist: groq (>=0.4.2,<1) ; extra == "all" or extra == "groq"
 Requires-Dist: ninja (>=1.11.1.1,<2.0.0.0) ; extra == "all" or extra == "huggingface"
 Requires-Dist: nvgpu (>=0.10.0,<0.11.0) ; (sys_platform == "linux") and (extra == "all" or extra == "cuda" or extra == "huggingface")
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: packaging (>=23.2,<24.0)
-Requires-Dist: pyassorted (>=0.8.0,<0.9.0)
+Requires-Dist: pyassorted (>=0.9.0,<0.10.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pydantic-settings (>=2,<3)
+Requires-Dist: pyjson5 (>=1.6,<2.0)
 Requires-Dist: python-dotenv (>=1,<2)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0) ; extra == "all" or extra == "huggingface"
 Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
 Requires-Dist: torch (>=2.2.0,<3.0.0) ; extra == "all" or extra == "huggingface" or extra == "torch"
 Requires-Dist: torchaudio (>=2.2.0,<3.0.0) ; extra == "all" or extra == "huggingface" or extra == "torch"
@@ -54,14 +56,23 @@
 Project-URL: Repository, https://github.com/dockhardman/languru
 Description-Content-Type: text/markdown
 
 # Languru
 
 The general-purpose LLM app stacks deploy AI services quickly and (stupidly) simply.
 
+```txt
+ _
+| |    __ _ _ __   __ _ _   _ _ __ _   _
+| |   / _` | '_ \ / _` | | | | '__| | | |
+| |__| (_| | | | | (_| | |_| | |  | |_| |
+|_____\__,_|_| |_|\__, |\__,_|_|   \__,_|
+                  |___/
+```
+
 [![image](https://img.shields.io/pypi/v/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/l/languru.svg)](https://pypi.python.org/pypi/languru)
 [![image](https://img.shields.io/pypi/pyversions/languru.svg)](https://pypi.python.org/pypi/languru)
 [![PytestCI](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/dockhardman/languru/actions/workflows/python-pytest.yml)
 [![codecov](https://codecov.io/gh/dockhardman/languru/graph/badge.svg?token=OFX6C8Z31C)](https://codecov.io/gh/dockhardman/languru)
 
 Documentation: [Github Pages](https://dockhardman.github.io/languru/)
```

