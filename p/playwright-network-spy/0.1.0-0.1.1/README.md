# Comparing `tmp/playwright_network_spy-0.1.0.tar.gz` & `tmp/playwright_network_spy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_network_spy-0.1.0.tar", max compression
+gzip compressed data, was "playwright_network_spy-0.1.1.tar", max compression
```

## Comparing `playwright_network_spy-0.1.0.tar` & `playwright_network_spy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-26 13:44:37.188146 playwright_network_spy-0.1.0/LICENSE
--rw-r--r--   0        0        0     3076 2024-05-26 14:56:30.202293 playwright_network_spy-0.1.0/README.md
--rw-r--r--   0        0        0      116 2024-05-26 14:43:03.750400 playwright_network_spy-0.1.0/playwright_network_spy/__init__.py
--rw-r--r--   0        0        0     5214 2024-05-26 14:43:03.750640 playwright_network_spy-0.1.0/playwright_network_spy/spy.py
--rw-r--r--   0        0        0      887 2024-05-26 14:43:03.743875 playwright_network_spy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 playwright_network_spy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 13:44:37.188146 playwright_network_spy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3076 2024-05-26 14:56:30.202293 playwright_network_spy-0.1.1/README.md
+-rw-r--r--   0        0        0      116 2024-05-26 14:43:03.750400 playwright_network_spy-0.1.1/playwright_network_spy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:01:59.713932 playwright_network_spy-0.1.1/playwright_network_spy/py.typed
+-rw-r--r--   0        0        0     5214 2024-05-26 14:43:03.750640 playwright_network_spy-0.1.1/playwright_network_spy/spy.py
+-rw-r--r--   0        0        0      887 2024-05-26 15:02:19.615604 playwright_network_spy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 playwright_network_spy-0.1.1/PKG-INFO
```

### Comparing `playwright_network_spy-0.1.0/LICENSE` & `playwright_network_spy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_network_spy-0.1.0/README.md` & `playwright_network_spy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `playwright_network_spy-0.1.0/playwright_network_spy/spy.py` & `playwright_network_spy-0.1.1/playwright_network_spy/spy.py`

 * *Files identical despite different names*

### Comparing `playwright_network_spy-0.1.0/pyproject.toml` & `playwright_network_spy-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "playwright-network-spy"
-version = "0.1.0"
+version = "0.1.1"
 description = "🔥 A powerful tool for crawling any website on Earth with infinite scrolling, using Playwright."
 authors = ["YeonGyu-Kim <code.yeon.gyu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `playwright_network_spy-0.1.0/PKG-INFO` & `playwright_network_spy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-network-spy
-Version: 0.1.0
+Version: 0.1.1
 Summary: 🔥 A powerful tool for crawling any website on Earth with infinite scrolling, using Playwright.
 License: MIT
 Author: YeonGyu-Kim
 Author-email: code.yeon.gyu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

