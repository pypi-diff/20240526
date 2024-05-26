# Comparing `tmp/proxygetter-0.2.1.tar.gz` & `tmp/proxygetter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxygetter-0.2.1.tar", last modified: Fri Dec 29 18:24:52 2023, max compression
+gzip compressed data, was "proxygetter-0.2.2.tar", last modified: Sun May 26 18:03:18 2024, max compression
```

## Comparing `proxygetter-0.2.1.tar` & `proxygetter-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-12-29 18:24:52.027465 proxygetter-0.2.1/
--rw-rw-rw-   0        0        0     1101 2023-12-29 18:15:10.000000 proxygetter-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-12-29 18:15:10.000000 proxygetter-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3136 2023-12-29 18:24:52.027465 proxygetter-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1994 2023-12-29 18:15:10.000000 proxygetter-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-12-29 18:24:52.010323 proxygetter-0.2.1/proxygetter/
--rw-rw-rw-   0        0        0      170 2023-12-29 18:15:10.000000 proxygetter-0.2.1/proxygetter/__init__.py
--rw-rw-rw-   0        0        0      181 2023-12-29 18:15:10.000000 proxygetter-0.2.1/proxygetter/blacklist.py
--rw-rw-rw-   0        0        0     1803 2023-12-29 18:15:10.000000 proxygetter-0.2.1/proxygetter/proxy.py
--rw-rw-rw-   0        0        0     2732 2023-12-29 18:15:10.000000 proxygetter-0.2.1/proxygetter/proxy_manager.py
--rw-rw-rw-   0        0        0     3146 2023-12-29 18:15:10.000000 proxygetter-0.2.1/proxygetter/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-29 18:24:52.026465 proxygetter-0.2.1/proxygetter.egg-info/
--rw-rw-rw-   0        0        0     3136 2023-12-29 18:24:51.000000 proxygetter-0.2.1/proxygetter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-12-29 18:24:51.000000 proxygetter-0.2.1/proxygetter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-29 18:24:51.000000 proxygetter-0.2.1/proxygetter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      259 2023-12-29 18:24:51.000000 proxygetter-0.2.1/proxygetter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-12-29 18:24:51.000000 proxygetter-0.2.1/proxygetter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       50 2023-12-29 18:15:10.000000 proxygetter-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      274 2023-12-29 18:16:48.000000 proxygetter-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-12-29 18:24:52.028465 proxygetter-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-12-29 18:18:14.000000 proxygetter-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-29 18:24:52.025465 proxygetter-0.2.1/tests/
--rw-rw-rw-   0        0        0        0 2023-12-29 18:15:10.000000 proxygetter-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0      957 2023-12-29 18:15:10.000000 proxygetter-0.2.1/tests/test_proxy.py
--rw-rw-rw-   0        0        0        6 2023-12-29 18:15:10.000000 proxygetter-0.2.1/tests/test_proxy_manager.py
--rw-rw-rw-   0        0        0     2004 2023-12-29 18:15:10.000000 proxygetter-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 VEAR4001   (502) staff       (20)        0 2024-05-26 18:03:18.925208 proxygetter-0.2.2/
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     1080 2024-05-26 17:45:00.000000 proxygetter-0.2.2/LICENSE
+-rw-r--r--   0 VEAR4001   (502) staff       (20)       24 2024-05-26 17:45:00.000000 proxygetter-0.2.2/MANIFEST.in
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     3047 2024-05-26 18:03:18.924990 proxygetter-0.2.2/PKG-INFO
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     1919 2024-05-26 17:45:00.000000 proxygetter-0.2.2/README.md
+drwxr-xr-x   0 VEAR4001   (502) staff       (20)        0 2024-05-26 18:03:18.923291 proxygetter-0.2.2/proxygetter/
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      165 2024-05-26 17:45:00.000000 proxygetter-0.2.2/proxygetter/__init__.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      171 2024-05-26 17:45:00.000000 proxygetter-0.2.2/proxygetter/blacklist.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     1751 2024-05-26 17:45:00.000000 proxygetter-0.2.2/proxygetter/proxy.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     2644 2024-05-26 17:45:00.000000 proxygetter-0.2.2/proxygetter/proxy_manager.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     3039 2024-05-26 17:45:00.000000 proxygetter-0.2.2/proxygetter/utils.py
+drwxr-xr-x   0 VEAR4001   (502) staff       (20)        0 2024-05-26 18:03:18.924739 proxygetter-0.2.2/proxygetter.egg-info/
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     3047 2024-05-26 18:03:18.000000 proxygetter-0.2.2/proxygetter.egg-info/PKG-INFO
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      450 2024-05-26 18:03:18.000000 proxygetter-0.2.2/proxygetter.egg-info/SOURCES.txt
+-rw-r--r--   0 VEAR4001   (502) staff       (20)        1 2024-05-26 18:03:18.000000 proxygetter-0.2.2/proxygetter.egg-info/dependency_links.txt
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      242 2024-05-26 18:03:18.000000 proxygetter-0.2.2/proxygetter.egg-info/requires.txt
+-rw-r--r--   0 VEAR4001   (502) staff       (20)       18 2024-05-26 18:03:18.000000 proxygetter-0.2.2/proxygetter.egg-info/top_level.txt
+-rw-r--r--   0 VEAR4001   (502) staff       (20)       49 2024-05-26 17:45:00.000000 proxygetter-0.2.2/pyproject.toml
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      242 2024-05-26 17:58:35.000000 proxygetter-0.2.2/requirements.txt
+-rw-r--r--   0 VEAR4001   (502) staff       (20)       38 2024-05-26 18:03:18.925246 proxygetter-0.2.2/setup.cfg
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     1158 2024-05-26 18:01:04.000000 proxygetter-0.2.2/setup.py
+drwxr-xr-x   0 VEAR4001   (502) staff       (20)        0 2024-05-26 18:03:18.924553 proxygetter-0.2.2/tests/
+-rw-r--r--   0 VEAR4001   (502) staff       (20)        0 2024-05-26 17:45:00.000000 proxygetter-0.2.2/tests/__init__.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)      923 2024-05-26 17:45:00.000000 proxygetter-0.2.2/tests/test_proxy.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)        5 2024-05-26 17:45:00.000000 proxygetter-0.2.2/tests/test_proxy_manager.py
+-rw-r--r--   0 VEAR4001   (502) staff       (20)     1941 2024-05-26 17:45:00.000000 proxygetter-0.2.2/tests/test_utils.py
```

### Comparing `proxygetter-0.2.1/LICENSE` & `proxygetter-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Arthur Verrez
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023 Arthur Verrez
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `proxygetter-0.2.1/PKG-INFO` & `proxygetter-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: proxygetter
-Version: 0.2.1
-Summary: A utility to get and filter free proxies
-Home-page: https://github.com/ArthurVerrez/proxygetter
-Author: Arthur Verrez
-Author-email: macdouglass@outlook.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: aiosignal==1.3.1
-Requires-Dist: async-timeout==4.0.3
-Requires-Dist: attrs==23.1.0
-Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.2.0
-Requires-Dist: frozenlist==1.4.0
-Requires-Dist: idna==3.4
-Requires-Dist: multidict==6.0.4
-Requires-Dist: nest-asyncio==1.5.8
-Requires-Dist: requests==2.31.0
-Requires-Dist: soupsieve==2.5
-Requires-Dist: urllib3==2.0.4
-Requires-Dist: yarl==1.9.2
-
-# proxygetter
-
-## Description
-
-`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
-
-## Installation
-
-Install the package via pip:
-
-```bash
-pip install proxygetter
-```
-
-## Features
-
-### Proxy Management
-Manage your proxies with ease using the `ProxyManager` class.
-
-```python
-from proxygetter import ProxyManager
-manager = ProxyManager()
-```
-
-#### Asynchronous Filtering
-Filter proxies based on their validity asynchronously.
-
-```python
-valid_proxies = manager.filter_with_validity(url="http://example.com")
-```
-
-### Proxy Information
-Access details about each proxy through the `Proxy` class.
-
-```python
-proxy = valid_proxies[0]
-print(proxy.get_requests_format())
-print(proxy.get_selenium_format())
-```
-
-### Advanced Filters
-
-Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
-
-```python
-filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
-```
-
-### Fetch a Random Proxy
-
-You can fetch a random proxy based on specified filters.
-
-```python
-random_proxy = manager.get_random_proxy(country_code='US', https=True)
-```
-
-### Environment Configuration
-
-Configure default user agent and timeout using environment variables.
-
-```bash
-export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
-export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
-```
-
-## License
-
-This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Upcoming Features
-
-- Proxy blacklisting
-- Additional proxy databases
-- Enhanced documentation and examples
-
-Feel free to contribute or suggest improvements.
+Metadata-Version: 2.1
+Name: proxygetter
+Version: 0.2.2
+Summary: A utility to get and filter free proxies
+Home-page: https://github.com/ArthurVerrez/proxygetter
+Author: Arthur Verrez
+Author-email: macdouglass@outlook.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.9.1
+Requires-Dist: aiosignal==1.3.1
+Requires-Dist: async-timeout==4.0.3
+Requires-Dist: attrs==23.1.0
+Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: certifi==2023.7.22
+Requires-Dist: charset-normalizer==3.2.0
+Requires-Dist: frozenlist==1.4.0
+Requires-Dist: idna==3.4
+Requires-Dist: nest-asyncio==1.5.8
+Requires-Dist: requests==2.31.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: urllib3==2.0.4
+Requires-Dist: yarl==1.9.2
+
+# proxygetter
+
+## Description
+
+`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
+
+## Installation
+
+Install the package via pip:
+
+```bash
+pip install proxygetter
+```
+
+## Features
+
+### Proxy Management
+Manage your proxies with ease using the `ProxyManager` class.
+
+```python
+from proxygetter import ProxyManager
+manager = ProxyManager()
+```
+
+#### Asynchronous Filtering
+Filter proxies based on their validity asynchronously.
+
+```python
+valid_proxies = manager.filter_with_validity(url="http://example.com")
+```
+
+### Proxy Information
+Access details about each proxy through the `Proxy` class.
+
+```python
+proxy = valid_proxies[0]
+print(proxy.get_requests_format())
+print(proxy.get_selenium_format())
+```
+
+### Advanced Filters
+
+Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
+
+```python
+filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
+```
+
+### Fetch a Random Proxy
+
+You can fetch a random proxy based on specified filters.
+
+```python
+random_proxy = manager.get_random_proxy(country_code='US', https=True)
+```
+
+### Environment Configuration
+
+Configure default user agent and timeout using environment variables.
+
+```bash
+export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
+export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
+```
+
+## License
+
+This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
+
+## Upcoming Features
+
+- Proxy blacklisting
+- Additional proxy databases
+- Enhanced documentation and examples
+
+Feel free to contribute or suggest improvements.
```

### Comparing `proxygetter-0.2.1/README.md` & `proxygetter-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# proxygetter
-
-## Description
-
-`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
-
-## Installation
-
-Install the package via pip:
-
-```bash
-pip install proxygetter
-```
-
-## Features
-
-### Proxy Management
-Manage your proxies with ease using the `ProxyManager` class.
-
-```python
-from proxygetter import ProxyManager
-manager = ProxyManager()
-```
-
-#### Asynchronous Filtering
-Filter proxies based on their validity asynchronously.
-
-```python
-valid_proxies = manager.filter_with_validity(url="http://example.com")
-```
-
-### Proxy Information
-Access details about each proxy through the `Proxy` class.
-
-```python
-proxy = valid_proxies[0]
-print(proxy.get_requests_format())
-print(proxy.get_selenium_format())
-```
-
-### Advanced Filters
-
-Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
-
-```python
-filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
-```
-
-### Fetch a Random Proxy
-
-You can fetch a random proxy based on specified filters.
-
-```python
-random_proxy = manager.get_random_proxy(country_code='US', https=True)
-```
-
-### Environment Configuration
-
-Configure default user agent and timeout using environment variables.
-
-```bash
-export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
-export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
-```
-
-## License
-
-This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Upcoming Features
-
-- Proxy blacklisting
-- Additional proxy databases
-- Enhanced documentation and examples
-
+# proxygetter
+
+## Description
+
+`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
+
+## Installation
+
+Install the package via pip:
+
+```bash
+pip install proxygetter
+```
+
+## Features
+
+### Proxy Management
+Manage your proxies with ease using the `ProxyManager` class.
+
+```python
+from proxygetter import ProxyManager
+manager = ProxyManager()
+```
+
+#### Asynchronous Filtering
+Filter proxies based on their validity asynchronously.
+
+```python
+valid_proxies = manager.filter_with_validity(url="http://example.com")
+```
+
+### Proxy Information
+Access details about each proxy through the `Proxy` class.
+
+```python
+proxy = valid_proxies[0]
+print(proxy.get_requests_format())
+print(proxy.get_selenium_format())
+```
+
+### Advanced Filters
+
+Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
+
+```python
+filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
+```
+
+### Fetch a Random Proxy
+
+You can fetch a random proxy based on specified filters.
+
+```python
+random_proxy = manager.get_random_proxy(country_code='US', https=True)
+```
+
+### Environment Configuration
+
+Configure default user agent and timeout using environment variables.
+
+```bash
+export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
+export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
+```
+
+## License
+
+This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
+
+## Upcoming Features
+
+- Proxy blacklisting
+- Additional proxy databases
+- Enhanced documentation and examples
+
 Feel free to contribute or suggest improvements.
```

### Comparing `proxygetter-0.2.1/proxygetter/proxy.py` & `proxygetter-0.2.2/proxygetter/proxy.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import os
-
-PROXY_URL_CHECKER_USER_AGENT_HEADER = os.getenv(
-    "PROXY_URL_CHECKER_USER_AGENT",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
-)
-PROXY_URL_CHECKER_TIMEOUT = os.getenv("PROXY_URL_CHECKER_TIMEOUT", 5)
-
-
-class Proxy:
-    def __init__(self, proxy_object):
-        self.ip = proxy_object["ip"]
-        self.port = proxy_object["port"]
-        self.anonymity = proxy_object["anonymity"]
-        self.country = proxy_object["country"]
-        self.country_code = proxy_object["code"]
-        self.https = proxy_object["https"]
-        self.google = proxy_object["google"]
-        self.last_checked = proxy_object["last_checked"]
-
-    def get_requests_format(self):
-        return f"http://{self.ip}:{self.port}"
-
-    def get_selenium_format(self):
-        return f"{self.ip}:{self.port}"
-
-    def blacklist(self):
-        pass
-
-    async def fetch_is_valid(self, session, url):
-        """
-        Fetch the url with the proxy and check if the status code is 200
-        If it is, return the proxy, else return None
-        """
-        try:
-            async with session.get(
-                url,
-                proxy=self.get_requests_format(),
-                headers={"User-Agent": PROXY_URL_CHECKER_USER_AGENT_HEADER},
-                timeout=PROXY_URL_CHECKER_TIMEOUT,
-            ) as response:
-                if response.status == 200:
-                    return self
-                return None
-        except:
-            return None
-
-    def __str__(self):
-        return self.get_requests_format()
-
-    def __repr__(self):
-        return f"{self.ip}:{self.port}, {self.country_code}, {self.anonymity}, {self.https}, {self.google}, {self.last_checked}"
+import os
+
+PROXY_URL_CHECKER_USER_AGENT_HEADER = os.getenv(
+    "PROXY_URL_CHECKER_USER_AGENT",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
+)
+PROXY_URL_CHECKER_TIMEOUT = os.getenv("PROXY_URL_CHECKER_TIMEOUT", 5)
+
+
+class Proxy:
+    def __init__(self, proxy_object):
+        self.ip = proxy_object["ip"]
+        self.port = proxy_object["port"]
+        self.anonymity = proxy_object["anonymity"]
+        self.country = proxy_object["country"]
+        self.country_code = proxy_object["code"]
+        self.https = proxy_object["https"]
+        self.google = proxy_object["google"]
+        self.last_checked = proxy_object["last_checked"]
+
+    def get_requests_format(self):
+        return f"http://{self.ip}:{self.port}"
+
+    def get_selenium_format(self):
+        return f"{self.ip}:{self.port}"
+
+    def blacklist(self):
+        pass
+
+    async def fetch_is_valid(self, session, url):
+        """
+        Fetch the url with the proxy and check if the status code is 200
+        If it is, return the proxy, else return None
+        """
+        try:
+            async with session.get(
+                url,
+                proxy=self.get_requests_format(),
+                headers={"User-Agent": PROXY_URL_CHECKER_USER_AGENT_HEADER},
+                timeout=PROXY_URL_CHECKER_TIMEOUT,
+            ) as response:
+                if response.status == 200:
+                    return self
+                return None
+        except:
+            return None
+
+    def __str__(self):
+        return self.get_requests_format()
+
+    def __repr__(self):
+        return f"{self.ip}:{self.port}, {self.country_code}, {self.anonymity}, {self.https}, {self.google}, {self.last_checked}"
```

### Comparing `proxygetter-0.2.1/proxygetter/utils.py` & `proxygetter-0.2.2/proxygetter/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-from typing import List, Dict, Union, Optional
-import requests
-from bs4 import BeautifulSoup
-import re
-
-
-def parse_time_to_seconds(time_string: str) -> Optional[int]:
-    """
-    Convert a time string to time in seconds.
-
-    Args:
-        time_string (str): Time string in human-readable format, e.g., '15 secs ago'.
-
-    Returns:
-        Optional[int]: Time in seconds. Returns 0 for any invalid string format.
-    """
-    try:
-        total_seconds = 0
-        for value, unit in re.findall(r"(\d+) (\w+)", time_string):
-            value = int(value)
-
-            if "sec" in unit:
-                total_seconds += value
-            elif "min" in unit:
-                total_seconds += value * 60
-            elif "hour" in unit:
-                total_seconds += value * 3600
-            elif "day" in unit:
-                total_seconds += value * 86400
-
-        return total_seconds
-    except:
-        return None
-
-
-def scrap_sslproxies() -> List[Dict[str, Union[str, bool, int]]]:
-    URL = "https://www.sslproxies.org/"
-    LINE_SELECTOR = "#list > div > div.table-responsive > div > table > tbody > tr"
-    COLUMNS = [
-        "ip",
-        "port",
-        "code",
-        "country",
-        "anonymity",
-        "google",
-        "https",
-        "last_checked",
-    ]
-    response = requests.get(URL)
-    soup = BeautifulSoup(response.content, "html.parser")
-    lines = soup.select(LINE_SELECTOR)
-
-    return [
-        {
-            COLUMNS[i]: parse_time_to_seconds(col.text)
-            if COLUMNS[i] == "last_checked"
-            else (True if col.text == "yes" else False)
-            if COLUMNS[i] in ["google", "https"]
-            else col.text
-            for i, col in enumerate(line.select("td"))
-        }
-        for line in lines
-    ]
-
-
-def filter_proxies(
-    all_proxies: List[Dict[str, Union[str, bool, int]]],
-    country_code: Optional[str] = None,
-    anonymity: Optional[str] = None,
-    https: Optional[bool] = None,
-    google: Optional[bool] = None,
-    last_checked_max: Optional[int] = None,
-) -> List[Dict[str, Union[str, bool, int]]]:
-    return [
-        proxy
-        for proxy in all_proxies
-        if all(
-            proxy.get(key) == val
-            for key, val in {
-                "code": country_code,
-                "anonymity": anonymity,
-                "https": https,
-                "google": google,
-            }.items()
-            if val is not None
-        )
-        and (
-            last_checked_max is None
-            or (
-                proxy.get("last_checked") is not None
-                and proxy["last_checked"] <= last_checked_max
-            )
-        )
-    ]
-
-
-def get_proxies(
-    country_code: Optional[str] = None,
-    anonymity: Optional[str] = None,
-    https: Optional[bool] = None,
-    google: Optional[bool] = None,
-    last_checked_max: Optional[int] = None,
-) -> List[Dict[str, Union[str, bool, int]]]:
-    all_proxies = scrap_sslproxies()
-    return filter_proxies(
-        all_proxies, country_code, anonymity, https, google, last_checked_max
-    )
+from typing import List, Dict, Union, Optional
+import requests
+from bs4 import BeautifulSoup
+import re
+
+
+def parse_time_to_seconds(time_string: str) -> Optional[int]:
+    """
+    Convert a time string to time in seconds.
+
+    Args:
+        time_string (str): Time string in human-readable format, e.g., '15 secs ago'.
+
+    Returns:
+        Optional[int]: Time in seconds. Returns 0 for any invalid string format.
+    """
+    try:
+        total_seconds = 0
+        for value, unit in re.findall(r"(\d+) (\w+)", time_string):
+            value = int(value)
+
+            if "sec" in unit:
+                total_seconds += value
+            elif "min" in unit:
+                total_seconds += value * 60
+            elif "hour" in unit:
+                total_seconds += value * 3600
+            elif "day" in unit:
+                total_seconds += value * 86400
+
+        return total_seconds
+    except:
+        return None
+
+
+def scrap_sslproxies() -> List[Dict[str, Union[str, bool, int]]]:
+    URL = "https://www.sslproxies.org/"
+    LINE_SELECTOR = "#list > div > div.table-responsive > div > table > tbody > tr"
+    COLUMNS = [
+        "ip",
+        "port",
+        "code",
+        "country",
+        "anonymity",
+        "google",
+        "https",
+        "last_checked",
+    ]
+    response = requests.get(URL)
+    soup = BeautifulSoup(response.content, "html.parser")
+    lines = soup.select(LINE_SELECTOR)
+
+    return [
+        {
+            COLUMNS[i]: parse_time_to_seconds(col.text)
+            if COLUMNS[i] == "last_checked"
+            else (True if col.text == "yes" else False)
+            if COLUMNS[i] in ["google", "https"]
+            else col.text
+            for i, col in enumerate(line.select("td"))
+        }
+        for line in lines
+    ]
+
+
+def filter_proxies(
+    all_proxies: List[Dict[str, Union[str, bool, int]]],
+    country_code: Optional[str] = None,
+    anonymity: Optional[str] = None,
+    https: Optional[bool] = None,
+    google: Optional[bool] = None,
+    last_checked_max: Optional[int] = None,
+) -> List[Dict[str, Union[str, bool, int]]]:
+    return [
+        proxy
+        for proxy in all_proxies
+        if all(
+            proxy.get(key) == val
+            for key, val in {
+                "code": country_code,
+                "anonymity": anonymity,
+                "https": https,
+                "google": google,
+            }.items()
+            if val is not None
+        )
+        and (
+            last_checked_max is None
+            or (
+                proxy.get("last_checked") is not None
+                and proxy["last_checked"] <= last_checked_max
+            )
+        )
+    ]
+
+
+def get_proxies(
+    country_code: Optional[str] = None,
+    anonymity: Optional[str] = None,
+    https: Optional[bool] = None,
+    google: Optional[bool] = None,
+    last_checked_max: Optional[int] = None,
+) -> List[Dict[str, Union[str, bool, int]]]:
+    all_proxies = scrap_sslproxies()
+    return filter_proxies(
+        all_proxies, country_code, anonymity, https, google, last_checked_max
+    )
```

### Comparing `proxygetter-0.2.1/proxygetter.egg-info/PKG-INFO` & `proxygetter-0.2.2/proxygetter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: proxygetter
-Version: 0.2.1
-Summary: A utility to get and filter free proxies
-Home-page: https://github.com/ArthurVerrez/proxygetter
-Author: Arthur Verrez
-Author-email: macdouglass@outlook.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: aiosignal==1.3.1
-Requires-Dist: async-timeout==4.0.3
-Requires-Dist: attrs==23.1.0
-Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.2.0
-Requires-Dist: frozenlist==1.4.0
-Requires-Dist: idna==3.4
-Requires-Dist: multidict==6.0.4
-Requires-Dist: nest-asyncio==1.5.8
-Requires-Dist: requests==2.31.0
-Requires-Dist: soupsieve==2.5
-Requires-Dist: urllib3==2.0.4
-Requires-Dist: yarl==1.9.2
-
-# proxygetter
-
-## Description
-
-`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
-
-## Installation
-
-Install the package via pip:
-
-```bash
-pip install proxygetter
-```
-
-## Features
-
-### Proxy Management
-Manage your proxies with ease using the `ProxyManager` class.
-
-```python
-from proxygetter import ProxyManager
-manager = ProxyManager()
-```
-
-#### Asynchronous Filtering
-Filter proxies based on their validity asynchronously.
-
-```python
-valid_proxies = manager.filter_with_validity(url="http://example.com")
-```
-
-### Proxy Information
-Access details about each proxy through the `Proxy` class.
-
-```python
-proxy = valid_proxies[0]
-print(proxy.get_requests_format())
-print(proxy.get_selenium_format())
-```
-
-### Advanced Filters
-
-Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
-
-```python
-filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
-```
-
-### Fetch a Random Proxy
-
-You can fetch a random proxy based on specified filters.
-
-```python
-random_proxy = manager.get_random_proxy(country_code='US', https=True)
-```
-
-### Environment Configuration
-
-Configure default user agent and timeout using environment variables.
-
-```bash
-export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
-export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
-```
-
-## License
-
-This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-## Upcoming Features
-
-- Proxy blacklisting
-- Additional proxy databases
-- Enhanced documentation and examples
-
-Feel free to contribute or suggest improvements.
+Metadata-Version: 2.1
+Name: proxygetter
+Version: 0.2.2
+Summary: A utility to get and filter free proxies
+Home-page: https://github.com/ArthurVerrez/proxygetter
+Author: Arthur Verrez
+Author-email: macdouglass@outlook.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.9.1
+Requires-Dist: aiosignal==1.3.1
+Requires-Dist: async-timeout==4.0.3
+Requires-Dist: attrs==23.1.0
+Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: certifi==2023.7.22
+Requires-Dist: charset-normalizer==3.2.0
+Requires-Dist: frozenlist==1.4.0
+Requires-Dist: idna==3.4
+Requires-Dist: nest-asyncio==1.5.8
+Requires-Dist: requests==2.31.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: urllib3==2.0.4
+Requires-Dist: yarl==1.9.2
+
+# proxygetter
+
+## Description
+
+`proxygetter` is a Python library that provides a fast and customizable way to scrape, filter, and manage proxies. It's powered by asyncio and aiohttp to validate proxies asynchronously. Originally designed to scrape from [sslproxies.org](https://www.sslproxies.org/), it now supports customizable sources and multiple filters.
+
+## Installation
+
+Install the package via pip:
+
+```bash
+pip install proxygetter
+```
+
+## Features
+
+### Proxy Management
+Manage your proxies with ease using the `ProxyManager` class.
+
+```python
+from proxygetter import ProxyManager
+manager = ProxyManager()
+```
+
+#### Asynchronous Filtering
+Filter proxies based on their validity asynchronously.
+
+```python
+valid_proxies = manager.filter_with_validity(url="http://example.com")
+```
+
+### Proxy Information
+Access details about each proxy through the `Proxy` class.
+
+```python
+proxy = valid_proxies[0]
+print(proxy.get_requests_format())
+print(proxy.get_selenium_format())
+```
+
+### Advanced Filters
+
+Get proxies using advanced filters like country code, anonymity, https support, Google compatibility, and last checked time.
+
+```python
+filtered_proxies = manager.get_proxies(country_code='US', anonymity='elite proxy', https=True, google=True, last_checked_max=600)
+```
+
+### Fetch a Random Proxy
+
+You can fetch a random proxy based on specified filters.
+
+```python
+random_proxy = manager.get_random_proxy(country_code='US', https=True)
+```
+
+### Environment Configuration
+
+Configure default user agent and timeout using environment variables.
+
+```bash
+export PROXY_URL_CHECKER_USER_AGENT=your_user_agent
+export PROXY_URL_CHECKER_TIMEOUT=your_timeout_value
+```
+
+## License
+
+This project is under the MIT License - see the [LICENSE](LICENSE) file for details.
+
+## Upcoming Features
+
+- Proxy blacklisting
+- Additional proxy databases
+- Enhanced documentation and examples
+
+Feel free to contribute or suggest improvements.
```

