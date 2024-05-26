# Comparing `tmp/doveseed-2.0.3.tar.gz` & `tmp/doveseed-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-2.0.3.tar", max compression
+gzip compressed data, was "doveseed-2.0.4.tar", max compression
```

## Comparing `doveseed-2.0.3.tar` & `doveseed-2.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2024-02-17 18:32:49.348151 doveseed-2.0.3/LICENSE
--rw-r--r--   0        0        0     6578 2024-02-17 18:32:49.348151 doveseed-2.0.3/README.rst
--rw-r--r--   0        0        0       22 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/__init__.py
--rw-r--r--   0        0        0     5806 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/app.py
--rw-r--r--   0        0        0     2163 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/cli.py
--rw-r--r--   0        0        0      705 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/config.py
--rw-r--r--   0        0        0      924 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/domain_types.py
--rw-r--r--   0        0        0     1126 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/feed.py
--rw-r--r--   0        0        0     1263 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/notifier.py
--rw-r--r--   0        0        0     2112 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3811 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/storage.py
--rw-r--r--   0        0        0      121 2024-02-17 18:32:49.348151 doveseed-2.0.3/doveseed/token_gen.py
--rw-r--r--   0        0        0     1273 2024-02-17 18:32:49.348151 doveseed-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     8015 1970-01-01 00:00:00.000000 doveseed-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 19:11:43.803603 doveseed-2.0.4/LICENSE
+-rw-r--r--   0        0        0     6578 2024-05-26 19:11:43.803603 doveseed-2.0.4/README.rst
+-rw-r--r--   0        0        0       22 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/__init__.py
+-rw-r--r--   0        0        0     5806 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/cli.py
+-rw-r--r--   0        0        0      705 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/config.py
+-rw-r--r--   0        0        0      924 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1126 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/feed.py
+-rw-r--r--   0        0        0     1263 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/notifier.py
+-rw-r--r--   0        0        0     2112 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3811 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2024-05-26 19:11:43.807603 doveseed-2.0.4/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1275 2024-05-26 19:11:43.807603 doveseed-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8015 1970-01-01 00:00:00.000000 doveseed-2.0.4/PKG-INFO
```

### Comparing `doveseed-2.0.3/LICENSE` & `doveseed-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/README.rst` & `doveseed-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/app.py` & `doveseed-2.0.4/doveseed/app.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/cli.py` & `doveseed-2.0.4/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/config.py` & `doveseed-2.0.4/doveseed/config.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/confirmation.py` & `doveseed-2.0.4/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/domain_types.py` & `doveseed-2.0.4/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/email_notification.py` & `doveseed-2.0.4/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/email_templating.py` & `doveseed-2.0.4/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/feed.py` & `doveseed-2.0.4/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/notifier.py` & `doveseed-2.0.4/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/recaptcha.py` & `doveseed-2.0.4/doveseed/recaptcha.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/registration.py` & `doveseed-2.0.4/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/smtp.py` & `doveseed-2.0.4/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/doveseed/storage.py` & `doveseed-2.0.4/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.3/pyproject.toml` & `doveseed-2.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "2.0.3" # Also update in doveseed/__init__.py
+version = "2.0.4" # Also update in doveseed/__init__.py
 
 [tool.poetry.dependencies]
 aiohttp = {version = "^3.8.4", optional = true}
-fastapi = "^0.109.2"
+fastapi = "^0.111.0"
 jinja2 = "^3.1.2"
 pydantic-settings = "^2.2.0"
 python = "^3.9.0"
-starlette = {version = "0.36.3", optional = true}
+starlette = {version = "0.37.2", optional = true}
 tinydb = "^4.7.0"
 typing_extensions = "^4.3.0"
 
 [tool.poetry.extras]
 all = ["aiohttp", "starlette"]
 recaptcha = ["aiohttp", "starlette"]
 
 [tool.poetry.group.dev.dependencies]
-black = "24.2.0"
-httpx = "^0.26.0"
+black = ">=24.3.0"
+httpx = "^0.27.0"
 mypy = "^1.8.0"
 pylint = "^3.0.3"
 pytest = "^8.0.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-emoji = "^0.2.0"
 pytest-mypy = "^0.10.0"
-uvicorn = "^0.27.1"
+uvicorn = "^0.29.0"
 
 [build-system]
 build-backend = "poetry.masonry.api"
 requires = ["poetry>=0.12"]
```

### Comparing `doveseed-2.0.3/PKG-INFO` & `doveseed-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 2.0.3
+Version: 2.0.4
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -19,18 +19,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: all
 Provides-Extra: recaptcha
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "all" or extra == "recaptcha"
-Requires-Dist: fastapi (>=0.109.2,<0.110.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic-settings (>=2.2.0,<3.0.0)
-Requires-Dist: starlette (==0.36.3) ; extra == "all" or extra == "recaptcha"
+Requires-Dist: starlette (==0.37.2) ; extra == "all" or extra == "recaptcha"
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Repository, https://github.com/jgosmann/doveseed/
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/jgosmann/doveseed/actions/workflows/ci.yml/badge.svg
   :target: https://github.com/jgosmann/doveseed/actions/workflows/ci.yml
```

