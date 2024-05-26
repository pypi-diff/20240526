# Comparing `tmp/altvmasterlist-3.1.0.tar.gz` & `tmp/altvmasterlist-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-3.1.0.tar", max compression
+gzip compressed data, was "altvmasterlist-3.2.0.tar", max compression
```

## Comparing `altvmasterlist-3.1.0.tar` & `altvmasterlist-3.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16725 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/LICENSE
--rw-r--r--   0        0        0     2186 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/README.md
--rw-r--r--   0        0        0     1534 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      385 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     3479 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/src/altvmasterlist/enum.py
--rw-r--r--   0        0        0    15799 2024-04-12 08:55:46.217277 altvmasterlist-3.1.0/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 altvmasterlist-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/LICENSE
+-rw-r--r--   0        0        0     2185 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/README.md
+-rw-r--r--   0        0        0     1534 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     3479 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/src/altvmasterlist/enum.py
+-rw-r--r--   0        0        0    15799 2024-05-26 11:30:16.701262 altvmasterlist-3.2.0/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 altvmasterlist-3.2.0/PKG-INFO
```

### Comparing `altvmasterlist-3.1.0/LICENSE` & `altvmasterlist-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-3.1.0/README.md` & `altvmasterlist-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   [![PyPI - Format](https://img.shields.io/pypi/format/altvmasterlist)](https://pypi.org/project/altvmasterlist/)
   [![PyPI - Downloads](https://img.shields.io/pypi/dm/altvmasterlist)](https://pypi.org/project/altvmasterlist/)
 
 </div>
 
 ---
 
-<p align="center"> This is a python3 package to interface with the <a href="https://altv.mp">alt:V</a>> Masterlist API.
+<p align="center"> This is a python3 package to interface with the <a href="https://altv.mp">alt:V</a> Masterlist API.
     <br> 
 </p>
 
 ## 📝 Table of Contents
 - [About](#about)
 - [Getting Started](#getting_started)
 - [Deployment](#deployment)
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
    [License](https://img.shields.io/github/license/nickwasused/altv-python-
    masterlist)](/LICENSE) [![PyPI - Version](https://img.shields.io/pypi/v/
  altvmasterlist)](https://pypi.org/project/altvmasterlist/) [![PyPI - Format]
 (https://img.shields.io/pypi/format/altvmasterlist)](https://pypi.org/project/
      altvmasterlist/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
           altvmasterlist)](https://pypi.org/project/altvmasterlist/)
 ---
-    This is a python3 package to interface with the _a_l_t_:_V> Masterlist API.
+     This is a python3 package to interface with the _a_l_t_:_V Masterlist API.
 ## ð Table of Contents - [About](#about) - [Getting Started]
 (#getting_started) - [Deployment](#deployment) - [Usage](#usage) - [Built
 Using](#built_using) - [Affiliation](#affiliation) ## ð§ About This is a
 python3 package to interface with the _a_l_t_:_V> Masterlist API. ## ð Getting
 Started These instructions will get you a copy of the project up and running on
 your local machine for development and testing purposes. See [deployment]
 (#deployment) for notes on how to deploy the project on a live system. ###
```

### Comparing `altvmasterlist-3.1.0/pyproject.toml` & `altvmasterlist-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "3.1.0"
+version = "3.2.0"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
```

### Comparing `altvmasterlist-3.1.0/src/altvmasterlist/enum.py` & `altvmasterlist-3.2.0/src/altvmasterlist/enum.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-3.1.0/src/altvmasterlist/masterlist.py` & `altvmasterlist-3.2.0/src/altvmasterlist/masterlist.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-3.1.0/PKG-INFO` & `altvmasterlist-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altvmasterlist
-Version: 3.1.0
+Version: 3.2.0
 Summary: A package to use the alt:V Masterlist api.
 Home-page: https://github.com/Nickwasused/altv-python-masterlist
 License: MPL-2.0
 Author: Nickwasused
 Author-email: contact.nickwasused.fa6c8@simplelogin.co
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
@@ -31,15 +31,15 @@
   [![PyPI - Format](https://img.shields.io/pypi/format/altvmasterlist)](https://pypi.org/project/altvmasterlist/)
   [![PyPI - Downloads](https://img.shields.io/pypi/dm/altvmasterlist)](https://pypi.org/project/altvmasterlist/)
 
 </div>
 
 ---
 
-<p align="center"> This is a python3 package to interface with the <a href="https://altv.mp">alt:V</a>> Masterlist API.
+<p align="center"> This is a python3 package to interface with the <a href="https://altv.mp">alt:V</a> Masterlist API.
     <br> 
 </p>
 
 ## 📝 Table of Contents
 - [About](#about)
 - [Getting Started](#getting_started)
 - [Deployment](#deployment)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: altvmasterlist Version: 3.1.0 Summary: A package to
+Metadata-Version: 2.1 Name: altvmasterlist Version: 3.2.0 Summary: A package to
 use the alt:V Masterlist api. Home-page: https://github.com/Nickwasused/altv-
 python-masterlist License: MPL-2.0 Author: Nickwasused Author-email:
 contact.nickwasused.fa6c8@simplelogin.co Requires-Python: >=3.10 Classifier:
 License :: OSI Approved Classifier: License :: OSI Approved :: Mozilla Public
 License 2.0 (MPL 2.0) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -17,15 +17,15 @@
    [License](https://img.shields.io/github/license/nickwasused/altv-python-
    masterlist)](/LICENSE) [![PyPI - Version](https://img.shields.io/pypi/v/
  altvmasterlist)](https://pypi.org/project/altvmasterlist/) [![PyPI - Format]
 (https://img.shields.io/pypi/format/altvmasterlist)](https://pypi.org/project/
      altvmasterlist/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
           altvmasterlist)](https://pypi.org/project/altvmasterlist/)
 ---
-    This is a python3 package to interface with the _a_l_t_:_V> Masterlist API.
+     This is a python3 package to interface with the _a_l_t_:_V Masterlist API.
 ## ð Table of Contents - [About](#about) - [Getting Started]
 (#getting_started) - [Deployment](#deployment) - [Usage](#usage) - [Built
 Using](#built_using) - [Affiliation](#affiliation) ## ð§ About This is a
 python3 package to interface with the _a_l_t_:_V> Masterlist API. ## ð Getting
 Started These instructions will get you a copy of the project up and running on
 your local machine for development and testing purposes. See [deployment]
 (#deployment) for notes on how to deploy the project on a live system. ###
```

