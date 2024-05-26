# Comparing `tmp/virustotal_python-1.0.2.tar.gz` & `tmp/virustotal_python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virustotal_python-1.0.2.tar", max compression
+gzip compressed data, was "virustotal_python-1.1.0.tar", max compression
```

## Comparing `virustotal_python-1.0.2.tar` & `virustotal_python-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-02-08 20:15:33.311072 virustotal_python-1.0.2/LICENSE
--rw-r--r--   0        0        0     5015 2023-02-08 20:15:33.311072 virustotal_python-1.0.2/README.md
--rw-r--r--   0        0        0     1042 2023-02-08 20:15:33.315072 virustotal_python-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      390 2023-02-08 20:15:33.315072 virustotal_python-1.0.2/virustotal_python/__init__.py
--rw-r--r--   0        0        0    14331 2023-02-08 20:15:33.315072 virustotal_python-1.0.2/virustotal_python/virustotal.py
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 virustotal_python-1.0.2/setup.py
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 virustotal_python-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-26 20:05:59.504681 virustotal_python-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5015 2024-05-26 20:05:59.504681 virustotal_python-1.1.0/README.md
+-rw-r--r--   0        0        0     1210 2024-05-26 20:05:59.504681 virustotal_python-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      391 2024-05-26 20:05:59.504681 virustotal_python-1.1.0/virustotal_python/__init__.py
+-rw-r--r--   0        0        0    14338 2024-05-26 20:05:59.504681 virustotal_python-1.1.0/virustotal_python/virustotal.py
+-rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 virustotal_python-1.1.0/PKG-INFO
```

### Comparing `virustotal_python-1.0.2/LICENSE` & `virustotal_python-1.1.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 dbrennand
+Copyright (c) 2024 Daniel Brennand
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `virustotal_python-1.0.2/README.md` & `virustotal_python-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `virustotal_python-1.0.2/pyproject.toml` & `virustotal_python-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virustotal-python"
-version = "1.0.2"
+version = "1.1.0"
 description = "A Python library to interact with the public VirusTotal v3 and v2 APIs."
 authors = ["dbrennand"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbrennand/virustotal-python"
 repository = "https://github.com/dbrennand/virustotal-python"
 keywords = [
@@ -16,28 +16,32 @@
     "v2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 exclude = [".gitignore"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-requests = {version = "^2.26.0", extras = ["socks"]}
+python = "^3.12"
+requests = { version = "^2.31.0" }
+PySocks = { version = "^1.7.1", optional = true }
 
 [tool.poetry.extras]
-socks = ["PySocks^1.7.1"]
+socks = ["PySocks"]
 
 [tool.poetry.dev-dependencies]
-black = "22.3.0"
-twine = "^3.5.0"
-pytest = "^6.2.5"
-pytest-mock = "^3.6.1"
-requests-mock = "^1.9.3"
-pytest-cov = "^3.0.0"
+black = "^24.4.2"
+twine = "^5.1.0"
+pytest = "^8.2.0"
+pytest-mock = "^3.14.0"
+requests-mock = "^1.12.1"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `virustotal_python-1.0.2/virustotal_python/virustotal.py` & `virustotal_python-1.1.0/virustotal_python/virustotal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 MIT License
 
-Copyright (c) 2023 dbrennand
+Copyright (c) 2024 Daniel Brennand
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -17,14 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 import requests
 import os
 from typing import Union
 from json.decoder import JSONDecodeError
 
 
 class VirustotalError(Exception):
@@ -263,22 +264,22 @@
         self.TIMEOUT = TIMEOUT
         # Declare appropriate variables depending on the API_VERSION provided
         if (API_VERSION == "v2") or (API_VERSION == 2):
             self.API_VERSION = API_VERSION
             self.BASEURL = "https://www.virustotal.com/vtapi/v2/"
             self.HEADERS = {
                 "Accept-Encoding": "gzip, deflate",
-                "User-Agent": f"gzip, virustotal-python 1.0.2",
+                "User-Agent": f"gzip, virustotal-python 1.1.0",
             }
         elif (API_VERSION == "v3") or (API_VERSION == 3):
             self.API_VERSION = API_VERSION
             self.BASEURL = "https://www.virustotal.com/api/v3/"
             self.HEADERS = {
                 "Accept-Encoding": "gzip, deflate",
-                "User-Agent": f"gzip, virustotal-python 1.0.2",
+                "User-Agent": f"gzip, virustotal-python 1.1.0",
                 "x-apikey": f"{self.API_KEY}",
             }
         else:
             raise ValueError(
                 f"The API version '{API_VERSION}' is not a valid VirusTotal API version.\nValid API versions are 'v2', 2, 'v3' and 3."
             )
```

### Comparing `virustotal_python-1.0.2/setup.py` & `virustotal_python-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,195 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: virustotal-python
+Version: 1.1.0
+Summary: A Python library to interact with the public VirusTotal v3 and v2 APIs.
+Home-page: https://github.com/dbrennand/virustotal-python
+License: MIT
+Keywords: VirusTotal,Wrapper,Public API,Library,v3,v2
+Author: dbrennand
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: socks
+Requires-Dist: PySocks (>=1.7.1,<2.0.0) ; extra == "socks"
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/dbrennand/virustotal-python
+Description-Content-Type: text/markdown
+
+# virustotal-python 🐍
+![PyPI](https://img.shields.io/pypi/v/virustotal-python.svg?style=flat-square)
+![PyPI Stats](https://img.shields.io/pypi/dm/virustotal-python?color=blue&style=flat-square)
+[![CI](https://github.com/dbrennand/virustotal-python/actions/workflows/ci.yml/badge.svg)](https://github.com/dbrennand/virustotal-python/actions/workflows/ci.yml)
+[![Publish](https://github.com/dbrennand/virustotal-python/actions/workflows/publish.yml/badge.svg)](https://github.com/dbrennand/virustotal-python/actions/workflows/publish.yml)
+
+A Python library to interact with the public VirusTotal v3 and v2 APIs.
+
+> This library is intended to be used with the public VirusTotal APIs. However, it *could* be used to interact with premium API endpoints as well.
+>
+> It is highly recommended that you use the VirusTotal v3 API as it is the "default and encouraged way to programmatically interact with VirusTotal".
+
+## Installation 🛠
+
+```bash
+# PyPi
+pip install virustotal-python
+# Manually
+pip install .
+# Poetry
+poetry install --no-dev
+```
+
+## Get a VirusTotal API Key 🔑
+
+[Sign up](https://www.virustotal.com/gui/join-us) for a VirusTotal account. Then, view your VirusTotal API key.
+
+![VirusTotal view API key](images/APIKey.png)
+
+## Getting Started
+
+```python
+import virustotal_python
+
+with virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:
+    # Your code here...
+
+# Use the (old) VirusTotal version 2 API
+with virustotal_python.Virustotal(
+    API_KEY="<VirusTotal API Key>", API_VERSION=2
+) as vtotal:
+    # Your code here...
+
+# You can also set proxies and timeouts for requests made by the library
+# NOTE: To use proxies, you must have the PySocks extra installed
+with virustotal_python.Virustotal(
+    API_KEY="<VirusTotal API Key>",
+    PROXIES={"http": "http://10.10.1.10:3128", "https": "https://10.10.1.10:1080"},
+    TIMEOUT=5.0,
+) as vtotal:
+    # Your code here...
+
+# You can also omit the API_KEY parameter and provide your
+# API key via the environment variable VIRUSTOTAL_API_KEY
+# Bash: export VIRUSTOTAL_API_KEY="<VirusTotal API Key>"
+# PowerShell: $Env:VIRUSTOTAL_API_KEY = "<VirusTotal API Key>"
+# Then...
+with virustotal_python.Virustotal() as vtotal:
+    # Your code here...
+```
+
+## Code Snippets
+
+> Further usage examples can be found in [examples](examples).
+
+### Send a file for analysis 🔎
+
+```python
+import virustotal_python
+import os.path
+from pprint import pprint
+
+FILE_PATH = "/path/to/file/to/scan.txt"
+
+# Create dictionary containing the file to send for multipart encoding upload
+files = {"file": (os.path.basename(FILE_PATH), open(os.path.abspath(FILE_PATH), "rb"))}
+
+with virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:
+    resp = vtotal.request("files", files=files, method="POST")
+    pprint(resp.json())
+```
+
+### Get information about a file 📁
+
+```python
+import virustotal_python
+from pprint import pprint
+
+# The ID (either SHA-256, SHA-1 or MD5 hash) identifying the file
+FILE_ID = "9f101483662fc071b7c10f81c64bb34491ca4a877191d464ff46fd94c7247115"
+
+with virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:
+    resp = vtotal.request(f"files/{FILE_ID}")
+    pprint(resp.data)
+```
+
+### Send a URL 🔗 for analysis and get the report 📄
+
+```python
+import virustotal_python
+from pprint import pprint
+from base64 import urlsafe_b64encode
+
+url = "ihaveaproblem.info"
+
+with virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:
+    try:
+        resp = vtotal.request("urls", data={"url": url}, method="POST")
+        # Safe encode URL in base64 format
+        # https://developers.virustotal.com/reference/url
+        url_id = urlsafe_b64encode(url.encode()).decode().strip("=")
+        report = vtotal.request(f"urls/{url_id}")
+        pprint(report.object_type)
+        pprint(report.data)
+    except virustotal_python.VirustotalError as err:
+        print(f"Failed to send URL: {url} for analysis and get the report: {err}")
+```
+
+### Get information about a domain:
+
+```python
+import virustotal_python
+from pprint import pprint
+
+domain = "virustotal.com"
+
+with virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:
+    resp = vtotal.request(f"domains/{domain}")
+    pprint(resp.data)
+```
+
+## Development
+
+[Black](https://github.com/psf/black) is used for code formatting.
+
+### Unit Tests
+
+Install the development dependencies using Poetry:
+
+```bash
+poetry install && poetry shell
+```
+
+To run the unit tests, run `pytest` from the root of the project:
+
+```bash
+pytest --cov=virustotal_python
+```
+
+### Publishing a new release
+
+```bash
+# Run from the master branch
+export VERSION=x.x.x
+git commit --allow-empty -m "Publish $VERSION"
+git tag -a $VERSION -m "Version $VERSION"
+git push --tags
+```
+
+## Authors & Contributors
+
+* [**dbrennand**](https://github.com/dbrennand) - *Author*
 
-packages = \
-['virustotal_python']
+* [**smk762**](https://github.com/smk762) - *Contributor*
 
-package_data = \
-{'': ['*']}
+## Changelog
 
-install_requires = \
-['requests[socks]>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'virustotal-python',
-    'version': '1.0.2',
-    'description': 'A Python library to interact with the public VirusTotal v3 and v2 APIs.',
-    'long_description': '# virustotal-python 🐍\n![PyPI](https://img.shields.io/pypi/v/virustotal-python.svg?style=flat-square)\n![PyPI Stats](https://img.shields.io/pypi/dm/virustotal-python?color=blue&style=flat-square)\n[![CI](https://github.com/dbrennand/virustotal-python/actions/workflows/ci.yml/badge.svg)](https://github.com/dbrennand/virustotal-python/actions/workflows/ci.yml)\n[![Publish](https://github.com/dbrennand/virustotal-python/actions/workflows/publish.yml/badge.svg)](https://github.com/dbrennand/virustotal-python/actions/workflows/publish.yml)\n\nA Python library to interact with the public VirusTotal v3 and v2 APIs.\n\n> This library is intended to be used with the public VirusTotal APIs. However, it *could* be used to interact with premium API endpoints as well.\n>\n> It is highly recommended that you use the VirusTotal v3 API as it is the "default and encouraged way to programmatically interact with VirusTotal".\n\n## Installation 🛠\n\n```bash\n# PyPi\npip install virustotal-python\n# Manually\npip install .\n# Poetry\npoetry install --no-dev\n```\n\n## Get a VirusTotal API Key 🔑\n\n[Sign up](https://www.virustotal.com/gui/join-us) for a VirusTotal account. Then, view your VirusTotal API key.\n\n![VirusTotal view API key](images/APIKey.png)\n\n## Getting Started\n\n```python\nimport virustotal_python\n\nwith virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:\n    # Your code here...\n\n# Use the (old) VirusTotal version 2 API\nwith virustotal_python.Virustotal(\n    API_KEY="<VirusTotal API Key>", API_VERSION=2\n) as vtotal:\n    # Your code here...\n\n# You can also set proxies and timeouts for requests made by the library\n# NOTE: To use proxies, you must have the PySocks extra installed\nwith virustotal_python.Virustotal(\n    API_KEY="<VirusTotal API Key>",\n    PROXIES={"http": "http://10.10.1.10:3128", "https": "https://10.10.1.10:1080"},\n    TIMEOUT=5.0,\n) as vtotal:\n    # Your code here...\n\n# You can also omit the API_KEY parameter and provide your\n# API key via the environment variable VIRUSTOTAL_API_KEY\n# Bash: export VIRUSTOTAL_API_KEY="<VirusTotal API Key>"\n# PowerShell: $Env:VIRUSTOTAL_API_KEY = "<VirusTotal API Key>"\n# Then...\nwith virustotal_python.Virustotal() as vtotal:\n    # Your code here...\n```\n\n## Code Snippets\n\n> Further usage examples can be found in [examples](examples).\n\n### Send a file for analysis 🔎\n\n```python\nimport virustotal_python\nimport os.path\nfrom pprint import pprint\n\nFILE_PATH = "/path/to/file/to/scan.txt"\n\n# Create dictionary containing the file to send for multipart encoding upload\nfiles = {"file": (os.path.basename(FILE_PATH), open(os.path.abspath(FILE_PATH), "rb"))}\n\nwith virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:\n    resp = vtotal.request("files", files=files, method="POST")\n    pprint(resp.json())\n```\n\n### Get information about a file 📁\n\n```python\nimport virustotal_python\nfrom pprint import pprint\n\n# The ID (either SHA-256, SHA-1 or MD5 hash) identifying the file\nFILE_ID = "9f101483662fc071b7c10f81c64bb34491ca4a877191d464ff46fd94c7247115"\n\nwith virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:\n    resp = vtotal.request(f"files/{FILE_ID}")\n    pprint(resp.data)\n```\n\n### Send a URL 🔗 for analysis and get the report 📄\n\n```python\nimport virustotal_python\nfrom pprint import pprint\nfrom base64 import urlsafe_b64encode\n\nurl = "ihaveaproblem.info"\n\nwith virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:\n    try:\n        resp = vtotal.request("urls", data={"url": url}, method="POST")\n        # Safe encode URL in base64 format\n        # https://developers.virustotal.com/reference/url\n        url_id = urlsafe_b64encode(url.encode()).decode().strip("=")\n        report = vtotal.request(f"urls/{url_id}")\n        pprint(report.object_type)\n        pprint(report.data)\n    except virustotal_python.VirustotalError as err:\n        print(f"Failed to send URL: {url} for analysis and get the report: {err}")\n```\n\n### Get information about a domain:\n\n```python\nimport virustotal_python\nfrom pprint import pprint\n\ndomain = "virustotal.com"\n\nwith virustotal_python.Virustotal("<VirusTotal API Key>") as vtotal:\n    resp = vtotal.request(f"domains/{domain}")\n    pprint(resp.data)\n```\n\n## Development\n\n[Black](https://github.com/psf/black) is used for code formatting.\n\n### Unit Tests\n\nInstall the development dependencies using Poetry:\n\n```bash\npoetry install && poetry shell\n```\n\nTo run the unit tests, run `pytest` from the root of the project:\n\n```bash\npytest --cov=virustotal_python\n```\n\n### Publishing a new release\n\n```bash\n# Run from the master branch\nexport VERSION=x.x.x\ngit commit --allow-empty -m "Publish $VERSION"\ngit tag -a $VERSION -m "Version $VERSION"\ngit push --tags\n```\n\n## Authors & Contributors\n\n* [**dbrennand**](https://github.com/dbrennand) - *Author*\n\n* [**smk762**](https://github.com/smk762) - *Contributor*\n\n## Changelog\n\nSee the [CHANGELOG](CHANGELOG.md) for details.\n\n## License\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) for details.\n',
-    'author': 'dbrennand',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dbrennand/virustotal-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+See the [CHANGELOG](CHANGELOG.md) for details.
 
+## License
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) for details.
 
-setup(**setup_kwargs)
```

