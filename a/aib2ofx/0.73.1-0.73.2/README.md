# Comparing `tmp/aib2ofx-0.73.1.tar.gz` & `tmp/aib2ofx-0.73.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib2ofx-0.73.1.tar", last modified: Mon Dec  6 23:02:10 2021, max compression
+gzip compressed data, was "aib2ofx-0.73.2.tar", max compression
```

## Comparing `aib2ofx-0.73.1.tar` & `aib2ofx-0.73.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1529 2020-06-09 18:55:30.000000 aib2ofx-0.73.1/LICENSE
--rw-r--r--   0        0        0     2776 2021-02-28 14:25:49.849073 aib2ofx-0.73.1/README.md
--rw-r--r--   0        0        0        0 2020-06-09 18:55:30.000000 aib2ofx-0.73.1/aib2ofx/__init__.py
--rw-r--r--   0        0        0    11472 2021-12-06 23:01:45.059759 aib2ofx-0.73.1/aib2ofx/aib.py
--rw-r--r--   0        0        0      864 2020-12-28 22:09:52.254227 aib2ofx-0.73.1/aib2ofx/cfg.py
--rw-r--r--   0        0        0     3248 2020-12-28 22:10:10.714227 aib2ofx-0.73.1/aib2ofx/cli.py
--rw-r--r--   0        0        0     3870 2021-12-05 18:56:20.899731 aib2ofx-0.73.1/aib2ofx/ofx.py
--rw-r--r--   0        0        0      625 2021-12-06 23:01:45.059759 aib2ofx-0.73.1/pyproject.toml
--rw-r--r--   0        0        0     3668 2021-12-06 23:02:10.618272 aib2ofx-0.73.1/setup.py
--rw-r--r--   0        0        0     3506 2021-12-06 23:02:10.618572 aib2ofx-0.73.1/PKG-INFO
+-rw-r--r--   0        0        0     1529 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/LICENSE
+-rw-r--r--   0        0        0     2776 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/README.md
+-rw-r--r--   0        0        0        0 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/aib2ofx/__init__.py
+-rw-r--r--   0        0        0    11472 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/aib2ofx/aib.py
+-rw-r--r--   0        0        0      864 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/aib2ofx/cfg.py
+-rw-r--r--   0        0        0     3248 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/aib2ofx/cli.py
+-rw-r--r--   0        0        0     3870 2023-01-25 21:14:13.000000 aib2ofx-0.73.2/aib2ofx/ofx.py
+-rw-r--r--   0        0        0      631 2024-05-26 21:42:54.552872 aib2ofx-0.73.2/pyproject.toml
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 aib2ofx-0.73.2/setup.py
+-rw-r--r--   0        0        0     3353 1970-01-01 00:00:00.000000 aib2ofx-0.73.2/PKG-INFO
```

### Comparing `aib2ofx-0.73.1/LICENSE` & `aib2ofx-0.73.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/README.md` & `aib2ofx-0.73.2/README.md`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/aib2ofx/aib.py` & `aib2ofx-0.73.2/aib2ofx/aib.py`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/aib2ofx/cfg.py` & `aib2ofx-0.73.2/aib2ofx/cfg.py`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/aib2ofx/cli.py` & `aib2ofx-0.73.2/aib2ofx/cli.py`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/aib2ofx/ofx.py` & `aib2ofx-0.73.2/aib2ofx/ofx.py`

 * *Files identical despite different names*

### Comparing `aib2ofx-0.73.1/pyproject.toml` & `aib2ofx-0.73.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.black]
 skip-string-normalization = true
 
 [tool.poetry]
 name = 'aib2ofx'
-version = '0.73.1'
+version = '0.73.2'
 description = 'Download data from aib.ie in OFX format'
 authors = ['Jakub Turski <yacoob@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/yacoob/aib2ofx'
 
 [tool.poetry.dependencies]
-python = '^3.6'
-mechanicalsoup = '^1.1'
-python-dateutil = '^2.8.1'
+python = '>=3.11'
+mechanicalsoup = '^1.3'
+python-dateutil = '^2.9.0'
 
 [tool.poetry.dev-dependencies]
-black = '^20.8b1'
-ipython = '>=1'
-pylint = '^2.6.0'
-rope = "^0.18.0"
+black = '^24.4.2'
+ipython = '^8.24.0'
+pylint = '^3.2.2'
+rope = '^1.13.0'
 
 [tool.poetry.scripts]
 aib2ofx = 'aib2ofx.cli:main'
 
 [build-system]
 requires = ['poetry-core>=1.0.0']
 build-backend = 'poetry.core.masonry.api'
```

### Comparing `aib2ofx-0.73.1/setup.py` & `aib2ofx-0.73.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['aib2ofx']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['mechanicalsoup>=1.1,<2.0', 'python-dateutil>=2.8.1,<3.0.0']
+['mechanicalsoup>=1.3,<2.0', 'python-dateutil>=2.9.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['aib2ofx = aib2ofx.cli:main']}
 
 setup_kwargs = {
     'name': 'aib2ofx',
-    'version': '0.73.1',
+    'version': '0.73.2',
     'description': 'Download data from aib.ie in OFX format',
     'long_description': '# aib2ofx\n\n...or how to grab transaction data out of AIB\'s online interface, and format it\ninto `OFX` file.\n\n**NOTE:** Last AIB login update (Feb\' 2021) made me realise how brittle the\noverall machinery here is. The code that works around Web Storage API use is\nugly and likely to break. The most likely road forward for this project is to\ndecouple it into [ofxstatement](https://github.com/kedder/ofxstatement) plugin\nand (maybe) Selenium-powered CSV acquisition script. The former will be easy,\nthe latter will most likely be a nightmare to maintain and install, unless you\nenjoy having your banking details pipe through an arbitrary docker image.\n\nTime will tell.\n\n## Installation\n\n    python3 -mvenv aib2ofx\n    source aib2ofx/bin/activate\n    pip3 install aib2ofx\n\nThis will create a virtualenv for `aib2ofx`, fetch its code then install it with\nall dependencies. Once that completes, you\'ll find `aib2ofx` executable in the\n`bin` directory of this new virtualenv.\n\n## Usage\n\nCreate a `~/.aib2ofx.json` file, with AIB login details.\nSet the permission bits to 0600 to prevent other system users from reading it.\n\n    touch ~/.aib2ofx.json\n    chmod 0600 ~/.aib2ofx.json\n\nIt has a JSON format, single object with one key per AIB login you want to use.\n\n    {\n        "bradmajors": {\n            "regNumber": "12345678",\n            "pin": "12345"\n        }\n    }\n\nThe fields are as follows:\n\n* regNumber\n    > Your AIB registered number.\n\n* pin\n    > Your five digit PIN.\n\nYou can put more than one set of credentials in the file; the script\nwill download data for all accounts for all logins.\n\n    {\n        "bradmajors": {\n            "regNumber": "12345678",\n            "pin": "12345"\n        },\n        "janetweiss": {\n            "regNumber": "87654321",\n            "pin": "54321"\n        }\n    }\n\nNote that there\'s no comma after the last account details.\n\nOnce you\'ve prepared that config file, run:\n\n    aib2ofx -d /output/directory\n\nThe script should connect to AIB, log in using provided credentials,\niterate through all accounts, and save each of those to a separate\nfile located in `/output/directory`.\n\n## Guarantee\n\nThere is none.\n\nI\'ve written that script with my best intentions, it\'s not malicious,\nit\'s not sending the data anywhere, it\'s not doing anything nasty. I\'m\nusing it day to day to get data about my AIB accounts into a financial\nprogram that I use. It should work for you as good as it works for\nme. See the `LICENSE` file for more details.\n\n## Development\n\naib2ofx works only with python 3.\n\nIn order to set up a dev environment clone the repository, get\n[poetry](https://python-poetry.org/docs/#installation)\nand run `poetry install`. This will create a virtualenv with all\ndependencies installed. You can activate it with `poetry shell`.\n',
     'author': 'Jakub Turski',
     'author_email': 'yacoob@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/yacoob/aib2ofx',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `aib2ofx-0.73.1/PKG-INFO` & `aib2ofx-0.73.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: aib2ofx
-Version: 0.73.1
+Version: 0.73.2
 Summary: Download data from aib.ie in OFX format
 Home-page: https://github.com/yacoob/aib2ofx
 License: MIT
 Author: Jakub Turski
 Author-email: yacoob@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: mechanicalsoup (>=1.1,<2.0)
-Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: mechanicalsoup (>=1.3,<2.0)
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Project-URL: Repository, https://github.com/yacoob/aib2ofx
 Description-Content-Type: text/markdown
 
 # aib2ofx
 
 ...or how to grab transaction data out of AIB's online interface, and format it
 into `OFX` file.
```

