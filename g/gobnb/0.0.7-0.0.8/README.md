# Comparing `tmp/gobnb-0.0.7.tar.gz` & `tmp/gobnb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gobnb-0.0.7.tar", last modified: Tue Apr 23 03:30:05 2024, max compression
+gzip compressed data, was "gobnb-0.0.8.tar", last modified: Sun May 26 21:34:10 2024, max compression
```

## Comparing `gobnb-0.0.7.tar` & `gobnb-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/
--rw-rw-r--   0 user      (1000) user      (1000)     1060 2024-03-27 06:52:07.000000 gobnb-0.0.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2239 2024-04-23 03:30:05.101741 gobnb-0.0.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1830 2024-03-27 06:52:07.000000 gobnb-0.0.7/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      315 2024-04-23 03:29:32.000000 gobnb-0.0.7/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-23 03:30:05.105741 gobnb-0.0.7/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      480 2024-03-27 07:16:39.000000 gobnb-0.0.7/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/gobnb/
--rw-rw-r--   0 user      (1000) user      (1000)      219 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1356 2024-04-23 03:27:28.000000 gobnb-0.0.7/src/gobnb/api.py
--rw-rw-r--   0 user      (1000) user      (1000)     2822 2024-03-27 06:58:14.000000 gobnb-0.0.7/src/gobnb/details.py
--rw-rw-r--   0 user      (1000) user      (1000)     1289 2024-03-27 07:10:44.000000 gobnb-0.0.7/src/gobnb/parse.py
--rw-rw-r--   0 user      (1000) user      (1000)     4363 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/price.py
--rw-rw-r--   0 user      (1000) user      (1000)     6127 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/search.py
--rw-rw-r--   0 user      (1000) user      (1000)    11241 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/standardize.py
--rw-rw-r--   0 user      (1000) user      (1000)      921 2024-03-27 06:52:07.000000 gobnb-0.0.7/src/gobnb/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-23 03:30:05.101741 gobnb-0.0.7/src/gobnb.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2239 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      367 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-04-23 03:30:05.000000 gobnb-0.0.7/src/gobnb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 21:34:10.137589 gobnb-0.0.8/
+-rw-rw-rw-   0        0        0     1080 2024-05-26 20:37:43.000000 gobnb-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2334 2024-05-26 21:34:10.136589 gobnb-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-05-26 21:32:40.000000 gobnb-0.0.8/README.md
+-rw-rw-rw-   0        0        0      341 2024-05-26 21:31:55.000000 gobnb-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 21:34:10.137589 gobnb-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      496 2024-05-26 20:37:43.000000 gobnb-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:34:10.126589 gobnb-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 21:34:10.132589 gobnb-0.0.8/src/gobnb/
+-rw-rw-rw-   0        0        0      223 2024-05-26 20:37:43.000000 gobnb-0.0.8/src/gobnb/__init__.py
+-rw-rw-rw-   0        0        0     1392 2024-05-26 20:37:43.000000 gobnb-0.0.8/src/gobnb/api.py
+-rw-rw-rw-   0        0        0     2875 2024-05-26 20:42:37.000000 gobnb-0.0.8/src/gobnb/details.py
+-rw-rw-rw-   0        0        0     1323 2024-05-26 20:37:43.000000 gobnb-0.0.8/src/gobnb/parse.py
+-rw-rw-rw-   0        0        0     4454 2024-05-26 20:37:43.000000 gobnb-0.0.8/src/gobnb/price.py
+-rw-rw-rw-   0        0        0     6357 2024-05-26 21:27:49.000000 gobnb-0.0.8/src/gobnb/search.py
+-rw-rw-rw-   0        0        0    11572 2024-05-26 21:30:35.000000 gobnb-0.0.8/src/gobnb/standardize.py
+-rw-rw-rw-   0        0        0      957 2024-05-26 20:37:43.000000 gobnb-0.0.8/src/gobnb/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:34:10.136589 gobnb-0.0.8/src/gobnb.egg-info/
+-rw-rw-rw-   0        0        0     2334 2024-05-26 21:34:10.000000 gobnb-0.0.8/src/gobnb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-05-26 21:34:10.000000 gobnb-0.0.8/src/gobnb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 21:34:10.000000 gobnb-0.0.8/src/gobnb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 21:34:10.000000 gobnb-0.0.8/src/gobnb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-26 21:34:10.000000 gobnb-0.0.8/src/gobnb.egg-info/top_level.txt
```

### Comparing `gobnb-0.0.7/README.md` & `gobnb-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,86 @@
-# Airbnb scraper in Python
-
-## Overview
-This project is an open-source tool developed in Python for extracting product information from Airbnb. It's designed to be easy to use, making it an ideal solution for developers looking for Airbnb product data.
-
-## Features
-- Full search support
-- Extracts detailed product information from Airbnb
-- Implemented in Python just because it's popular
-- Easy to integrate with existing Python projects
-- The code is optimize to work on this format: ```https://www.airbnb.com/rooms/[roomID]```
-
-### Install
-
-```bash
-$ pip install gobnb
-```
-## Examples
-
-```Python
-import gobnb
-import json
-currency="MXN"
-check_in = "2024-03-11"
-check_out = "2024-03-14"
-ne_lat = -1.1225978433925647
-ne_long = -77.59713412765507
-sw_lat = -1.03866277790021
-sw_long = -77.53091734683608
-zoom_value = 2
-results = gobnb.Search_all(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value, currency,"")
-details_data = []
-progress = 1
-jsondata = json.dumps(results)
-f = open("results.json", "w")
-f.write(jsondata)
-f.close()
-for result in results[:10]:
-    data = gobnb.Get_from_room_id(result["room_id"],currency,"")
-    details_data.append(data)
-    print("len results: ",progress, len(results))
-    progress=progress+1
-    
-details_data_json = json.dumps(details_data)
-f = open("details_data.json", "w")
-f.write(details_data_json)
-f.close()
-```
-
-```Python
-import gobnb
-import json
-room_url="https://www.airbnb.com/rooms/[room_id]"
-currency="USD"
-data = gobnb.Get_from_room_url(room_url,currency,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
-
-```Python
-import gobnb
-import json
-room_id=0#obviously the room id
-currency="MXN"
-data = gobnb.Get_from_room_id(room_id,currency,"")
-jsondata = json.dumps(data)
-f = open("details.json", "w")
-f.write(jsondata)
-f.close()
-```
+Metadata-Version: 2.1
+Name: gobnb
+Version: 0.0.8
+Summary: Airbnb scraper in Python
+Home-page: https://github.com/johnbalvin/pybnb
+Author: John (John Balvin)
+Author-email: John Balvin <johnchristian@hotmail.es>
+Project-URL: Homepage, https://github.com/johnbalvin/pybnb
+Keywords: airbnb,scraper,crawler,requests
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: curl_cffi
+Requires-Dist: bs4
+
+# Airbnb scraper in Python
+
+## Overview
+This project is an open-source tool developed in Python for extracting product information from Airbnb. It's designed to be easy to use, making it an ideal solution for developers looking for Airbnb product data.
+
+## Features
+- Full search support
+- Extracts detailed product information from Airbnb
+- Implemented in Python just because it's popular
+- Easy to integrate with existing Python projects
+- The code is optimize to work on this format: ```https://www.airbnb.com/rooms/[roomID]```
+
+### Install
+
+```bash
+$ pip install gobnb
+```
+## Examples
+
+```Python
+import gobnb
+import json
+currency="MXN"
+check_in = "2024-08-20"
+check_out = "2024-08-28"
+ne_lat = -1.03866277790021
+ne_long = -77.53091734683608
+sw_lat = -1.1225978433925647
+sw_long = -77.59713412765507
+zoom_value = 2
+results = gobnb.Search_all(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value, currency,"")
+details_data = []
+progress = 1
+jsondata = json.dumps(results)
+f = open("results.json", "w")
+f.write(jsondata)
+f.close()
+for result in results[:10]:
+    data = gobnb.Get_from_room_id(result["room_id"],currency,"")
+    details_data.append(data)
+    print("len results: ",progress, len(results))
+    progress=progress+1
+    
+details_data_json = json.dumps(details_data)
+f = open("details_data.json", "w")
+f.write(details_data_json)
+f.close()
+```
+
+```Python
+import gobnb
+import json
+room_url="https://www.airbnb.com/rooms/[room_id]"
+currency="USD"
+data = gobnb.Get_from_room_url(room_url,currency,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
+
+```Python
+import gobnb
+import json
+room_id=0#obviously the room id
+currency="MXN"
+data = gobnb.Get_from_room_id(room_id,currency,"")
+jsondata = json.dumps(data)
+f = open("details.json", "w")
+f.write(jsondata)
+f.close()
+```
```

### Comparing `gobnb-0.0.7/src/gobnb/api.py` & `gobnb-0.0.8/src/gobnb/api.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from curl_cffi import requests
-import re
-
-ep = "https://www.airbnb.com"
-
-regx_api_key = re.compile(r'"api_config":{"key":".+?"')
-
-def get(proxy_url: str) -> str:
-    headers = {
-        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-        "Accept-Language": "en",
-        "Cache-Control": "no-cache",
-        "Pragma": "no-cache",
-        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
-        "Sec-Ch-Ua-Mobile": "?0",
-        "Sec-Ch-Ua-Platform": '"Windows"',
-        "Sec-Fetch-Dest": "document",
-        "Sec-Fetch-Mode": "navigate",
-        "Sec-Fetch-Site": "none",
-        "Sec-Fetch-User": "?1",
-        "Upgrade-Insecure-Requests": "1",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
-    }
-    session = requests.Session()
-    session.headers.update(headers)
-    if proxy_url:
-        session.proxies.update({'http': proxy_url, 'https': proxy_url})
-
-    response = session.get(ep, timeout=60)  
-    response.raise_for_status() 
-
-    body = response.text
-    api_key = regx_api_key.search(body).group()
-    api_key = api_key.replace('"api_config":{"key":"', '')
-    api_key = api_key.replace('"', "")
-    return api_key
+from curl_cffi import requests
+import re
+
+ep = "https://www.airbnb.com"
+
+regx_api_key = re.compile(r'"api_config":{"key":".+?"')
+
+def get(proxy_url: str) -> str:
+    headers = {
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "Accept-Language": "en",
+        "Cache-Control": "no-cache",
+        "Pragma": "no-cache",
+        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
+        "Sec-Ch-Ua-Mobile": "?0",
+        "Sec-Ch-Ua-Platform": '"Windows"',
+        "Sec-Fetch-Dest": "document",
+        "Sec-Fetch-Mode": "navigate",
+        "Sec-Fetch-Site": "none",
+        "Sec-Fetch-User": "?1",
+        "Upgrade-Insecure-Requests": "1",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
+    }
+    session = requests.Session()
+    session.headers.update(headers)
+    if proxy_url:
+        session.proxies.update({'http': proxy_url, 'https': proxy_url})
+
+    response = session.get(ep, timeout=60)  
+    response.raise_for_status() 
+
+    body = response.text
+    api_key = regx_api_key.search(body).group()
+    api_key = api_key.replace('"api_config":{"key":"', '')
+    api_key = api_key.replace('"', "")
+    return api_key
```

### Comparing `gobnb-0.0.7/src/gobnb/details.py` & `gobnb-0.0.8/src/gobnb/details.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-from curl_cffi import requests
-from gobnb.parse import parse_body_details_wrapper
-from gobnb.price import get_price
-
-def Get_from_room_url(roomURL: str, currency: str, proxy_url: str):
-    data, price_input, cookies = get_from_room_url(roomURL, proxy_url)
-    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
-    data["price"] = {
-        "ammount":ammount,
-        "currency_symbol":currency,
-        "qualifier": qualifier
-    }
-    return data
-
-def Get_from_room_id(room_id: int, currency: str, proxy_url: str):
-    room_url = f"https://www.airbnb.com/rooms/{room_id}"
-    data, price_input, cookies = get_from_room_url(room_url, proxy_url)
-    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
-    data["price"] = {
-        "ammount":ammount,
-        "currency_symbol":currency,
-        "qualifier": qualifier
-    }
-    return data
-
-def Get_from_room_id_and_domain(room_id: int, domain: str, currency: str, proxy_url: str):
-    room_url = f"https://{domain}/rooms/{room_id}"
-    data, price_input, cookies = get_from_room_url(room_url, proxy_url)
-    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
-    data["price"] = {
-        "ammount":ammount,
-        "currency_symbol":currency,
-        "qualifier": qualifier
-    }
-    return data
-
-
-def get_from_room_url(room_url: str, proxy_url: str):
-    headers = {
-        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-        "Accept-Language": "en",
-        "Cache-Control": "no-cache",
-        "Pragma": "no-cache",
-        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
-        "Sec-Ch-Ua-Mobile": "?0",
-        "Sec-Ch-Ua-Platform": '"Windows"',
-        "Sec-Fetch-Dest": "document",
-        "Sec-Fetch-Mode": "navigate",
-        "Sec-Fetch-Site": "none",
-        "Sec-Fetch-User": "?1",
-        "Upgrade-Insecure-Requests": "1",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
-    }
-    proxies = {}
-    if proxy_url:
-        parsed_proxy_url = reque
-        sts.utils.requote_uri(proxy_url)
-        proxies = {"http": parsed_proxy_url, "https": parsed_proxy_url}
-    response = requests.get(room_url, headers=headers, proxies=proxies)
-    response.raise_for_status()
-    data_formatted, price_dependency_input=parse_body_details_wrapper(response.text)
-    cookies = response.cookies
-    return data_formatted, price_dependency_input, cookies
+from curl_cffi import requests
+from gobnb.parse import parse_body_details_wrapper
+from gobnb.price import get_price
+
+def Get_from_room_url(roomURL: str, currency: str, proxy_url: str):
+    data, price_input, cookies = get_from_room_url(roomURL, proxy_url)
+    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
+    data["price"] = {
+        "ammount":ammount,
+        "currency_symbol":currency,
+        "qualifier": qualifier
+    }
+    return data
+
+def Get_from_room_id(room_id: int, currency: str, proxy_url: str):
+    room_url = f"https://www.airbnb.com/rooms/{room_id}"
+    data, price_input, cookies = get_from_room_url(room_url, proxy_url)
+    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
+    data["price"] = {
+        "ammount":ammount,
+        "currency_symbol":currency,
+        "qualifier": qualifier
+    }
+    return data
+
+def Get_from_room_id_and_domain(room_id: int, domain: str, currency: str, proxy_url: str):
+    room_url = f"https://{domain}/rooms/{room_id}"
+    data, price_input, cookies = get_from_room_url(room_url, proxy_url)
+    ammount, currency, qualifier = get_price(price_input["product_id"],price_input["impression_id"],price_input["api_key"],currency, cookies, proxy_url)
+    data["price"] = {
+        "ammount":ammount,
+        "currency_symbol":currency,
+        "qualifier": qualifier
+    }
+    return data
+
+
+def get_from_room_url(room_url: str, proxy_url: str):
+    headers = {
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "Accept-Language": "en",
+        "Cache-Control": "no-cache",
+        "Pragma": "no-cache",
+        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
+        "Sec-Ch-Ua-Mobile": "?0",
+        "Sec-Ch-Ua-Platform": '"Windows"',
+        "Sec-Fetch-Dest": "document",
+        "Sec-Fetch-Mode": "navigate",
+        "Sec-Fetch-Site": "none",
+        "Sec-Fetch-User": "?1",
+        "Upgrade-Insecure-Requests": "1",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
+    }
+    proxies = {}
+    if proxy_url:
+        parsed_proxy_url = requests.utils.requote_uri(proxy_url)
+        proxies = {"http": parsed_proxy_url, "https": parsed_proxy_url}
+    response = requests.get(room_url, headers=headers, proxies=proxies)
+    response.raise_for_status()
+    data_formatted, price_dependency_input=parse_body_details_wrapper(response.text)
+    cookies = response.cookies
+    return data_formatted, price_dependency_input, cookies
```

### Comparing `gobnb-0.0.7/src/gobnb/parse.py` & `gobnb-0.0.8/src/gobnb/parse.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import re
-import json
-from bs4 import BeautifulSoup
-from gobnb.standardize import standardize_details
-from gobnb.utils import remove_space
-
-regxApiKey = re.compile(r'"key":".+?"')
-regexLanguage = re.compile(r'"language":".+?"')
-
-
-def parse_body_details_wrapper(body:str):
-    data_raw, language, api_key = parse_body_details(body)
-    data_formatted = standardize_details(data_raw) 
-    data_formatted["language"] = language
-    price_dependency_input={
-        "product_id": data_raw['variables']['id'],
-        "impression_id": data_raw['variables']['pdpSectionsRequest']['p3ImpressionId'],
-        "api_key": api_key
-    }
-    return data_formatted, price_dependency_input
-
-def parse_body_details(body:str):
-    soup = BeautifulSoup(body, 'html.parser')
-    data_deferred_state = soup.select("#data-deferred-state-0")[0].getText()
-    html_data = remove_space(data_deferred_state)
-    language = regexLanguage.search(body).group()
-    language = language.replace('"language":"', "")
-    language = language.replace('"', "")
-    api_key = regxApiKey.search(body).group()
-    api_key = api_key.replace('"key":"', "")
-    api_key = api_key.replace('"', "")
-    data = json.loads(html_data)
-    details_data = data["niobeMinimalClientData"][0][1]
-    return details_data, language, api_key
+import re
+import json
+from bs4 import BeautifulSoup
+from gobnb.standardize import standardize_details
+from gobnb.utils import remove_space
+
+regxApiKey = re.compile(r'"key":".+?"')
+regexLanguage = re.compile(r'"language":".+?"')
+
+
+def parse_body_details_wrapper(body:str):
+    data_raw, language, api_key = parse_body_details(body)
+    data_formatted = standardize_details(data_raw) 
+    data_formatted["language"] = language
+    price_dependency_input={
+        "product_id": data_raw['variables']['id'],
+        "impression_id": data_raw['variables']['pdpSectionsRequest']['p3ImpressionId'],
+        "api_key": api_key
+    }
+    return data_formatted, price_dependency_input
+
+def parse_body_details(body:str):
+    soup = BeautifulSoup(body, 'html.parser')
+    data_deferred_state = soup.select("#data-deferred-state-0")[0].getText()
+    html_data = remove_space(data_deferred_state)
+    language = regexLanguage.search(body).group()
+    language = language.replace('"language":"', "")
+    language = language.replace('"', "")
+    api_key = regxApiKey.search(body).group()
+    api_key = api_key.replace('"key":"', "")
+    api_key = api_key.replace('"', "")
+    data = json.loads(html_data)
+    details_data = data["niobeMinimalClientData"][0][1]
+    return details_data, language, api_key
```

### Comparing `gobnb-0.0.7/src/gobnb/price.py` & `gobnb-0.0.8/src/gobnb/price.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import json
-from curl_cffi import requests
-from gobnb.utils import get_nested_value,remove_space,parse_price_symbol
-from urllib.parse import urlencode
-
-ep = "https://www.airbnb.com/api/v3/StaysPdpSections"
-
-def get_price(product_id: str,impresion_id: str,api_key: str, currency: str, cookies: list, proxy_url: str) -> (float,str,str):
-        headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
-            "X-Airbnb-Api-Key": api_key,
-        }
-        entension={
-            "persistedQuery": {
-                "version":1,
-                "sha256Hash": "e6a7821cf0f78dfc0baab6fd111027eb2976355f2aecbb84bc2086ee6e57161b",
-            },
-        }
-        dataRawExtension = json.dumps(entension)
-        variablesData={
-            "id": product_id,
-            "pdpSectionsRequest": {
-                "adults": "1",
-                "bypassTargetings": None,
-                "bypassTargetings":              False,
-                "categoryTag":                   None,
-                "causeId":                       None,
-                "children":                      None,
-                "disasterId":                    None,
-                "discountedGuestFeeVersion":     None,
-                "displayExtensions":             None,
-                "federatedSearchId":             None,
-                "forceBoostPriorityMessageType": None,
-                "infants":                       None,
-                "interactionType":               None,
-                "layouts":                       ["SIDEBAR", "SINGLE_COLUMN"],
-                "pets":                          0,
-                "pdpTypeOverride":               None,
-                "photoId":                       None,
-                "preview":                       False,
-                "previousStateCheckIn":          None,
-                "previousStateCheckOut":         None,
-                "priceDropSource":               None,
-                "privateBooking":                False,
-                "promotionUuid":                 None,
-                "relaxedAmenityIds":             None,
-                "searchId":                      None,
-                "selectedCancellationPolicyId":  None,
-                "selectedRatePlanId":            None,
-                "splitStays":                    None,
-                "staysBookingMigrationEnabled":  False,
-                "translateUgc":                  None,
-                "useNewSectionWrapperApi":       False,
-                "sectionIds": [
-                    "CANCELLATION_POLICY_PICKER_MODAL", "BOOK_IT_CALENDAR_SHEET", "POLICIES_DEFAULT", "BOOK_IT_SIDEBAR", "URGENCY_COMMITMENT_SIDEBAR",
-                    "BOOK_IT_NAV", "BOOK_IT_FLOATING_FOOTER", "EDUCATION_FOOTER_BANNER", "URGENCY_COMMITMENT", "EDUCATION_FOOTER_BANNER_MODAL"],
-                "checkIn":        None,
-                "checkOut":       None,
-                "p3ImpressionId": impresion_id,
-            },
-        }
-        dataRawVariables = json.dumps(variablesData)
-        query = {
-            "operationName": "StaysPdpSections",
-            "locale": "en",
-            "currency": currency,
-            "variables": dataRawVariables,
-            "extensions": dataRawExtension,
-        }
-        url = f"{ep}?{urlencode(query)}"
-        
-        session = requests.Session()
-        if proxy_url:
-            session.proxies.update({'http': proxy_url, 'https': proxy_url})
-
-        for name in cookies:
-            session.cookies.set(name, cookies[name])
-
-        response = session.get(url, headers=headers)
-        response.raise_for_status()
-
-        data = response.json()
-        for section in get_nested_value(data,"data.presentation.stayProductDetailPage.sections.sections",[]):
-            if get_nested_value(section,"section.__typename","")=="BookItSection":
-                pr=get_nested_value(section,"section.structuredDisplayPrice.primaryLine",{})
-                price=remove_space(pr.get("price",""))
-                qualifier=remove_space(pr.get("qualifier",""))
-                ammount, currency = parse_price_symbol(price)
-                return ammount, currency,qualifier
+import json
+from curl_cffi import requests
+from gobnb.utils import get_nested_value,remove_space,parse_price_symbol
+from urllib.parse import urlencode
+
+ep = "https://www.airbnb.com/api/v3/StaysPdpSections"
+
+def get_price(product_id: str,impresion_id: str,api_key: str, currency: str, cookies: list, proxy_url: str) -> (float,str,str):
+        headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+            "X-Airbnb-Api-Key": api_key,
+        }
+        entension={
+            "persistedQuery": {
+                "version":1,
+                "sha256Hash": "e6a7821cf0f78dfc0baab6fd111027eb2976355f2aecbb84bc2086ee6e57161b",
+            },
+        }
+        dataRawExtension = json.dumps(entension)
+        variablesData={
+            "id": product_id,
+            "pdpSectionsRequest": {
+                "adults": "1",
+                "bypassTargetings": None,
+                "bypassTargetings":              False,
+                "categoryTag":                   None,
+                "causeId":                       None,
+                "children":                      None,
+                "disasterId":                    None,
+                "discountedGuestFeeVersion":     None,
+                "displayExtensions":             None,
+                "federatedSearchId":             None,
+                "forceBoostPriorityMessageType": None,
+                "infants":                       None,
+                "interactionType":               None,
+                "layouts":                       ["SIDEBAR", "SINGLE_COLUMN"],
+                "pets":                          0,
+                "pdpTypeOverride":               None,
+                "photoId":                       None,
+                "preview":                       False,
+                "previousStateCheckIn":          None,
+                "previousStateCheckOut":         None,
+                "priceDropSource":               None,
+                "privateBooking":                False,
+                "promotionUuid":                 None,
+                "relaxedAmenityIds":             None,
+                "searchId":                      None,
+                "selectedCancellationPolicyId":  None,
+                "selectedRatePlanId":            None,
+                "splitStays":                    None,
+                "staysBookingMigrationEnabled":  False,
+                "translateUgc":                  None,
+                "useNewSectionWrapperApi":       False,
+                "sectionIds": [
+                    "CANCELLATION_POLICY_PICKER_MODAL", "BOOK_IT_CALENDAR_SHEET", "POLICIES_DEFAULT", "BOOK_IT_SIDEBAR", "URGENCY_COMMITMENT_SIDEBAR",
+                    "BOOK_IT_NAV", "BOOK_IT_FLOATING_FOOTER", "EDUCATION_FOOTER_BANNER", "URGENCY_COMMITMENT", "EDUCATION_FOOTER_BANNER_MODAL"],
+                "checkIn":        None,
+                "checkOut":       None,
+                "p3ImpressionId": impresion_id,
+            },
+        }
+        dataRawVariables = json.dumps(variablesData)
+        query = {
+            "operationName": "StaysPdpSections",
+            "locale": "en",
+            "currency": currency,
+            "variables": dataRawVariables,
+            "extensions": dataRawExtension,
+        }
+        url = f"{ep}?{urlencode(query)}"
+        
+        session = requests.Session()
+        if proxy_url:
+            session.proxies.update({'http': proxy_url, 'https': proxy_url})
+
+        for name in cookies:
+            session.cookies.set(name, cookies[name])
+
+        response = session.get(url, headers=headers)
+        response.raise_for_status()
+
+        data = response.json()
+        for section in get_nested_value(data,"data.presentation.stayProductDetailPage.sections.sections",[]):
+            if get_nested_value(section,"section.__typename","")=="BookItSection":
+                pr=get_nested_value(section,"section.structuredDisplayPrice.primaryLine",{})
+                price=remove_space(pr.get("price",""))
+                qualifier=remove_space(pr.get("qualifier",""))
+                ammount, currency = parse_price_symbol(price)
+                return ammount, currency,qualifier
         return 0,"",""
```

### Comparing `gobnb-0.0.7/src/gobnb/search.py` & `gobnb-0.0.8/src/gobnb/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,130 @@
-import gobnb.api as api
-from datetime import datetime
-from urllib.parse import urlencode
-from gobnb.standardize import get_nested_value,standardize_search
-from curl_cffi import requests
-import json
-
-treament = [
-	"feed_map_decouple_m11_treatment",
-	"stays_search_rehydration_treatment_desktop",
-	"stays_search_rehydration_treatment_moweb",
-	"selective_query_feed_map_homepage_desktop_treatment",
-	"selective_query_feed_map_homepage_moweb_treatment",
-]
-
-def Search_all(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, currency:str, proxy_url:str):
-    api_key = api.get(proxy_url)
-    all_results = []
-    cursor = ""
-    while True:
-        results_raw = search(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value,cursor, currency, api_key, proxy_url)
-        results = standardize_search(results_raw.get("searchResults",[]))
-        all_results = all_results + results
-        if len(results)==0 or "nextPageCursor" not in results_raw["paginationInfo"] or  results_raw["paginationInfo"]["nextPageCursor"] is None:
-            break
-        cursor = results_raw["paginationInfo"]["nextPageCursor"]
-    return all_results
-
-def Search_first_page(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, cursor:str, currency:str, proxy_url:str):
-    api_key = api.get(proxy_url)
-    results = search(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value,"", currency, api_key, proxy_url)
-    results = standardize_search(results)
-    return results
-
-def search(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, cursor:str, currency:str, api_key:str, proxy_url:str):
-    check_in_date = datetime.strptime(check_in, "%Y-%m-%d")
-    check_out_date = datetime.strptime(check_out, "%Y-%m-%d")
-
-    difference = check_out_date - check_in_date
-
-    days = difference.days
-
-    base_url = "https://www.airbnb.com/api/v3/StaysSearch/d4d9503616dc72ab220ed8dcf17f166816dccb2593e7b4625c91c3fce3a3b3d6"
-    query_params = {
-        "operationName": "StaysSearch",
-        "locale": "en",
-        "currency": currency,
-    }
-    url_parsed = f"{base_url}?{urlencode(query_params)}"
-    rawParams=[
-        {"filterName":"cdnCacheSafe","filterValues":["false"]},
-        {"filterName":"channel","filterValues":["EXPLORE"]},
-        {"filterName":"checkin","filterValues":[check_in]},
-        {"filterName":"checkout","filterValues":[check_out]},
-        {"filterName":"datePickerType","filterValues":["calendar"]},
-        {"filterName":"flexibleTripLengths","filterValues":["one_week"]},
-        {"filterName":"itemsPerGrid","filterValues":["50"]},#if you read this, this is items returned number, this can bex exploited  ;)
-        {"filterName":"monthlyLength","filterValues":["3"]},
-        {"filterName":"monthlyStartDate","filterValues":["2024-02-01"]},
-        {"filterName":"neLat","filterValues":[str(ne_lat)]},
-        {"filterName":"neLng","filterValues":[str(ne_long)]},
-        {"filterName":"placeId","filterValues":["ChIJpTeBx6wjq5oROJeXkPCSSSo"]},
-        {"filterName":"priceFilterInputType","filterValues":["0"]},
-        {"filterName":"priceFilterNumNights","filterValues":[str(days)]},
-        {"filterName":"query","filterValues":["Galapagos Island, Ecuador"]},
-        {"filterName":"screenSize","filterValues":["large"]},
-        {"filterName":"refinementPaths","filterValues":["/homes"]},
-        {"filterName":"searchByMap","filterValues":["true"]},
-        {"filterName":"swLat","filterValues":[str(sw_lat)]},
-        {"filterName":"swLng","filterValues":[str(sw_long)]},
-        {"filterName":"tabId","filterValues":["home_tab"]},
-        {"filterName":"version","filterValues":["1.8.3"]},
-        {"filterName":"zoomLevel","filterValues":[str(zoom_value)]},
-    ]
-    inputData = {
-        "operationName":"StaysSearch",
-        "extensions":{
-            "persistedQuery": {
-                "version": 1,
-                "sha256Hash": "d4d9503616dc72ab220ed8dcf17f166816dccb2593e7b4625c91c3fce3a3b3d6",
-            },
-        },
-        "variables":{
-            "includeMapResults": True,
-            "isLeanTreatment": False,
-            "staysMapSearchRequestV2": {
-                "cursor":cursor,
-                "requestedPageType":"STAYS_SEARCH",
-                "metadataOnly":False,
-                "source":"structured_search_input_header",
-                "searchType":"user_map_move",
-                "treatmentFlags":treament,
-                "rawParams":rawParams,
-            },
-            "staysSearchRequest": {
-                "cursor":cursor,
-                "maxMapItems": 9999,
-                "requestedPageType":"STAYS_SEARCH",
-                "metadataOnly":False,
-                "source":"structured_search_input_header",
-                "searchType":"user_map_move",
-                "treatmentFlags":treament,
-                "rawParams":rawParams,
-            },
-        },
-    }
-    headers = {
-        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-        "Accept-Language": "en",
-        "Cache-Control": "no-cache",
-        "Connection": "close",
-        "Pragma": "no-cache",
-        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
-        "Sec-Ch-Ua-Mobile": "?0",
-        "X-Airbnb-Api-Key": api_key,
-        "Sec-Ch-Ua-Platform": '"Windows"',
-        "Sec-Fetch-Dest": "document",
-        "Sec-Fetch-Mode": "navigate",
-        "Sec-Fetch-Site": "none",
-        "Sec-Fetch-User": "?1",
-        "Upgrade-Insecure-Requests": "1",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
-    }
-    proxies = {"http": proxy_url, "https": proxy_url} if proxy_url else None
-    response = requests.post(url_parsed, json = inputData, headers=headers,  impersonate="chrome110")
-    data = response.json()
-    to_return=get_nested_value(data,"data.presentation.staysSearch.results",{})
-    return to_return
+import gobnb.api as api
+from datetime import datetime
+from urllib.parse import urlencode
+from gobnb.standardize import get_nested_value,standardize_search
+from curl_cffi import requests
+
+treament = [
+	"feed_map_decouple_m11_treatment",
+	"stays_search_rehydration_treatment_desktop",
+	"stays_search_rehydration_treatment_moweb",
+	"selective_query_feed_map_homepage_desktop_treatment",
+	"selective_query_feed_map_homepage_moweb_treatment",
+]
+
+def Search_all(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, currency:str, proxy_url:str):
+    api_key = api.get(proxy_url)
+    all_results = []
+    cursor = ""
+    while True:
+        results_raw = search(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value,cursor, currency, api_key, proxy_url)
+        results = standardize_search(results_raw.get("searchResults",[]))
+        all_results = all_results + results
+        if len(results)==0 or "nextPageCursor" not in results_raw["paginationInfo"] or  results_raw["paginationInfo"]["nextPageCursor"] is None:
+            break
+        cursor = results_raw["paginationInfo"]["nextPageCursor"]
+    return all_results
+
+def Search_first_page(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, cursor:str, currency:str, proxy_url:str):
+    api_key = api.get(proxy_url)
+    results = search(check_in,check_out,ne_lat,ne_long,sw_lat,sw_long,zoom_value,"", currency, api_key, proxy_url)
+    results = standardize_search(results)
+    return results
+
+def search(check_in:str, check_out:str, ne_lat:float, ne_long:float, sw_lat:float, sw_long:float, zoom_value:int, cursor:str, currency:str, api_key:str, proxy_url:str):
+    check_in_date = datetime.strptime(check_in, "%Y-%m-%d")
+    check_out_date = datetime.strptime(check_out, "%Y-%m-%d")
+
+    difference = check_out_date - check_in_date
+
+    days = difference.days
+
+    base_url = "https://www.airbnb.com/api/v3/StaysSearch/d4d9503616dc72ab220ed8dcf17f166816dccb2593e7b4625c91c3fce3a3b3d6"
+    query_params = {
+        "operationName": "StaysSearch",
+        "locale": "en",
+        "currency": currency,
+    }
+    url_parsed = f"{base_url}?{urlencode(query_params)}"
+    rawParams=[
+        {"filterName":"cdnCacheSafe","filterValues":["false"]},
+        {"filterName":"channel","filterValues":["EXPLORE"]},
+        {"filterName":"checkin","filterValues":[check_in]},
+        {"filterName":"checkout","filterValues":[check_out]},
+        {"filterName":"datePickerType","filterValues":["calendar"]},
+        {"filterName":"flexibleTripLengths","filterValues":["one_week"]},
+        {"filterName":"itemsPerGrid","filterValues":["50"]},#if you read this, this is items returned number, this can bex exploited  ;)
+        {"filterName":"monthlyLength","filterValues":["3"]},
+        {"filterName":"monthlyStartDate","filterValues":["2024-02-01"]},
+        {"filterName":"neLat","filterValues":[str(ne_lat)]},
+        {"filterName":"neLng","filterValues":[str(ne_long)]},
+        {"filterName":"placeId","filterValues":["ChIJpTeBx6wjq5oROJeXkPCSSSo"]},
+        {"filterName":"priceFilterInputType","filterValues":["0"]},
+        {"filterName":"priceFilterNumNights","filterValues":[str(days)]},
+        {"filterName":"query","filterValues":["Galapagos Island, Ecuador"]},
+        {"filterName":"screenSize","filterValues":["large"]},
+        {"filterName":"refinementPaths","filterValues":["/homes"]},
+        {"filterName":"searchByMap","filterValues":["true"]},
+        {"filterName":"swLat","filterValues":[str(sw_lat)]},
+        {"filterName":"swLng","filterValues":[str(sw_long)]},
+        {"filterName":"tabId","filterValues":["home_tab"]},
+        {"filterName":"version","filterValues":["1.8.3"]},
+        {"filterName":"zoomLevel","filterValues":[str(zoom_value)]},
+    ]
+    inputData = {
+        "operationName":"StaysSearch",
+        "extensions":{
+            "persistedQuery": {
+                "version": 1,
+                "sha256Hash": "d4d9503616dc72ab220ed8dcf17f166816dccb2593e7b4625c91c3fce3a3b3d6",
+            },
+        },
+        "variables":{
+            "includeMapResults": True,
+            "isLeanTreatment": False,
+            "staysMapSearchRequestV2": {
+                "cursor":cursor,
+                "requestedPageType":"STAYS_SEARCH",
+                "metadataOnly":False,
+                "source":"structured_search_input_header",
+                "searchType":"user_map_move",
+                "treatmentFlags":treament,
+                "rawParams":rawParams,
+            },
+            "staysSearchRequest": {
+                "cursor":cursor,
+                "maxMapItems": 9999,
+                "requestedPageType":"STAYS_SEARCH",
+                "metadataOnly":False,
+                "source":"structured_search_input_header",
+                "searchType":"user_map_move",
+                "treatmentFlags":treament,
+                "rawParams":rawParams,
+            },
+        },
+    }
+    headers = {
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "Accept-Language": "en",
+        "Cache-Control": "no-cache",
+        "Connection": "close",
+        "Pragma": "no-cache",
+        "Sec-Ch-Ua": '"Not_A Brand";v="8", "Chromium";v="120", "Google Chrome";v="120"',
+        "Sec-Ch-Ua-Mobile": "?0",
+        "X-Airbnb-Api-Key": api_key,
+        "Sec-Ch-Ua-Platform": '"Windows"',
+        "Sec-Fetch-Dest": "document",
+        "Sec-Fetch-Mode": "navigate",
+        "Sec-Fetch-Site": "none",
+        "Sec-Fetch-User": "?1",
+        "Upgrade-Insecure-Requests": "1",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36"
+    }
+    proxies = {}
+    if proxy_url:
+        parsed_proxy_url = requests.utils.requote_uri(proxy_url)
+        proxies = {"http": parsed_proxy_url, "https": parsed_proxy_url}
+    response = requests.post(url_parsed, json = inputData, headers=headers, proxies=proxies,  impersonate="chrome110")
+    data = response.json()
+    to_return=get_nested_value(data,"data.presentation.staysSearch.results",{})
+    return to_return
```

### Comparing `gobnb-0.0.7/src/gobnb/standardize.py` & `gobnb-0.0.8/src/gobnb/standardize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,229 +1,231 @@
-import re
-from gobnb.utils import get_nested_value,parse_price_symbol
-
-regex_number =  re.compile(r'\d+')
-            
-def standardize_search(results):
-    datas = []
-    for result in results:
-        lt = get_nested_value(result,"listing",{})
-        pr = get_nested_value(result,"pricingQuote.structuredStayDisplayPrice",{})
-        data = {
-            "room_id":  int(lt["id"]),
-            "category": get_nested_value(lt,"roomTypeCategory",""),
-            "kind":     get_nested_value(lt,"pdpUrlType",""),
-            "name":     get_nested_value(lt,"name",""),
-            "title":    get_nested_value(lt,"title",""),
-            "type":     get_nested_value(lt,"listingObjType",""),
-            "long_stay_discount":{},
-            "fee":{
-                "airbnb":{},
-                "cleaning":{},
-            },
-            "price": {
-                "unit":{
-                    "qualifier":  get_nested_value(pr,"primaryLine.qualifier","") 
-                },
-                "total":{},
-                "break_down":[],
-            },
-            "rating":{
-                "value":0,
-                "reviewCount": 0,
-            },
-            "images": [],
-            "badges": [],
-            "coordinates":{
-                "latitude": get_nested_value(lt,"coordinate.latitude",0),
-                "longitud": get_nested_value(lt,"coordinate.longitude",0),
-            },
-        }
-        for badge in get_nested_value(lt,"formattedBadges",[]):
-            data["badges"].append(get_nested_value(badge,"loggingContext.badgeType",""))
-
-        avgRatingLocalized = get_nested_value(lt,"avgRatingLocalized","")
-        splited = avgRatingLocalized.split(" ")
-        if len(splited)==2:
-            rating = float(splited[0])
-            data["rating"]["value"]=rating
-            reviewCount = regex_number.search(splited[1]).group()
-            data["rating"]["reviewCount"]=reviewCount
-        price_to_use = get_nested_value(pr,"primaryLine.originalPrice","")
-        if price_to_use=="":
-              price_to_use = get_nested_value(pr,"primaryLine.price","")
-
-        if price_to_use!="": 
-            amount, currency = parse_price_symbol(price_to_use)
-            data["price"]["unit"]["curency_symbol"]=currency
-            data["price"]["unit"]["amount"]=amount   
-
-        discountedPrice=get_nested_value(pr,"primaryLine.discountedPrice","")
-        if discountedPrice!="":
-            amount, _ = parse_price_symbol(discountedPrice)
-            data["price"]["unit"]["discount"]=amount
-
-        splited = get_nested_value(pr,"secondaryLine.price","").split(" ")
-        price_to_use=""
-        match len(splited):
-            case 2:
-                price_to_use=splited[0]
-            case 3:
-                splited = splited[:len(splited)-1]
-                price_to_use = "".join(splited)
-            case _:
-                print("error check: ",splited )
-                continue
-
-        amount, currency = parse_price_symbol(price_to_use)
-        data["price"]["total"]["currency_symbol"]=currency
-        data["price"]["total"]["amount"]=amount
-        for image_data in get_nested_value(lt,"contextualPictures",[]):
-            img={"url": get_nested_value(image_data,"picture","")}
-            data["images"].append(img)   
-        for price_detail in get_nested_value(pr,"explanationData.priceDetails",[]):
-            if "items" not in price_detail:
-                continue
-            for item in get_nested_value(price_detail,"items",[]): 
-                amount, currency = parse_price_symbol(item["priceString"])
-                data["price"]["break_down"].append({"description":item["description"],"amount":amount,"currency":currency})
-                match item["displayComponentType"]:
-                    case "DISCOUNTED_EXPLANATION_LINE_ITEM":
-                        match item["description"]:
-                            case "Long stay discount":
-                                data["long_stay_discount"]["amount"]=amount
-                                data["long_stay_discount"]["currency_symbol"]=currency
-                    case "DEFAULT_EXPLANATION_LINE_ITEM":
-                        match item["description"]:
-                            case "Cleaning fee":
-                                data["fee"]["cleaning"]["amount"]=amount
-                                data["fee"]["cleaning"]["currency_symbol"]=currency
-                            case "Airbnb service fee":
-                                data["fee"]["airbnb"]["amount"]=amount
-                                data["fee"]["airbnb"]["currency_symbol"]=currency
-        datas.append(data)
-
-    return datas
-        
-
-def standardize_details(meta):
-    ev = meta["data"]["presentation"]["stayProductDetailPage"]["sections"]["metadata"]["loggingContext"]["eventDataLogging"]
-    data = {
-        "coordinates": {
-                "latitude":         get_nested_value(ev,"listingLat",0),
-                "longitude":        get_nested_value(ev,"listingLng",0),
-        },
-        "room_type":                get_nested_value(ev,"roomType",""),
-        "is_super_host":            get_nested_value(ev,"isSuperhost",""),
-        "home_tier":                get_nested_value(ev,"homeTier",""),
-        "person_capacity":          get_nested_value(ev,"personCapacity",0),
-        "rating":{
-            "accuracy":             get_nested_value(ev,"accuracyRating",0),
-            "checking":             get_nested_value(ev,"checkinRating",0),
-            "cleanliness":          get_nested_value(ev,"cleanlinessRating",0),
-            "communication":        get_nested_value(ev,"communicationRating",0),
-            "location":             get_nested_value(ev,"locationRating",0),
-            "value":                get_nested_value(ev,"valueRating",0),
-            "guest_satisfaction":   get_nested_value(ev,"guestSatisfactionOverall",0),
-            "review_count":         get_nested_value(ev,"visibleReviewCount",0),
-        },
-        "house_rules":{
-            "aditional":"",
-            "general": [],
-        },
-        "host":{
-                "id":"",   
-                "name":"",  
-                "joined_on":"",  
-                "description":"",  
-        },
-        "sub_description":{
-            "title":"",
-            "items": [],
-        },
-        "amenities": [],
-        "co_hosts":[],
-        "images":[],
-        "location_descriptions":[],
-        "amenities":[],
-        "highlights":[],
-    }
-
-    sd = get_nested_value(meta,"data.presentation.stayProductDetailPage.sections.sbuiData")
-    for section in get_nested_value(sd,"sectionConfiguration.root.sections",[]):
-        typeName=get_nested_value(section,"sectionData.__typename","")
-        if typeName == "PdpHostOverviewDefaultSection":
-            data["host"]={
-                "id" :  get_nested_value(section,"sectionData.hostAvatar.loggingEventData.eventData.pdpContext.hostId",""),
-                "name": get_nested_value(section,"sectionData.title",""),
-            }
-        elif typeName == "PdpOverviewV2Section":
-            data["sub_description"]["title"]=get_nested_value(section,"sectionData.title","")
-            for item in get_nested_value(section,"sectionData.overviewItems",[]):
-                data["sub_description"]["items"].append(get_nested_value(item,"title",""))
-
-    for section in get_nested_value(meta,"data.presentation.stayProductDetailPage.sections.sections",[]):
-        typeName=get_nested_value(section,"section.__typename","")
-        match typeName:
-            case "HostProfileSection": 
-                data["host"]["id"] = get_nested_value(section,"section.hostAvatar.userID","")
-                data["host"]["name"] = get_nested_value(section,"section.title","")
-                data["host"]["joined_on"] = get_nested_value(section,"section.subtitle","")
-                data["host"]["description"] = get_nested_value(section,"section.hostProfileDescription.htmlText","")
-                for cohost in get_nested_value(section,"section.additionalHosts",[]):
-                    data["co_hosts"].append({"id":cohost.get("id",""),"name":cohost.get("name","")})
-            case "PhotoTourModalSection":  
-                for mediaItem in get_nested_value(section,"section.mediaItems",[]):
-                    img={
-                        "title": mediaItem.get("accessibilityLabel",""),
-                        "url": mediaItem.get("baseUrl",""),
-                    }
-                    data["images"].append(img)
-            case "PoliciesSection":        
-                for houseRulesSection in get_nested_value(section,"section.houseRulesSections",[]):
-                    house_rule={
-                        "title": houseRulesSection.get("title",""),
-                        "values":[],
-                    }
-                    for item in houseRulesSection.get("items",[]):
-                            if item.get("title","")=="Additional rules":
-                                data["house_rules"]["aditional"]=get_nested_value(item,"html.htmlText","")
-                                continue
-                            house_rule["values"].append({"title":item.get("title","") ,"icon": item.get("icon","")})
-
-                    data["house_rules"]["general"].append(house_rule)
-            case "LocationSection":
-                for locationDetail in get_nested_value(section,"section.seeAllLocationDetails",[]):
-                    seeAllLocationDetail={
-                        "title": locationDetail.get("title",""),
-                        "content": get_nested_value(locationDetail,"content.htmlText"),
-                    }
-                    data["location_descriptions"].append(seeAllLocationDetail)
-            case "PdpTitleSection":           
-                    data["title"]=section.get("title","")
-            case "PdpHighlightsSection":
-                for highlitingData in get_nested_value(section,"section.highlights",[]):
-                    highliting={
-                        "title": highlitingData.get("title",""),
-                        "subtitle": highlitingData.get("subtitle",""),
-                        "icon": highlitingData.get("icon",""),
-                    }
-                    data["highlights"].append(highliting)
-            case "PdpDescriptionSection":
-                data["description"]=  get_nested_value(section,"section.htmlDescription.htmlText","")
-            case "AmenitiesSection":  
-                for amenityGroupRaw in get_nested_value(section,"section.seeAllAmenitiesGroups",[]):
-                    amenityGroup={
-                        "title": amenityGroupRaw.get("title",""),
-                        "values": [],
-                    }
-                    for amenityRaw in amenityGroupRaw.get("amenities",[]):
-                        amenity = {
-                            "title":     amenityRaw.get("title",""),
-                            "subtitle":  amenityRaw.get("subtitle",""),
-                            "icon":      amenityRaw.get("icon",""),
-                            "available": amenityRaw.get("available",""),
-                        }
-                        amenityGroup["values"].append(amenity)
-                    data["amenities"].append(amenityGroup)
-    return data
-
+import re
+from gobnb.utils import get_nested_value,parse_price_symbol
+
+regex_number =  re.compile(r'\d+')
+            
+def standardize_search(results):
+    datas = []
+    for result in results:
+        type_name = get_nested_value(result,"__typename","")
+        if type_name!="StaySearchResult":
+            continue
+        lt = get_nested_value(result,"listing",{})
+        pr = get_nested_value(result,"pricingQuote.structuredStayDisplayPrice",{})
+        data = {
+            "room_id":  int(lt["id"]),
+            "category": get_nested_value(lt,"roomTypeCategory",""),
+            "kind":     get_nested_value(lt,"pdpUrlType",""),
+            "name":     get_nested_value(lt,"name",""),
+            "title":    get_nested_value(lt,"title",""),
+            "type":     get_nested_value(lt,"listingObjType",""),
+            "long_stay_discount":{},
+            "fee":{
+                "airbnb":{},
+                "cleaning":{},
+            },
+            "price": {
+                "unit":{
+                    "qualifier":  get_nested_value(pr,"primaryLine.qualifier","") 
+                },
+                "total":{},
+                "break_down":[],
+            },
+            "rating":{
+                "value":0,
+                "reviewCount": 0,
+            },
+            "images": [],
+            "badges": [],
+            "coordinates":{
+                "latitude": get_nested_value(lt,"coordinate.latitude",0),
+                "longitud": get_nested_value(lt,"coordinate.longitude",0),
+            },
+        }
+        for badge in get_nested_value(lt,"formattedBadges",[]):
+            data["badges"].append(get_nested_value(badge,"loggingContext.badgeType",""))
+
+        avgRatingLocalized = get_nested_value(lt,"avgRatingLocalized","")
+        splited = avgRatingLocalized.split(" ")
+        if len(splited)==2:
+            rating = float(splited[0])
+            data["rating"]["value"]=rating
+            reviewCount = regex_number.search(splited[1]).group()
+            data["rating"]["reviewCount"]=reviewCount
+        price_to_use = get_nested_value(pr,"primaryLine.originalPrice","")
+        if price_to_use=="":
+              price_to_use = get_nested_value(pr,"primaryLine.price","")
+
+        if price_to_use!="": 
+            amount, currency = parse_price_symbol(price_to_use)
+            data["price"]["unit"]["curency_symbol"]=currency
+            data["price"]["unit"]["amount"]=amount   
+
+        discountedPrice=get_nested_value(pr,"primaryLine.discountedPrice","")
+        if discountedPrice!="":
+            amount, _ = parse_price_symbol(discountedPrice)
+            data["price"]["unit"]["discount"]=amount
+
+        splited = get_nested_value(pr,"secondaryLine.price","").split(" ")
+        price_to_use=""
+        match len(splited):
+            case 2:
+                price_to_use=splited[0]
+            case 3:
+                splited = splited[:len(splited)-1]
+                price_to_use = "".join(splited)
+            case _:
+                print("error check: ",splited )
+                continue
+
+        amount, currency = parse_price_symbol(price_to_use)
+        data["price"]["total"]["currency_symbol"]=currency
+        data["price"]["total"]["amount"]=amount
+        for image_data in get_nested_value(lt,"contextualPictures",[]):
+            img={"url": get_nested_value(image_data,"picture","")}
+            data["images"].append(img)   
+        for price_detail in get_nested_value(pr,"explanationData.priceDetails",[]):
+            if "items" not in price_detail:
+                continue
+            for item in get_nested_value(price_detail,"items",[]): 
+                amount, currency = parse_price_symbol(item["priceString"])
+                data["price"]["break_down"].append({"description":item["description"],"amount":amount,"currency":currency})
+                match item["displayComponentType"]:
+                    case "DISCOUNTED_EXPLANATION_LINE_ITEM":
+                        match item["description"]:
+                            case "Long stay discount":
+                                data["long_stay_discount"]["amount"]=amount
+                                data["long_stay_discount"]["currency_symbol"]=currency
+                    case "DEFAULT_EXPLANATION_LINE_ITEM":
+                        match item["description"]:
+                            case "Cleaning fee":
+                                data["fee"]["cleaning"]["amount"]=amount
+                                data["fee"]["cleaning"]["currency_symbol"]=currency
+                            case "Airbnb service fee":
+                                data["fee"]["airbnb"]["amount"]=amount
+                                data["fee"]["airbnb"]["currency_symbol"]=currency
+        datas.append(data)
+
+    return datas
+        
+
+def standardize_details(meta):
+    ev = meta["data"]["presentation"]["stayProductDetailPage"]["sections"]["metadata"]["loggingContext"]["eventDataLogging"]
+    data = {
+        "coordinates": {
+                "latitude":         get_nested_value(ev,"listingLat",0),
+                "longitude":        get_nested_value(ev,"listingLng",0),
+        },
+        "room_type":                get_nested_value(ev,"roomType",""),
+        "is_super_host":            get_nested_value(ev,"isSuperhost",""),
+        "home_tier":                get_nested_value(ev,"homeTier",""),
+        "person_capacity":          get_nested_value(ev,"personCapacity",0),
+        "rating":{
+            "accuracy":             get_nested_value(ev,"accuracyRating",0),
+            "checking":             get_nested_value(ev,"checkinRating",0),
+            "cleanliness":          get_nested_value(ev,"cleanlinessRating",0),
+            "communication":        get_nested_value(ev,"communicationRating",0),
+            "location":             get_nested_value(ev,"locationRating",0),
+            "value":                get_nested_value(ev,"valueRating",0),
+            "guest_satisfaction":   get_nested_value(ev,"guestSatisfactionOverall",0),
+            "review_count":         get_nested_value(ev,"visibleReviewCount",0),
+        },
+        "house_rules":{
+            "aditional":"",
+            "general": [],
+        },
+        "host":{
+                "id":"",   
+                "name":"",  
+                "joined_on":"",  
+                "description":"",  
+        },
+        "sub_description":{
+            "title":"",
+            "items": [],
+        },
+        "amenities": [],
+        "co_hosts":[],
+        "images":[],
+        "location_descriptions":[],
+        "highlights":[],
+    }
+
+    sd = get_nested_value(meta,"data.presentation.stayProductDetailPage.sections.sbuiData")
+    for section in get_nested_value(sd,"sectionConfiguration.root.sections",[]):
+        typeName=get_nested_value(section,"sectionData.__typename","")
+        if typeName == "PdpHostOverviewDefaultSection":
+            data["host"]={
+                "id" :  get_nested_value(section,"sectionData.hostAvatar.loggingEventData.eventData.pdpContext.hostId",""),
+                "name": get_nested_value(section,"sectionData.title",""),
+            }
+        elif typeName == "PdpOverviewV2Section":
+            data["sub_description"]["title"]=get_nested_value(section,"sectionData.title","")
+            for item in get_nested_value(section,"sectionData.overviewItems",[]):
+                data["sub_description"]["items"].append(get_nested_value(item,"title",""))
+
+    for section in get_nested_value(meta,"data.presentation.stayProductDetailPage.sections.sections",[]):
+        typeName=get_nested_value(section,"section.__typename","")
+        match typeName:
+            case "HostProfileSection": 
+                data["host"]["id"] = get_nested_value(section,"section.hostAvatar.userID","")
+                data["host"]["name"] = get_nested_value(section,"section.title","")
+                data["host"]["joined_on"] = get_nested_value(section,"section.subtitle","")
+                data["host"]["description"] = get_nested_value(section,"section.hostProfileDescription.htmlText","")
+                for cohost in get_nested_value(section,"section.additionalHosts",[]):
+                    data["co_hosts"].append({"id":cohost.get("id",""),"name":cohost.get("name","")})
+            case "PhotoTourModalSection":  
+                for mediaItem in get_nested_value(section,"section.mediaItems",[]):
+                    img={
+                        "title": mediaItem.get("accessibilityLabel",""),
+                        "url": mediaItem.get("baseUrl",""),
+                    }
+                    data["images"].append(img)
+            case "PoliciesSection":        
+                for houseRulesSection in get_nested_value(section,"section.houseRulesSections",[]):
+                    house_rule={
+                        "title": houseRulesSection.get("title",""),
+                        "values":[],
+                    }
+                    for item in houseRulesSection.get("items",[]):
+                            if item.get("title","")=="Additional rules":
+                                data["house_rules"]["aditional"]=get_nested_value(item,"html.htmlText","")
+                                continue
+                            house_rule["values"].append({"title":item.get("title","") ,"icon": item.get("icon","")})
+
+                    data["house_rules"]["general"].append(house_rule)
+            case "LocationSection":
+                for locationDetail in get_nested_value(section,"section.seeAllLocationDetails",[]):
+                    seeAllLocationDetail={
+                        "title": locationDetail.get("title",""),
+                        "content": get_nested_value(locationDetail,"content.htmlText"),
+                    }
+                    data["location_descriptions"].append(seeAllLocationDetail)
+            case "PdpTitleSection":           
+                    data["title"]=section.get("title","")
+            case "PdpHighlightsSection":
+                for highlitingData in get_nested_value(section,"section.highlights",[]):
+                    highliting={
+                        "title": highlitingData.get("title",""),
+                        "subtitle": highlitingData.get("subtitle",""),
+                        "icon": highlitingData.get("icon",""),
+                    }
+                    data["highlights"].append(highliting)
+            case "PdpDescriptionSection":
+                data["description"]=  get_nested_value(section,"section.htmlDescription.htmlText","")
+            case "AmenitiesSection":  
+                for amenityGroupRaw in get_nested_value(section,"section.seeAllAmenitiesGroups",[]):
+                    amenityGroup={
+                        "title": amenityGroupRaw.get("title",""),
+                        "values": [],
+                    }
+                    for amenityRaw in amenityGroupRaw.get("amenities",[]):
+                        amenity = {
+                            "title":     amenityRaw.get("title",""),
+                            "subtitle":  amenityRaw.get("subtitle",""),
+                            "icon":      amenityRaw.get("icon",""),
+                            "available": amenityRaw.get("available",""),
+                        }
+                        amenityGroup["values"].append(amenity)
+                    data["amenities"].append(amenityGroup)
+    return data
+
```

