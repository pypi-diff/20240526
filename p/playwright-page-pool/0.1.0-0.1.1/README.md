# Comparing `tmp/playwright_page_pool-0.1.0.tar.gz` & `tmp/playwright_page_pool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_page_pool-0.1.0.tar", max compression
+gzip compressed data, was "playwright_page_pool-0.1.1.tar", max compression
```

## Comparing `playwright_page_pool-0.1.0.tar` & `playwright_page_pool-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.0/LICENSE
--rw-r--r--   0        0        0     3786 2024-05-26 13:34:13.045007 playwright_page_pool-0.1.0/README.md
--rw-r--r--   0        0        0       44 2024-05-26 13:18:10.499859 playwright_page_pool-0.1.0/playwright_page_pool/__init__.py
--rw-r--r--   0        0        0     4292 2024-05-26 13:18:10.500179 playwright_page_pool-0.1.0/playwright_page_pool/page_pool.py
--rw-r--r--   0        0        0      879 2024-05-26 13:18:10.492501 playwright_page_pool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-26 11:31:26.371890 playwright_page_pool-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3786 2024-05-26 14:44:02.032762 playwright_page_pool-0.1.1/README.md
+-rw-r--r--   0        0        0       44 2024-05-26 14:43:52.481726 playwright_page_pool-0.1.1/playwright_page_pool/__init__.py
+-rw-r--r--   0        0        0     4292 2024-05-26 14:43:52.481964 playwright_page_pool-0.1.1/playwright_page_pool/page_pool.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:00:17.715334 playwright_page_pool-0.1.1/playwright_page_pool/py.typed
+-rw-r--r--   0        0        0      879 2024-05-26 15:00:07.442946 playwright_page_pool-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 playwright_page_pool-0.1.1/PKG-INFO
```

### Comparing `playwright_page_pool-0.1.0/LICENSE` & `playwright_page_pool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.0/README.md` & `playwright_page_pool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.0/playwright_page_pool/page_pool.py` & `playwright_page_pool-0.1.1/playwright_page_pool/page_pool.py`

 * *Files identical despite different names*

### Comparing `playwright_page_pool-0.1.0/pyproject.toml` & `playwright_page_pool-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "playwright-page-pool"
-version = "0.1.0"
+version = "0.1.1"
 description = "A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool."
 authors = ["YeonGyu-Kim <code.yeon.gyu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `playwright_page_pool-0.1.0/PKG-INFO` & `playwright_page_pool-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-page-pool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A utility for managing Playwright browser pages in a pool, inspired by Python's ThreadPool.
 License: MIT
 Author: YeonGyu-Kim
 Author-email: code.yeon.gyu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

