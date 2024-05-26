# Comparing `tmp/continuo-0.2.2.tar.gz` & `tmp/continuo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuo-0.2.2.tar", last modified: Thu Aug 18 13:53:51 2022, max compression
+gzip compressed data, was "continuo-0.3.0.tar", last modified: Sun May 26 11:36:01 2024, max compression
```

## Comparing `continuo-0.2.2.tar` & `continuo-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 13:53:51.929006 continuo-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-08-18 13:53:41.000000 continuo-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-18 13:53:41.000000 continuo-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7017 2022-08-18 13:53:51.929006 continuo-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-08-18 13:53:41.000000 continuo-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 13:53:51.925005 continuo-0.2.2/continuo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/duration.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/effects.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/music_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/output.py
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/playback.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-08-18 13:53:41.000000 continuo-0.2.2/continuo/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 13:53:51.929006 continuo-0.2.2/continuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7017 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-18 13:53:51.000000 continuo-0.2.2/continuo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-18 13:53:41.000000 continuo-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-18 13:53:51.929006 continuo-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-08-18 13:53:41.000000 continuo-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:36:01.021618 continuo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-26 11:35:56.000000 continuo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-26 11:35:56.000000 continuo-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-26 11:36:01.021618 continuo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-26 11:35:56.000000 continuo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:36:01.017618 continuo-0.3.0/continuo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/music_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/playback.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 11:35:56.000000 continuo-0.3.0/continuo/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:36:01.021618 continuo-0.3.0/continuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-26 11:36:01.000000 continuo-0.3.0/continuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-26 11:36:01.000000 continuo-0.3.0/continuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:36:01.000000 continuo-0.3.0/continuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:36:00.000000 continuo-0.3.0/continuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 11:36:01.000000 continuo-0.3.0/continuo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 11:36:01.000000 continuo-0.3.0/continuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 11:35:57.000000 continuo-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:36:01.021618 continuo-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-26 11:35:57.000000 continuo-0.3.0/setup.py
```

### Comparing `continuo-0.2.2/LICENSE` & `continuo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/PKG-INFO` & `continuo-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: continuo
-Version: 0.2.2
-Summary: Procedural music generator
-Home-page: https://github.com/rbaltrusch/continuo
-Author: Richard Baltrusch
-License: AGPLv3
-Keywords: python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Pylint](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml)
 [![Unit tests](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 # Music Generation
 
 This tool procedurally generates music based on codified Western classical music principles.
@@ -35,14 +13,20 @@
     python -m pip install continuo
     python -m continuo
 
 ## Example music
 
 Example music can be found [here](https://github.com/rbaltrusch/continuo/blob/master/example_music).
 
+## ⚠️ State of the repository ⚠️
+
+This repository is unlikely to receive new features in the future, although maintenance and small fixes will still be done.
+
+This means that some features that are missing now will stay missing (but feel free to submit a pull request to add them!), and non-optimal aspects of the codebase or the application are unlikely to get fixed.
+
 ## Parameterization
 
 Custom parameterization is possible over the command line interface or an external configuration file, but currently not consolidated into one config file.
 
 ### Command line interface
 
 The application supports configuration of almost every configurable setting directly over the command line interface.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `continuo-0.2.2/README.md` & `continuo-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: continuo
+Version: 0.3.0
+Summary: Procedural music generator
+Home-page: https://github.com/rbaltrusch/continuo
+Author: Richard Baltrusch
+License: AGPLv3
+Keywords: python
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Desktop Environment
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: musical==0.3.0
+Requires-Dist: numpy==1.24.0
+Requires-Dist: pygame==2.5.2
+
 [![Pylint](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml)
 [![Unit tests](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 # Music Generation
 
 This tool procedurally generates music based on codified Western classical music principles.
@@ -13,14 +46,20 @@
     python -m pip install continuo
     python -m continuo
 
 ## Example music
 
 Example music can be found [here](https://github.com/rbaltrusch/continuo/blob/master/example_music).
 
+## ⚠️ State of the repository ⚠️
+
+This repository is unlikely to receive new features in the future, although maintenance and small fixes will still be done.
+
+This means that some features that are missing now will stay missing (but feel free to submit a pull request to add them!), and non-optimal aspects of the codebase or the application are unlikely to get fixed.
+
 ## Parameterization
 
 Custom parameterization is possible over the command line interface or an external configuration file, but currently not consolidated into one config file.
 
 ### Command line interface
 
 The application supports configuration of almost every configurable setting directly over the command line interface.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `continuo-0.2.2/continuo/__main__.py` & `continuo-0.3.0/continuo/__main__.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/cli.py` & `continuo-0.3.0/continuo/cli.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/config.py` & `continuo-0.3.0/continuo/config.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/generator.py` & `continuo-0.3.0/continuo/generator.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/layer.py` & `continuo-0.3.0/continuo/layer.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/music_algorithm.py` & `continuo-0.3.0/continuo/music_algorithm.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/output.py` & `continuo-0.3.0/continuo/output.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/playback.py` & `continuo-0.3.0/continuo/playback.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/scale.py` & `continuo-0.3.0/continuo/scale.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo/timeline.py` & `continuo-0.3.0/continuo/timeline.py`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/continuo.egg-info/PKG-INFO` & `continuo-0.3.0/continuo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
 Name: continuo
-Version: 0.2.2
+Version: 0.3.0
 Summary: Procedural music generator
 Home-page: https://github.com/rbaltrusch/continuo
 Author: Richard Baltrusch
 License: AGPLv3
 Keywords: python
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Desktop Environment
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: musical==0.3.0
+Requires-Dist: numpy==1.24.0
+Requires-Dist: pygame==2.5.2
 
 [![Pylint](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pylint.yml)
 [![Unit tests](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/rbaltrusch/continuo/actions/workflows/pytest-unit-tests.yml)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
 # Music Generation
 
@@ -35,14 +46,20 @@
     python -m pip install continuo
     python -m continuo
 
 ## Example music
 
 Example music can be found [here](https://github.com/rbaltrusch/continuo/blob/master/example_music).
 
+## ⚠️ State of the repository ⚠️
+
+This repository is unlikely to receive new features in the future, although maintenance and small fixes will still be done.
+
+This means that some features that are missing now will stay missing (but feel free to submit a pull request to add them!), and non-optimal aspects of the codebase or the application are unlikely to get fixed.
+
 ## Parameterization
 
 Custom parameterization is possible over the command line interface or an external configuration file, but currently not consolidated into one config file.
 
 ### Command line interface
 
 The application supports configuration of almost every configurable setting directly over the command line interface.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `continuo-0.2.2/continuo.egg-info/SOURCES.txt` & `continuo-0.3.0/continuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `continuo-0.2.2/setup.py` & `continuo-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 project_dir = Path(__file__).parent
 
 setuptools.setup(
     name="continuo",
-    version="0.2.2",
+    version="0.3.0",
     description="Procedural music generator",
     long_description=project_dir.joinpath("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     keywords=["python"],
     author="Richard Baltrusch",
     url="https://github.com/rbaltrusch/continuo",
     packages=setuptools.find_packages("."),
@@ -25,18 +25,26 @@
     install_requires=project_dir.joinpath("requirements.txt")
     .read_text(encoding="utf-8")
     .split("\n"),
     zip_safe=False,
     license="AGPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
+        "Environment :: Console",
         "Intended Audience :: Developers",
+        "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Artistic Software",
+        "Topic :: Desktop Environment",
+        "Topic :: Multimedia",
+        "Topic :: Multimedia :: Sound/Audio",
+        "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
         "Typing :: Typed",
     ],
 )
```

