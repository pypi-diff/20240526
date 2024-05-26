# Comparing `tmp/pyventim-0.1.1.tar.gz` & `tmp/pyventim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyventim-0.1.1.tar", last modified: Sat May 18 07:35:06 2024, max compression
+gzip compressed data, was "pyventim-0.2.0.tar", last modified: Sun May 26 12:12:30 2024, max compression
```

## Comparing `pyventim-0.1.1.tar` & `pyventim-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:06.108486 pyventim-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 07:35:01.000000 pyventim-0.1.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-18 07:35:06.108486 pyventim-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-18 07:35:01.000000 pyventim-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-18 07:35:01.000000 pyventim-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 07:35:01.000000 pyventim-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-18 07:35:01.000000 pyventim-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 07:35:06.108486 pyventim-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:06.104486 pyventim-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:06.108486 pyventim-0.1.1/src/pyventim/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 07:35:01.000000 pyventim-0.1.1/src/pyventim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-05-18 07:35:01.000000 pyventim-0.1.1/src/pyventim/public.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 07:35:01.000000 pyventim-0.1.1/src/pyventim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:06.108486 pyventim-0.1.1/src/pyventim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-18 07:35:06.000000 pyventim-0.1.1/src/pyventim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-18 07:35:06.000000 pyventim-0.1.1/src/pyventim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:35:06.000000 pyventim-0.1.1/src/pyventim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-18 07:35:06.000000 pyventim-0.1.1/src/pyventim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 07:35:06.000000 pyventim-0.1.1/src/pyventim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:06.108486 pyventim-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-18 07:35:01.000000 pyventim-0.1.1/tests/test_public_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-18 07:35:01.000000 pyventim-0.1.1/tests/test_public_explorer_attraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-18 07:35:01.000000 pyventim-0.1.1/tests/test_public_explorer_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-18 07:35:01.000000 pyventim-0.1.1/tests/test_public_explorer_product_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 07:35:01.000000 pyventim-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:12:30.699021 pyventim-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-26 12:12:26.000000 pyventim-0.2.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-26 12:12:30.699021 pyventim-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-26 12:12:26.000000 pyventim-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-26 12:12:26.000000 pyventim-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-26 12:12:26.000000 pyventim-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 12:12:26.000000 pyventim-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 12:12:30.699021 pyventim-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:12:30.695021 pyventim-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:12:30.699021 pyventim-0.2.0/src/pyventim/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/eventim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-26 12:12:26.000000 pyventim-0.2.0/src/pyventim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:12:30.699021 pyventim-0.2.0/src/pyventim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-26 12:12:30.000000 pyventim-0.2.0/src/pyventim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-26 12:12:30.000000 pyventim-0.2.0/src/pyventim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:12:30.000000 pyventim-0.2.0/src/pyventim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-26 12:12:30.000000 pyventim-0.2.0/src/pyventim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 12:12:30.000000 pyventim-0.2.0/src/pyventim.egg-info/top_level.txt
```

### Comparing `pyventim-0.1.1/LICENCE.md` & `pyventim-0.2.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pyventim-0.1.1/PKG-INFO` & `pyventim-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyventim
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python wrapper to fetch a reverse engineered Eventim API.
 Author-email: Kilian Braun <hello@kilianbraun.de>
 Maintainer-email: Kilian Braun <hello@kilianbraun.de>
 Project-URL: Homepage, https://github.com/kggx/pyventim
 Project-URL: Issues, https://github.com/kggx/pyventim/issues
 Project-URL: Documentation, https://kggx.github.io/pyventim/pyventim.html
 Classifier: Programming Language :: Python :: 3.10
@@ -12,28 +12,34 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: requests>=2.31.0
+Requires-Dist: lxml>=5.2.0
+Requires-Dist: pydantic>=2.7.0
 Provides-Extra: dev
 Requires-Dist: requests>=2.31.0; extra == "dev"
+Requires-Dist: lxml>=5.2.2; extra == "dev"
+Requires-Dist: pydantic>=2.7.0; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: black>=24.4.0; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
 Requires-Dist: twine>=5.1.0; extra == "dev"
 Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
 
 [![Testing](https://github.com/kggx/pyventim/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/testing.yml)
 [![Documentation](https://github.com/kggx/pyventim/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/docs.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
-[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg)](https://pypi.org/project/pyventim/)
+[![Python](https://img.shields.io/pypi/pyversions/pyventim?label=Python)](https://pypi.org/project/pyventim/)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg?label=PyPI)](https://pypi.org/project/pyventim/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyventim.svg?label=PyPI%20downloads)](https://pypi.org/project/pyventim/)
 [![Coverage](https://codecov.io/github/kggx/pyventim/coverage.svg?branch=main)](https://app.codecov.io/github/kggx/pyventim)
 
 ---
 
 > [!NOTE]
 > Consider the whole project as unstable until version 1.0.0 is reached.
@@ -51,35 +57,50 @@
 
 ## Getting Started
 
 ### Dependencies
 
 - Python >= 3.10
 - Requests >= 2.31.0
+- lxml >= 5.2.2
+- Pydantic >= 2.7.0
 
 ### Installing
 
 ```bash
 pip install pyventim
 ```
 
 ### Quick start
 
-#### Public API
+To find attractions we can use the exploration endpoint:
 
 ```python
-# Import the module
-from pyventim.public import EventimExploration
+import pyventim
 
-# Returns attractions found by the explorer api given the search term.
-explorer: EventimExploration = EventimExploration()
-result = explorer.explore_attractions(
-    search_term="Stage Theater im Hafen Hamburg",
-    sort="DateAsc",
-)
+# Create the Eventim class
+eventim = pyventim.Eventim()
+
+# Returns an iterator that fetches all pages off the search endpoint.
+attractions = eventim.explore_attractions(search_term="Landmvrks")
+
+# We can loop over each attraction. The module handles fetching pages automatically.
+for attraction in attractions:
+    print(attraction["attractionId"], attraction["name"])
+```
+
+Next we use the product group endpoint to fetch events for our attraction and get the events of the html endpoint.
+
+```python
+
+# We loop over each product group and fetch the events automatically.
+for product_group in eventim.explore_product_groups(search_term="Landmvrks"):
+    product_group_id = product_group["productGroupId"]
+    for event in eventim.get_product_group_events_from_calendar(product_group_id):
+        print(event["title"], event["eventDate"], event["price"], event["ticketAvailable"], sep=" | ")
 ```
 
 For a more detailed information please refer to the [documentation](https://kggx.github.io/pyventim/pyventim.html).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
```

### Comparing `pyventim-0.1.1/README.md` & `pyventim-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Testing](https://github.com/kggx/pyventim/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/testing.yml)
 [![Documentation](https://github.com/kggx/pyventim/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/docs.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
-[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg)](https://pypi.org/project/pyventim/)
+[![Python](https://img.shields.io/pypi/pyversions/pyventim?label=Python)](https://pypi.org/project/pyventim/)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg?label=PyPI)](https://pypi.org/project/pyventim/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyventim.svg?label=PyPI%20downloads)](https://pypi.org/project/pyventim/)
 [![Coverage](https://codecov.io/github/kggx/pyventim/coverage.svg?branch=main)](https://app.codecov.io/github/kggx/pyventim)
 
 ---
 
 > [!NOTE]
 > Consider the whole project as unstable until version 1.0.0 is reached.
@@ -23,35 +24,50 @@
 
 ## Getting Started
 
 ### Dependencies
 
 - Python >= 3.10
 - Requests >= 2.31.0
+- lxml >= 5.2.2
+- Pydantic >= 2.7.0
 
 ### Installing
 
 ```bash
 pip install pyventim
 ```
 
 ### Quick start
 
-#### Public API
+To find attractions we can use the exploration endpoint:
 
 ```python
-# Import the module
-from pyventim.public import EventimExploration
+import pyventim
 
-# Returns attractions found by the explorer api given the search term.
-explorer: EventimExploration = EventimExploration()
-result = explorer.explore_attractions(
-    search_term="Stage Theater im Hafen Hamburg",
-    sort="DateAsc",
-)
+# Create the Eventim class
+eventim = pyventim.Eventim()
+
+# Returns an iterator that fetches all pages off the search endpoint.
+attractions = eventim.explore_attractions(search_term="Landmvrks")
+
+# We can loop over each attraction. The module handles fetching pages automatically.
+for attraction in attractions:
+    print(attraction["attractionId"], attraction["name"])
+```
+
+Next we use the product group endpoint to fetch events for our attraction and get the events of the html endpoint.
+
+```python
+
+# We loop over each product group and fetch the events automatically.
+for product_group in eventim.explore_product_groups(search_term="Landmvrks"):
+    product_group_id = product_group["productGroupId"]
+    for event in eventim.get_product_group_events_from_calendar(product_group_id):
+        print(event["title"], event["eventDate"], event["price"], event["ticketAvailable"], sep=" | ")
 ```
 
 For a more detailed information please refer to the [documentation](https://kggx.github.io/pyventim/pyventim.html).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
```

#### html2text {}

```diff
@@ -1,34 +1,45 @@
 [![Testing](https://github.com/kggx/pyventim/actions/workflows/testing.yml/
 badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/
 testing.yml) [![Documentation](https://github.com/kggx/pyventim/actions/
 workflows/docs.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/
 actions/workflows/docs.yml) [![Contributor Covenant](https://img.shields.io/
-badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![PyPI
-Latest Release](https://img.shields.io/pypi/v/pyventim.svg)](https://pypi.org/
-project/pyventim/) [![PyPI Downloads](https://img.shields.io/pypi/dm/
-pyventim.svg?label=PyPI%20downloads)](https://pypi.org/project/pyventim/) [!
-[Coverage](https://codecov.io/github/kggx/pyventim/coverage.svg?branch=main)]
-(https://app.codecov.io/github/kggx/pyventim) --- > [!NOTE] > Consider the
-whole project as unstable until version 1.0.0 is reached. # pyventim A Python
-module to fetch usable data with a reverse engineered Eventim API. ##
-Description The [Eventim](https://www.eventim.com/) API has some public
-endpoints but also hidden data in the HTML responses. The project goal is to
-provide away to fetch this data with simple to use python objecs. >
-[!IMPORTANT] > Be aware that the APIs of Eventim can change without notice and
-therefore break the module. ## Getting Started ### Dependencies - Python >=
-3.10 - Requests >= 2.31.0 ### Installing ```bash pip install pyventim ``` ###
-Quick start #### Public API ```python # Import the module from pyventim.public
-import EventimExploration # Returns attractions found by the explorer api given
-the search term. explorer: EventimExploration = EventimExploration() result =
-explorer.explore_attractions( search_term="Stage Theater im Hafen Hamburg",
-sort="DateAsc", ) ``` For a more detailed information please refer to the
-[documentation](https://kggx.github.io/pyventim/pyventim.html). ## License This
-project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md)
-file for details ## Code of conduct Please follow our [code of conduct]
+badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![Python]
+(https://img.shields.io/pypi/pyversions/pyventim?label=Python)](https://
+pypi.org/project/pyventim/) [![PyPI Latest Release](https://img.shields.io/
+pypi/v/pyventim.svg?label=PyPI)](https://pypi.org/project/pyventim/) [![PyPI
+Downloads](https://img.shields.io/pypi/dm/pyventim.svg?label=PyPI%20downloads)]
+(https://pypi.org/project/pyventim/) [![Coverage](https://codecov.io/github/
+kggx/pyventim/coverage.svg?branch=main)](https://app.codecov.io/github/kggx/
+pyventim) --- > [!NOTE] > Consider the whole project as unstable until version
+1.0.0 is reached. # pyventim A Python module to fetch usable data with a
+reverse engineered Eventim API. ## Description The [Eventim](https://
+www.eventim.com/) API has some public endpoints but also hidden data in the
+HTML responses. The project goal is to provide away to fetch this data with
+simple to use python objecs. > [!IMPORTANT] > Be aware that the APIs of Eventim
+can change without notice and therefore break the module. ## Getting Started
+### Dependencies - Python >= 3.10 - Requests >= 2.31.0 - lxml >= 5.2.2 -
+Pydantic >= 2.7.0 ### Installing ```bash pip install pyventim ``` ### Quick
+start To find attractions we can use the exploration endpoint: ```python import
+pyventim # Create the Eventim class eventim = pyventim.Eventim() # Returns an
+iterator that fetches all pages off the search endpoint. attractions =
+eventim.explore_attractions(search_term="Landmvrks") # We can loop over each
+attraction. The module handles fetching pages automatically. for attraction in
+attractions: print(attraction["attractionId"], attraction["name"]) ``` Next we
+use the product group endpoint to fetch events for our attraction and get the
+events of the html endpoint. ```python # We loop over each product group and
+fetch the events automatically. for product_group in
+eventim.explore_product_groups(search_term="Landmvrks"): product_group_id =
+product_group["productGroupId"] for event in
+eventim.get_product_group_events_from_calendar(product_group_id): print(event
+["title"], event["eventDate"], event["price"], event["ticketAvailable"], sep="
+| ") ``` For a more detailed information please refer to the [documentation]
+(https://kggx.github.io/pyventim/pyventim.html). ## License This project is
+licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for
+details ## Code of conduct Please follow our [code of conduct]
 (CODE_OF_CONDUCT.md). ## Finding help The code documentation can be found
 [here](https://kggx.github.io/pyventim/pyventim.html). However if you encounter
 a unexpected behaviour: Feel free to open an [issue](https://github.com/kggx/
 pyventim/issues). ## Contributing All contributions, bug reports, bug fixes,
 documentation improvements, enhancements, and ideas are welcome. If youre
 looking to work on the pyventim codebase: 1. Fork the repository. 1. Make your
 changes and follow common code practices as well as Python PEP standards. 1.
```

### Comparing `pyventim-0.1.1/pyproject.toml` & `pyventim-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyventim"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Kilian Braun", email="hello@kilianbraun.de" },
 ]
 maintainers = [
   { name="Kilian Braun", email="hello@kilianbraun.de" },
 ]
```

### Comparing `pyventim-0.1.1/src/pyventim.egg-info/PKG-INFO` & `pyventim-0.2.0/src/pyventim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyventim
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python wrapper to fetch a reverse engineered Eventim API.
 Author-email: Kilian Braun <hello@kilianbraun.de>
 Maintainer-email: Kilian Braun <hello@kilianbraun.de>
 Project-URL: Homepage, https://github.com/kggx/pyventim
 Project-URL: Issues, https://github.com/kggx/pyventim/issues
 Project-URL: Documentation, https://kggx.github.io/pyventim/pyventim.html
 Classifier: Programming Language :: Python :: 3.10
@@ -12,28 +12,34 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 Requires-Dist: requests>=2.31.0
+Requires-Dist: lxml>=5.2.0
+Requires-Dist: pydantic>=2.7.0
 Provides-Extra: dev
 Requires-Dist: requests>=2.31.0; extra == "dev"
+Requires-Dist: lxml>=5.2.2; extra == "dev"
+Requires-Dist: pydantic>=2.7.0; extra == "dev"
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: black>=24.4.0; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
 Requires-Dist: twine>=5.1.0; extra == "dev"
 Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: Pillow; extra == "dev"
 
 [![Testing](https://github.com/kggx/pyventim/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/testing.yml)
 [![Documentation](https://github.com/kggx/pyventim/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/kggx/pyventim/actions/workflows/docs.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
-[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg)](https://pypi.org/project/pyventim/)
+[![Python](https://img.shields.io/pypi/pyversions/pyventim?label=Python)](https://pypi.org/project/pyventim/)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pyventim.svg?label=PyPI)](https://pypi.org/project/pyventim/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyventim.svg?label=PyPI%20downloads)](https://pypi.org/project/pyventim/)
 [![Coverage](https://codecov.io/github/kggx/pyventim/coverage.svg?branch=main)](https://app.codecov.io/github/kggx/pyventim)
 
 ---
 
 > [!NOTE]
 > Consider the whole project as unstable until version 1.0.0 is reached.
@@ -51,35 +57,50 @@
 
 ## Getting Started
 
 ### Dependencies
 
 - Python >= 3.10
 - Requests >= 2.31.0
+- lxml >= 5.2.2
+- Pydantic >= 2.7.0
 
 ### Installing
 
 ```bash
 pip install pyventim
 ```
 
 ### Quick start
 
-#### Public API
+To find attractions we can use the exploration endpoint:
 
 ```python
-# Import the module
-from pyventim.public import EventimExploration
+import pyventim
 
-# Returns attractions found by the explorer api given the search term.
-explorer: EventimExploration = EventimExploration()
-result = explorer.explore_attractions(
-    search_term="Stage Theater im Hafen Hamburg",
-    sort="DateAsc",
-)
+# Create the Eventim class
+eventim = pyventim.Eventim()
+
+# Returns an iterator that fetches all pages off the search endpoint.
+attractions = eventim.explore_attractions(search_term="Landmvrks")
+
+# We can loop over each attraction. The module handles fetching pages automatically.
+for attraction in attractions:
+    print(attraction["attractionId"], attraction["name"])
+```
+
+Next we use the product group endpoint to fetch events for our attraction and get the events of the html endpoint.
+
+```python
+
+# We loop over each product group and fetch the events automatically.
+for product_group in eventim.explore_product_groups(search_term="Landmvrks"):
+    product_group_id = product_group["productGroupId"]
+    for event in eventim.get_product_group_events_from_calendar(product_group_id):
+        print(event["title"], event["eventDate"], event["price"], event["ticketAvailable"], sep=" | ")
 ```
 
 For a more detailed information please refer to the [documentation](https://kggx.github.io/pyventim/pyventim.html).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
```

