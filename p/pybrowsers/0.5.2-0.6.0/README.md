# Comparing `tmp/pybrowsers-0.5.2.tar.gz` & `tmp/pybrowsers-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrowsers-0.5.2.tar", max compression
+gzip compressed data, was "pybrowsers-0.6.0.tar", max compression
```

## Comparing `pybrowsers-0.5.2.tar` & `pybrowsers-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1071 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/LICENSE
--rw-r--r--   0        0        0     6433 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/README.md
--rw-r--r--   0        0        0     3022 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/browsers/__init__.py
--rw-r--r--   0        0        0      229 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/browsers/common.py
--rw-r--r--   0        0        0     2110 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/browsers/linux.py
--rw-r--r--   0        0        0     2443 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/browsers/osx.py
--rw-r--r--   0        0        0     3002 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/browsers/windows.py
--rw-r--r--   0        0        0     2249 2022-12-16 17:08:12.375895 pybrowsers-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pybrowsers-0.5.2/setup.py
--rw-r--r--   0        0        0     7890 1970-01-01 00:00:00.000000 pybrowsers-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-26 13:46:19.903488 pybrowsers-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6434 2024-05-26 13:46:19.903488 pybrowsers-0.6.0/README.md
+-rw-r--r--   0        0        0     3022 2024-05-26 13:46:19.903488 pybrowsers-0.6.0/browsers/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-26 13:46:19.903488 pybrowsers-0.6.0/browsers/common.py
+-rw-r--r--   0        0        0     2110 2024-05-26 13:46:19.907488 pybrowsers-0.6.0/browsers/linux.py
+-rw-r--r--   0        0        0     2443 2024-05-26 13:46:19.907488 pybrowsers-0.6.0/browsers/osx.py
+-rw-r--r--   0        0        0     3002 2024-05-26 13:46:19.907488 pybrowsers-0.6.0/browsers/windows.py
+-rw-r--r--   0        0        0     2219 2024-05-26 13:46:19.907488 pybrowsers-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 pybrowsers-0.6.0/PKG-INFO
```

### Comparing `pybrowsers-0.5.2/LICENSE` & `pybrowsers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybrowsers-0.5.2/README.md` & `pybrowsers-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         <td>Version</td>
         <td><img src='https://img.shields.io/pypi/v/pybrowsers.svg?logo=pypi&style=for-the-badge' alt="Version"></td>
     </tr>
     <tr>
         <td>Github Actions</td>
         <td><img src='https://img.shields.io/github/actions/workflow/status/roniemartinez/browsers/python.yml?branch=master&label=actions&logo=github%20actions&style=for-the-badge' alt="Github Actions"></td>
         <td>Coverage</td>
-        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/browsers/branch?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
+        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/browsers/master?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
     </tr>
     <tr>
         <td>Supported versions</td>
         <td><img src='https://img.shields.io/pypi/pyversions/pybrowsers.svg?logo=python&style=for-the-badge' alt="Python Versions"></td>
         <td>Wheel</td>
         <td><img src='https://img.shields.io/pypi/wheel/pybrowsers.svg?style=for-the-badge' alt="Wheel"></td>
     </tr>
@@ -59,15 +59,15 @@
 
 ### Import
 
 ```python
 import browsers
 ```
 
-### List all installer browsers
+### List all installed browsers
 
 ```python
 import browsers
 
 print(list(browsers.browsers()))
 # [{'browser_type': 'chrome', 'path': '/Applications/Google Chrome.app/Contents/MacOS/Google Chrome', 'display_name': 'Google Chrome', 'version': '100.0.4896.127'}, {'browser_type': 'firefox', 'path': '/Applications/Firefox.app/Contents/MacOS/firefox', 'display_name': 'Firefox', 'version': '99.0.1'}, {'browser_type': 'safari', 'path': '/Applications/Safari.app/Contents/MacOS/Safari', 'display_name': 'Safari', 'version': '15.4'}, {'browser_type': 'opera', 'path': '/Applications/Opera.app/Contents/MacOS/Opera', 'display_name': 'Opera', 'version': '85.0.4341.60'}, {'browser_type': 'msedge', 'path': '/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge', 'display_name': 'Microsoft Edge', 'version': '100.1185.22042050'}]
 ```
@@ -145,8 +145,8 @@
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 based on https://github.com/httptoolkit/browser-launcher and I thought this
 could be useful to other devs since I cannot find an equivalent library of
 `httptoolkit/browser-launcher` in Python and the known `webbrowser` standard
 library does not support arguments. ## Installation ```bash pip install
 pybrowsers ``` ## Features - Detect browser on OSX - Detect browser on Linux -
 Detect browser on Windows - Launch browser with arguments - Launch and get
 browser by version with wildcard support ## Usage ### Import ```python import
-browsers ``` ### List all installer browsers ```python import browsers print
+browsers ``` ### List all installed browsers ```python import browsers print
 (list(browsers.browsers())) # [{'browser_type': 'chrome', 'path': '/
 Applications/Google Chrome.app/Contents/MacOS/Google Chrome', 'display_name':
 'Google Chrome', 'version': '100.0.4896.127'}, {'browser_type': 'firefox',
 'path': '/Applications/Firefox.app/Contents/MacOS/firefox', 'display_name':
 'Firefox', 'version': '99.0.1'}, {'browser_type': 'safari', 'path': '/
 Applications/Safari.app/Contents/MacOS/Safari', 'display_name': 'Safari',
 'version': '15.4'}, {'browser_type': 'opera', 'path': '/Applications/Opera.app/
```

### Comparing `pybrowsers-0.5.2/browsers/__init__.py` & `pybrowsers-0.6.0/browsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrowsers-0.5.2/browsers/linux.py` & `pybrowsers-0.6.0/browsers/linux.py`

 * *Files identical despite different names*

### Comparing `pybrowsers-0.5.2/browsers/osx.py` & `pybrowsers-0.6.0/browsers/osx.py`

 * *Files identical despite different names*

### Comparing `pybrowsers-0.5.2/browsers/windows.py` & `pybrowsers-0.6.0/browsers/windows.py`

 * *Files identical despite different names*

### Comparing `pybrowsers-0.5.2/pyproject.toml` & `pybrowsers-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "pybrowsers"
-version = "0.5.2"
+version = "0.6.0"
 repository = "https://github.com/roniemartinez/browsers"
 description = "Python library for detecting and launching browsers"
 authors = ["Ronie Martinez <ronmarti18@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Topic :: Internet :: WWW/HTTP :: Browsers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 packages = [
@@ -24,27 +23,27 @@
 ]
 
 [tool.poetry.urls]
 "Donate" = "https://github.com/sponsors/roniemartinez"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
+pywin32 = { version = ">=303,<307", markers = "sys_platform == 'win32'" }
 pyxdg = { version = ">=0.27,<0.29", markers = "sys_platform == 'linux'" }
-pywin32 = { version = ">=303,<306", markers = "sys_platform == 'win32'" }
 
-[tool.poetry.dev-dependencies]
-autoflake = "^1.7.8"
-black = "^22.12"
-isort = "^5.11.2"
-mypy = "^0.991"
-pyproject-flake8 = "^5.0.4"
-pytest = "^7.2.0"
+[tool.poetry.group.dev.dependencies]
+autoflake = "^2.3.0"
+black = "^24.2.0"
+isort = "^5.11.5"
+mypy = "^1.4"
+pyproject-flake8 = ">=6.1,<8.0"
+pytest = "^8.0.2"
 pytest-clarity = "^1.0.1"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.isort]
 line_length = 120
 multi_line_output = 3
 force_grid_wrap = 0
 use_parentheses = true
 include_trailing_comma = true
```

### Comparing `pybrowsers-0.5.2/PKG-INFO` & `pybrowsers-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 Metadata-Version: 2.1
 Name: pybrowsers
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python library for detecting and launching browsers
 Home-page: https://github.com/roniemartinez/browsers
 License: MIT
 Author: Ronie Martinez
 Author-email: ronmarti18@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pywin32 (>=303,<306) ; sys_platform == "win32"
+Requires-Dist: pywin32 (>=303,<307) ; sys_platform == "win32"
 Requires-Dist: pyxdg (>=0.27,<0.29) ; sys_platform == "linux"
 Project-URL: Donate, https://github.com/sponsors/roniemartinez
 Project-URL: Repository, https://github.com/roniemartinez/browsers
 Description-Content-Type: text/markdown
 
 <table>
     <tr>
@@ -37,15 +31,15 @@
         <td>Version</td>
         <td><img src='https://img.shields.io/pypi/v/pybrowsers.svg?logo=pypi&style=for-the-badge' alt="Version"></td>
     </tr>
     <tr>
         <td>Github Actions</td>
         <td><img src='https://img.shields.io/github/actions/workflow/status/roniemartinez/browsers/python.yml?branch=master&label=actions&logo=github%20actions&style=for-the-badge' alt="Github Actions"></td>
         <td>Coverage</td>
-        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/browsers/branch?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
+        <td><img src='https://img.shields.io/codecov/c/github/roniemartinez/browsers/master?label=codecov&logo=codecov&style=for-the-badge' alt="CodeCov"></td>
     </tr>
     <tr>
         <td>Supported versions</td>
         <td><img src='https://img.shields.io/pypi/pyversions/pybrowsers.svg?logo=python&style=for-the-badge' alt="Python Versions"></td>
         <td>Wheel</td>
         <td><img src='https://img.shields.io/pypi/wheel/pybrowsers.svg?style=for-the-badge' alt="Wheel"></td>
     </tr>
@@ -91,15 +85,15 @@
 
 ### Import
 
 ```python
 import browsers
 ```
 
-### List all installer browsers
+### List all installed browsers
 
 ```python
 import browsers
 
 print(list(browsers.browsers()))
 # [{'browser_type': 'chrome', 'path': '/Applications/Google Chrome.app/Contents/MacOS/Google Chrome', 'display_name': 'Google Chrome', 'version': '100.0.4896.127'}, {'browser_type': 'firefox', 'path': '/Applications/Firefox.app/Contents/MacOS/firefox', 'display_name': 'Firefox', 'version': '99.0.1'}, {'browser_type': 'safari', 'path': '/Applications/Safari.app/Contents/MacOS/Safari', 'display_name': 'Safari', 'version': '15.4'}, {'browser_type': 'opera', 'path': '/Applications/Opera.app/Contents/MacOS/Opera', 'display_name': 'Opera', 'version': '85.0.4341.60'}, {'browser_type': 'msedge', 'path': '/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge', 'display_name': 'Microsoft Edge', 'version': '100.1185.22042050'}]
 ```
@@ -178,7 +172,8 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
```

#### html2text {}

```diff
@@ -1,27 +1,23 @@
-Metadata-Version: 2.1 Name: pybrowsers Version: 0.5.2 Summary: Python library
+Metadata-Version: 2.1 Name: pybrowsers Version: 0.6.0 Summary: Python library
 for detecting and launching browsers Home-page: https://github.com/
 roniemartinez/browsers License: MIT Author: Ronie Martinez Author-email:
-ronmarti18@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
-:: 3 - Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: Implementation :: CPython Classifier: Topic
-:: Internet :: WWW/HTTP :: Browsers Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Requires-Dist: pywin32 (>=303,<306) ;
-sys_platform == "win32" Requires-Dist: pyxdg (>=0.27,<0.29) ; sys_platform ==
-"linux" Project-URL: Donate, https://github.com/sponsors/roniemartinez Project-
-URL: Repository, https://github.com/roniemartinez/browsers Description-Content-
-Type: text/markdown
+ronmarti18@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: Development
+Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Dist: pywin32
+(>=303,<307) ; sys_platform == "win32" Requires-Dist: pyxdg (>=0.27,<0.29) ;
+sys_platform == "linux" Project-URL: Donate, https://github.com/sponsors/
+roniemartinez Project-URL: Repository, https://github.com/roniemartinez/
+browsers Description-Content-Type: text/markdown
 License            [License]          Version   [Version]
 Github Actions     [Github Actions]   Coverage  [CodeCov]
 Supported versions [Python Versions]  Wheel     [Wheel]
 Status             [Status]           Downloads [Downloads]
 All Contributors   _[_A_l_l_ _C_o_n_t_r_i_b_u_t_o_r_s_]
 # browsers Python library for detecting and launching browsers ## Why? I
 recently wrote a snippet for detecting installed browsers in an OSX machine in
@@ -29,15 +25,15 @@
 based on https://github.com/httptoolkit/browser-launcher and I thought this
 could be useful to other devs since I cannot find an equivalent library of
 `httptoolkit/browser-launcher` in Python and the known `webbrowser` standard
 library does not support arguments. ## Installation ```bash pip install
 pybrowsers ``` ## Features - Detect browser on OSX - Detect browser on Linux -
 Detect browser on Windows - Launch browser with arguments - Launch and get
 browser by version with wildcard support ## Usage ### Import ```python import
-browsers ``` ### List all installer browsers ```python import browsers print
+browsers ``` ### List all installed browsers ```python import browsers print
 (list(browsers.browsers())) # [{'browser_type': 'chrome', 'path': '/
 Applications/Google Chrome.app/Contents/MacOS/Google Chrome', 'display_name':
 'Google Chrome', 'version': '100.0.4896.127'}, {'browser_type': 'firefox',
 'path': '/Applications/Firefox.app/Contents/MacOS/firefox', 'display_name':
 'Firefox', 'version': '99.0.1'}, {'browser_type': 'safari', 'path': '/
 Applications/Safari.app/Contents/MacOS/Safari', 'display_name': 'Safari',
 'version': '15.4'}, {'browser_type': 'opera', 'path': '/Applications/Opera.app/
```

