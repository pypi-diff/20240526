# Comparing `tmp/duckduckgo_search-6.1.0.tar.gz` & `tmp/duckduckgo_search-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-6.1.0.tar", last modified: Wed May 15 13:45:36 2024, max compression
+gzip compressed data, was "duckduckgo_search-6.1.1.tar", last modified: Sat May 25 22:49:04 2024, max compression
```

## Comparing `duckduckgo_search-6.1.0.tar` & `duckduckgo_search-6.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:45:36.213081 duckduckgo_search-6.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-05-15 13:45:36.213081 duckduckgo_search-6.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    17333 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:45:36.209081 duckduckgo_search-6.1.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    42475 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:45:36.213081 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 13:45:36.000000 duckduckgo_search-6.1.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:45:36.213081 duckduckgo_search-6.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:45:36.213081 duckduckgo_search-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/tests/test_duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-15 13:45:23.000000 duckduckgo_search-6.1.0/tests/test_duckduckgo_search_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:04.115534 duckduckgo_search-6.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-25 22:49:04.115534 duckduckgo_search-6.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17488 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:04.111534 duckduckgo_search-6.1.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42430 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:04.111534 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 22:49:04.000000 duckduckgo_search-6.1.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:49:04.115534 duckduckgo_search-6.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:49:04.111534 duckduckgo_search-6.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/tests/test_duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-25 22:48:53.000000 duckduckgo_search-6.1.1/tests/test_duckduckgo_search_async.py
```

### Comparing `duckduckgo_search-6.1.0/LICENSE.md` & `duckduckgo_search-6.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/PKG-INFO` & `duckduckgo_search-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.0
+Version: 6.1.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -79,21 +79,23 @@
 ```
 
 CLI examples:
 ```python3
 # AI chat
 ddgs chat
 # text search
-ddgs text -k "axon regeneration"
+ddgs text -k "'how to tame a fox' site:wikihow.com"
 # find and download pdf files via proxy (example: Tor browser)
-ddgs text -k "neuroscience filetype:pdf" -r wt-wt -m 50 -d -p socks5://localhost:9150
+ddgs text -k "pushkin filetype:pdf" -r wt-wt -m 50 -d -p socks5://127.0.0.1:9150
+# find and save to csv
+ddgs text -k "neuroscience exploring the brain fourth edition filetype:pdf" -m 70 -o csv
 # find and download images
-ddgs images -k "gaz 14 chaika" -r ru-ru -type photo -m 500 -d
-# get latest news and save to csv
-ddgs news -k "hubble telescope" -m 50 -o csv
+ddgs images -k "you can run but you can't hide" -r wt-wt -type photo -m 500 -d
+# get news for the last day and save to json
+ddgs news -k "ukraine war" -m 50 -t d -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -236,15 +238,15 @@
 ## Proxy
 
 Package supports http/https/socks proxies. Example: `http://user:pass@example.com:3128`.
 Use a rotating proxy. Otherwise, use a new proxy with each DDGS or AsyncDDGS initialization.
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
-ddgs = DDGS(proxy="socks5://localhost:9150", timeout=20)
+ddgs = DDGS(proxy="socks5://127.0.0.1:9150", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
 *2. Use any proxy server* (*example with [iproyal rotating residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 ddgs = DDGS(proxy="socks5://user:password@geo.iproyal.com:32325", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
```

### Comparing `duckduckgo_search-6.1.0/README.md` & `duckduckgo_search-6.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,23 @@
 ```
 
 CLI examples:
 ```python3
 # AI chat
 ddgs chat
 # text search
-ddgs text -k "axon regeneration"
+ddgs text -k "'how to tame a fox' site:wikihow.com"
 # find and download pdf files via proxy (example: Tor browser)
-ddgs text -k "neuroscience filetype:pdf" -r wt-wt -m 50 -d -p socks5://localhost:9150
+ddgs text -k "pushkin filetype:pdf" -r wt-wt -m 50 -d -p socks5://127.0.0.1:9150
+# find and save to csv
+ddgs text -k "neuroscience exploring the brain fourth edition filetype:pdf" -m 70 -o csv
 # find and download images
-ddgs images -k "gaz 14 chaika" -r ru-ru -type photo -m 500 -d
-# get latest news and save to csv
-ddgs news -k "hubble telescope" -m 50 -o csv
+ddgs images -k "you can run but you can't hide" -r wt-wt -type photo -m 500 -d
+# get news for the last day and save to json
+ddgs news -k "ukraine war" -m 50 -t d -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -201,15 +203,15 @@
 ## Proxy
 
 Package supports http/https/socks proxies. Example: `http://user:pass@example.com:3128`.
 Use a rotating proxy. Otherwise, use a new proxy with each DDGS or AsyncDDGS initialization.
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
-ddgs = DDGS(proxy="socks5://localhost:9150", timeout=20)
+ddgs = DDGS(proxy="socks5://127.0.0.1:9150", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
 *2. Use any proxy server* (*example with [iproyal rotating residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 ddgs = DDGS(proxy="socks5://user:password@geo.iproyal.com:32325", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
```

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search/__init__.py` & `duckduckgo_search-6.1.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search/cli.py` & `duckduckgo_search-6.1.1/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-6.1.1/duckduckgo_search/duckduckgo_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         if LXML_AVAILABLE is False and backend != "api":
             backend = "api"
             warnings.warn("lxml is not installed. Using backend='api'.", stacklevel=2)
 
         if backend == "api":
             results = self._text_api(keywords, region, safesearch, timelimit, max_results)
         elif backend == "html":
-            results = self._text_html(keywords, region, safesearch, timelimit, max_results)
+            results = self._text_html(keywords, region, timelimit, max_results)
         elif backend == "lite":
             results = self._text_lite(keywords, region, timelimit, max_results)
         return results
 
     def _text_api(
         self,
         keywords: str,
@@ -233,14 +233,15 @@
             "q": keywords,
             "kl": region,
             "l": region,
             "p": "",
             "s": "0",
             "df": "",
             "vqd": vqd,
+            "bing_market": region,
             "ex": "",
         }
         safesearch = safesearch.lower()
         if safesearch == "moderate":
             payload["ex"] = "-1"
         elif safesearch == "off":
             payload["ex"] = "-2"
@@ -283,44 +284,43 @@
 
         return list(islice(results, max_results))
 
     def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
-        safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
         """DuckDuckGo text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
-            safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "q": keywords,
-            "kl": region,
-            "p": safesearch_base[safesearch.lower()],
+            "s": "0",
             "o": "json",
             "api": "d.js",
+            "vqd": "",
+            "kl": region,
+            "bing_market": region,
         }
         if timelimit:
             payload["df"] = timelimit
         if max_results and max_results > 20:
             vqd = self._get_vqd(keywords)
             payload["vqd"] = vqd
 
@@ -397,17 +397,20 @@
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
+            "s": "0",
             "o": "json",
             "api": "d.js",
+            "vqd": "",
             "kl": region,
+            "bing_market": region,
         }
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
         results: List[Dict[str, str]] = []
```

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-6.1.1/duckduckgo_search/duckduckgo_search_async.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search/utils.py` & `duckduckgo_search-6.1.1/duckduckgo_search/utils.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-6.1.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.0
+Version: 6.1.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -79,21 +79,23 @@
 ```
 
 CLI examples:
 ```python3
 # AI chat
 ddgs chat
 # text search
-ddgs text -k "axon regeneration"
+ddgs text -k "'how to tame a fox' site:wikihow.com"
 # find and download pdf files via proxy (example: Tor browser)
-ddgs text -k "neuroscience filetype:pdf" -r wt-wt -m 50 -d -p socks5://localhost:9150
+ddgs text -k "pushkin filetype:pdf" -r wt-wt -m 50 -d -p socks5://127.0.0.1:9150
+# find and save to csv
+ddgs text -k "neuroscience exploring the brain fourth edition filetype:pdf" -m 70 -o csv
 # find and download images
-ddgs images -k "gaz 14 chaika" -r ru-ru -type photo -m 500 -d
-# get latest news and save to csv
-ddgs news -k "hubble telescope" -m 50 -o csv
+ddgs images -k "you can run but you can't hide" -r wt-wt -type photo -m 500 -d
+# get news for the last day and save to json
+ddgs news -k "ukraine war" -m 50 -t d -o json
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -236,15 +238,15 @@
 ## Proxy
 
 Package supports http/https/socks proxies. Example: `http://user:pass@example.com:3128`.
 Use a rotating proxy. Otherwise, use a new proxy with each DDGS or AsyncDDGS initialization.
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
-ddgs = DDGS(proxy="socks5://localhost:9150", timeout=20)
+ddgs = DDGS(proxy="socks5://127.0.0.1:9150", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
 *2. Use any proxy server* (*example with [iproyal rotating residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 ddgs = DDGS(proxy="socks5://user:password@geo.iproyal.com:32325", timeout=20)
 results = ddgs.text("something you need", max_results=50)
 ```
```

### Comparing `duckduckgo_search-6.1.0/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-6.1.1/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/pyproject.toml` & `duckduckgo_search-6.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/tests/test_cli.py` & `duckduckgo_search-6.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-6.1.1/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.0/tests/test_duckduckgo_search_async.py` & `duckduckgo_search-6.1.1/tests/test_duckduckgo_search_async.py`

 * *Files identical despite different names*

