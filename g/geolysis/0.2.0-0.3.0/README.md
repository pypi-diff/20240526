# Comparing `tmp/geolysis-0.2.0.tar.gz` & `tmp/geolysis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolysis-0.2.0.tar", last modified: Tue Feb  6 22:58:27 2024, max compression
+gzip compressed data, was "geolysis-0.3.0.tar", last modified: Sat May 25 22:36:25 2024, max compression
```

## Comparing `geolysis-0.2.0.tar` & `geolysis-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 22:58:27.367234 geolysis-0.2.0/
--rw-rw-rw-   0        0        0     1086 2023-10-15 09:38:28.000000 geolysis-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     8123 2024-02-06 22:58:27.366227 geolysis-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5195 2024-02-06 22:03:07.000000 geolysis-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 22:58:27.070644 geolysis-0.2.0/geolysis/
--rw-rw-rw-   0        0        0      162 2024-02-06 22:57:05.000000 geolysis-0.2.0/geolysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:58:27.239231 geolysis-0.2.0/geolysis/bearing_capacity/
--rw-rw-rw-   0        0        0       19 2024-01-24 22:12:34.000000 geolysis-0.2.0/geolysis/bearing_capacity/__init__.py
--rw-rw-rw-   0        0        0     9960 2024-02-06 18:20:58.000000 geolysis-0.2.0/geolysis/bearing_capacity/abc.py
--rw-rw-rw-   0        0        0      444 2024-02-05 23:33:52.000000 geolysis-0.2.0/geolysis/constants.py
--rw-rw-rw-   0        0        0     7459 2024-02-06 00:12:57.000000 geolysis-0.2.0/geolysis/estimators.py
--rw-rw-rw-   0        0        0     4192 2024-02-06 18:17:23.000000 geolysis-0.2.0/geolysis/foundation.py
--rw-rw-rw-   0        0        0    22543 2024-02-06 16:21:05.000000 geolysis-0.2.0/geolysis/soil_classifier.py
--rw-rw-rw-   0        0        0    18129 2024-02-06 18:17:14.000000 geolysis-0.2.0/geolysis/spt.py
--rw-rw-rw-   0        0        0     2422 2024-02-06 18:27:00.000000 geolysis-0.2.0/geolysis/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:58:27.260200 geolysis-0.2.0/geolysis.egg-info/
--rw-rw-rw-   0        0        0     8123 2024-02-06 22:58:26.000000 geolysis-0.2.0/geolysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-02-06 22:58:26.000000 geolysis-0.2.0/geolysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 22:58:26.000000 geolysis-0.2.0/geolysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-02-06 22:58:26.000000 geolysis-0.2.0/geolysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-06 22:58:26.000000 geolysis-0.2.0/geolysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2750 2024-01-28 09:57:17.000000 geolysis-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      138 2024-02-06 22:58:27.488494 geolysis-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-12-08 13:51:01.000000 geolysis-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:58:27.256510 geolysis-0.2.0/tests/
--rw-rw-rw-   0        0        0     3006 2024-02-06 17:26:09.000000 geolysis-0.2.0/tests/test_bearing_capacity.py
--rw-rw-rw-   0        0        0     2338 2024-01-11 14:24:15.000000 geolysis-0.2.0/tests/test_estimators.py
--rw-rw-rw-   0        0        0     6058 2024-02-06 17:28:52.000000 geolysis-0.2.0/tests/test_soil_classifier.py
--rw-rw-rw-   0        0        0     4157 2024-02-06 18:09:18.000000 geolysis-0.2.0/tests/test_spt.py
--rw-rw-rw-   0        0        0      922 2024-01-11 14:11:48.000000 geolysis-0.2.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:36:25.512782 geolysis-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-09 20:50:13.000000 geolysis-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9007 2024-05-25 22:36:25.502854 geolysis-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7342 2024-05-25 22:22:58.000000 geolysis-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 22:36:25.377150 geolysis-0.3.0/geolysis/
+-rw-rw-rw-   0        0        0       45 2024-05-13 08:55:06.000000 geolysis-0.3.0/geolysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:36:25.462126 geolysis-0.3.0/geolysis/core/
+-rw-rw-rw-   0        0        0      149 2024-05-13 10:53:35.000000 geolysis-0.3.0/geolysis/core/__init__.py
+-rw-rw-rw-   0        0        0    15401 2024-05-25 22:07:56.000000 geolysis-0.3.0/geolysis/core/abc_4_cohl_soils.py
+-rw-rw-rw-   0        0        0      991 2024-05-25 22:23:57.000000 geolysis-0.3.0/geolysis/core/constants.py
+-rw-rw-rw-   0        0        0    13324 2024-05-25 22:24:45.000000 geolysis-0.3.0/geolysis/core/estimators.py
+-rw-rw-rw-   0        0        0    13692 2024-05-18 20:26:33.000000 geolysis-0.3.0/geolysis/core/foundation.py
+-rw-rw-rw-   0        0        0    28201 2024-05-25 22:25:38.000000 geolysis-0.3.0/geolysis/core/soil_classifier.py
+-rw-rw-rw-   0        0        0    17109 2024-05-25 22:26:26.000000 geolysis-0.3.0/geolysis/core/spt.py
+-rw-rw-rw-   0        0        0     3070 2024-05-25 22:28:40.000000 geolysis-0.3.0/geolysis/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:36:25.501906 geolysis-0.3.0/geolysis.egg-info/
+-rw-rw-rw-   0        0        0     9007 2024-05-25 22:36:25.000000 geolysis-0.3.0/geolysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2024-05-25 22:36:25.000000 geolysis-0.3.0/geolysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:36:25.000000 geolysis-0.3.0/geolysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-25 22:36:25.000000 geolysis-0.3.0/geolysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 22:36:25.000000 geolysis-0.3.0/geolysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2698 2024-05-25 22:33:52.000000 geolysis-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:36:25.512782 geolysis-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-12-08 13:51:01.000000 geolysis-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:36:25.490011 geolysis-0.3.0/tests/
+-rw-rw-rw-   0        0        0       17 2024-05-18 17:25:19.000000 geolysis-0.3.0/tests/test_abc_4_cohl_soils.py
+-rw-rw-rw-   0        0        0      600 2024-05-18 20:26:58.000000 geolysis-0.3.0/tests/test_estimators.py
+-rw-rw-rw-   0        0        0     2381 2024-05-18 20:25:16.000000 geolysis-0.3.0/tests/test_foundation.py
+-rw-rw-rw-   0        0        0     6098 2024-05-18 20:25:16.000000 geolysis-0.3.0/tests/test_soil_classifier.py
+-rw-rw-rw-   0        0        0     1527 2024-05-18 20:25:16.000000 geolysis-0.3.0/tests/test_spt.py
+-rw-rw-rw-   0        0        0      814 2024-05-13 09:02:05.000000 geolysis-0.3.0/tests/test_utils.py
```

### Comparing `geolysis-0.2.0/LICENSE.txt` & `geolysis-0.3.0/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 geolysis
+Copyright (c) 2024 geolysis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `geolysis-0.2.0/PKG-INFO` & `geolysis-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,193 +1,189 @@
-Metadata-Version: 2.1
-Name: geolysis
-Version: 0.2.0
-Summary: geolysis is an opensource software for geotechnical engineering analysis and modeling.
-Author-email: Patrick Boateng <boatengpato.pb@gmail.com>
-Maintainer-email: Patrick Boateng <boatengpato.pb@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 geolysis
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/patrickboateng/geolysis
-Project-URL: Repository, https://github.com/patrickboateng/geolysis
-Project-URL: Changelog, https://github.com/patrickboateng/geolysis/blob/main/CHANGELOG.md
-Project-URL: Issue Tracker, https://github.com/patrickboateng/geolysis/issues
-Project-URL: Discussions, https://github.com/patrickboateng/geolysis/discussions
-Keywords: discrete-element-method,geotechnical-engineering,soil-classification,settlement-analysis,bearing-capacity-analysis
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-
 [code_of_conduct_url]: https://github.com/patrickboateng/geolysis/blob/main/CODE_OF_CONDUCT.md/
 [contributing_url]: https://github.com/patrickboateng/geolysis/blob/main/docs/CONTRIBUTING.md#how-to-contribute
-[changelog_url]: https://github.com/patrickboateng/geolysis/blob/main/CHANGELOG.md
 [license_url]: https://github.com/patrickboateng/geolysis/blob/main/LICENSE.txt
 
-<h1 align="center">
-<img src="https://raw.githubusercontent.com/patrickboateng/geolysis/main/docs/source/_static/geolysis_logo.png" alt="logo" width="300">
-</h1><br>
+# geolysis
 
 <div align="center">
 
-[![GitHub Repo stars](https://img.shields.io/github/stars/patrickboateng/geolysis?style=flat&logo=github)](https://github.com/patrickboateng/geolysis/stargazers)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/geolysis?style=flat&logo=pypi)](https://pypi.org/project/geolysis/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/geolysis.svg?logo=python&style=flat)](https://pypi.python.org/pypi/geolysis/)
-[![GitHub last commit](https://img.shields.io/github/last-commit/patrickboateng/geolysis?logo=github&style=flat)](https://github.com/patrickboateng/geolysis/commits)
 [![license](https://img.shields.io/pypi/l/geolysis?style=flat&logo=opensourceinitiative)](https://opensource.org/license/mit/)
 
-#
-
 ![Coveralls Status](https://img.shields.io/coverallsCoverage/github/patrickboateng/geolysis?logo=coveralls)
-[![CI-Unit-Test](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml)
-[![CI-Build-Test](https://github.com/patrickboateng/geolysis/actions/workflows/build.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/build.yml)
+[![Unit-Tests](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml)
+[![Pkg Build](https://github.com/patrickboateng/geolysis/actions/workflows/pkg_build.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/pkg_build.yml)
+[![Documentation Status](https://readthedocs.org/projects/geolysis/badge/?version=latest)](https://geolysis.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-## Project Links
+#
+
+`geolysis` is your one-stop shop for all your geotechnical engineering
+solutions, ranging from site investigation and laboratory test analysis
+to advanced geotechnical designs.
+
+`geolysis` is divided into four (4) main parts:
+
+1. `geolyis.core (Python Package)`
+
+   `geolysis.core` is an open-source Python package that provides features
+   for analyzing geotechnical results obtained from field and laboratory
+   tests. `geolysis.core` is designed specifically to assist developers
+   in building applications that can solve complex geotechnical
+   problems.
+
+   Whether you're working on soil mechanics, rock mechanics, or any other
+   geotechnical field, `geolysis.core` provides a powerful set of tools
+   that can help you design and develop robust solutions. With an
+   intuitive API and a wide range of features, this software is an
+   essential tool for anyone who needs to work with geotechnical data on
+   a regular basis. Whether you're a seasoned geotechnical engineer or a
+   new developer just getting started in the field, `geolysis.core` is
+   the ideal solution for all your software development needs.
+
+   Some of the features implemented so far include soil classification,
+   standard penetration test analysis (such as SPT N-design and SPT
+   N-value corrections), and calculating the allowable bearing capacity of
+   soils from Standard Penetration Test N-values. There are more features
+   underway, which include settlement analysis, ultimate bearing capacity
+   analysis, etc.
+
+   `geolysis.core` is the foundation application on which other parts of the
+   application will depend. Developers can also use `geolysis.core` to power
+   their applications.
+
+1. `geolysis.ui (Qt, PySide6)`
+
+   `geolysis.ui` is a Graphical User Interface (GUI) which will enable
+   users to graphically interact with `geolysis`. User will be able to
+   input data and view generated plots, such as `PSD` curves,
+   `Atterberg Limits` plots, `Compaction` curves, etc within the application.
+
+1. `geolysis.excel (Javascript & Others)`
+
+   `geolysis.excel` provides a Microsoft Excel add-in for simple geotechnical
+   analysis. _More on this later._
+
+1. `geolysis.ai (Python, Pytorch & Others)`
 
-<!-- - [Documentation](/docs) -->
+   `geolysis.ai` explores the use of Artificial Intelligence (**AI**) in
+   enhancing productivity in Geotechnical Engineering.
 
-- [Homepage](https://github.com/patrickboateng/geolysis)
+## Project Links
+
+- [Documentation](https://geolysis.readthedocs.org/en/latest)
+- [Repo](https://github.com/patrickboateng/geolysis)
 - [PyPi](https://pypi.org/project/geolysis/)
 - [Bug Reports](https://github.com/patrickboateng/geolysis/issues)
 - [Discussions](https://github.com/patrickboateng/geolysis/discussions)
 
-> [!IMPORTANT]
-> Project documentation is underway
+<!-- > [!IMPORTANT]
+> Project documentation is underway -->
 
 ## Table of Contents
 
-- [What is geolysis?](#what-is-geolysis)
+- [Motivation](#motivation)
 - [Installation](#installation)
-- [Soil Classification Example](#soil-classification-example)
-  - [AASHTO Classification](#aashto-classification)
-  - [USCS Classification](#uscs-classification)
+- [Getting Started](#getting-started)
+  - [Soil Classification Example](#soil-classification-example)
 - [Release History](#release-history)
 - [Code of Conduct](#code-of-conduct)
 - [Contributing](#contributing)
 - [License](#license)
+- [Governance of this project](#governance-of-this-project)
 - [Contact Information](#contact-information)
 
-## What is geolysis?
+## Motivation
 
-`geolysis` is an open-source software for geotechnical analysis and modeling.
-It provides features such as `soil classifications`
-(based on the USCS and AASHTO classification standards), `estimating soil
-bearing capacity` using SPT N-value, and `estimating of soil engineering parameters`
-such as `Soil Unit Weight` (moist, saturated, and submerged), `Compression index`,
-`soil internal angle of friction`, and `undrained shear strength of soil`.
-
-**Features to include in upcoming versions:**
-
-- Settlement analysis
-- Discrete element method (DEM)
-
-The motivation behind `geolysis` is to provide free software to assist
-geotechnical engineers in their day-to-day work and to expose civil
-engineering students (especially geotechnical students) to tools that
-can make them industry-ready geotechnical engineers right from college.
+`geolysis` is a software solution that aims to support geotechnical
+engineers in their daily work by providing a set of tools that makes
+them perform their tasks in a more efficient and effective manner.
+Moreover, the platform is designed to educate civil engineering
+students, especially those who specialize in geotechnical engineering,
+by exposing them to industry-relevant tools and techniques that will
+help them become industry-ready professionals as soon as they graduate.
+With `geolysis`, users will be better equipped to handle geotechnical
+challenges, make informed decisions, and improve their overall
+productivity.
 
 ## Installation
 
 ```shell
 pip install geolysis
 ```
 
-## Soil Classification Example
+## Getting Started
+
+### Soil Classification Example
 
-### AASHTO Classification
+AASHTO classification
 
 ```python
 
->>> from geolysis.soil_classifier import AASHTO
+>>> from geolysis.core.soil_classifier import AASHTO
 >>> aashto_cls = AASHTO(liquid_limit=30.2, plasticity_index=6.3, fines=11.18)
 >>> aashto_cls.soil_class
 'A-2-4(0)'
 >>> aashto_cls.soil_desc
 'Silty or clayey gravel and sand'
 
 ```
 
-### USCS Classification
+USCS Classification
 
 ```python
 
->>> from geolysis.soil_classifier import USCS
->>> uscs_cls = USCS(liquid_limit=34.1, plastic_limit=21.1, fines=47.88,
-...                 sand=37.84, gravel=14.8)
+>>> from geolysis.core.soil_classifier import USCS
+>>> uscs_cls = USCS(liquid_limit=34.1, plastic_limit=21.1,
+...                 fines=47.88, sand=37.84, gravel=14.8)
 >>> uscs_cls.soil_class
 'SC'
 >>> uscs_cls.soil_desc
 'Clayey sands'
 >>> uscs_cls = USCS(liquid_limit=30.8, plastic_limit=20.7, fines=10.29,
 ...                 sand=81.89, gravel=7.83, d_10=0.07, d_30=0.3, d_60=0.8)
 >>> uscs_cls.soil_class
 'SW-SC'
 >>> uscs_cls.soil_desc
 'Well graded sand with clay'
 
 ```
 
+<!-- See the [Quick start section] of the docs for more examples. -->
+
 ## Release History
 
-Check the [changelog][changelog_url] for release history.
+Check out the [release notes](https://geolysis.rtfd.io/en/latest/release_notes/index.html)
+for features.
 
 ## Code of Conduct
 
-This project has a [code of conduct][code_of_conduct_url] that we
-expect all contributors to adhere to. Please read and follow it
-when participating in this project.
+This project has a [code of conduct][code_of_conduct_url] that
+we expect all contributors to adhere to. Please read and follow
+it when participating in this project.
 
 ## Contributing
 
-If you would like to contribute to this project, please read the
-[contributing guidelines][contributing_url]
+If you would like to contribute to this project, please read
+the [contributing guidelines][contributing_url]
 
 ## License
 
 Distributed under the [**MIT**][license_url] license. By using,
 distributing, or contributing to this project, you agree to the
 terms and conditions of this license.
 
+## Governance of this project
+
+`geolysis.core` is still developing relatively rapidly, so please
+be patient if things change or features iterate and change quickly.
+Once `geolysis.core` hits `1.0.0`, it will slow down considerably.
+
 ## Contact Information
 
 - [**LinkedIn**](https://linkedin.com/in/patrickboateng/)
 
 > [!IMPORTANT]
 > For questions or comments about `geolysis`, please ask them in the
 > [discussions forum](https://github.com/patrickboateng/geolysis/discussions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geolysis-0.2.0/geolysis/soil_classifier.py` & `geolysis-0.3.0/geolysis/core/soil_classifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,241 +1,99 @@
-from types import MappingProxyType
-from typing import NamedTuple
+from abc import abstractmethod
+from typing import NamedTuple, Protocol
 
 from .constants import ERROR_TOL
-from .utils import ceil, isclose, round_
+from .utils import isclose, round_
 
-__all__ = [
-    "AASHTO_SOIL_DESC",
-    "USCS_SOIL_DESC",
-    "AtterbergLimits",
-    "PSD",
-    "AASHTO",
-    "USCS",
-]
-
-
-def _chk_psd(fines: float, sand: float, gravel: float):
-    total_agg = fines + sand + gravel
-    if not isclose(total_agg, 100.0, rel_tol=ERROR_TOL):
-        errmsg = f"fines + sand + gravels = 100% not {total_agg}"
-        raise PSDError(errmsg)
-
-
-# Soil Symbols
-GRAVEL = "G"
-SAND = "S"
-SILT = "M"
-CLAY = "C"
-ORGANIC = "O"
-
-# Gradation Symbols
-WELL_GRADED = "W"
-POORLY_GRADED = "P"
-
-# Liquid Limit Symbols
-LOW_PLASTICITY = "L"
-HIGH_PLASTICITY = "H"
-
-
-#: Descriptions for various AASHTO soil classes.
-AASHTO_SOIL_DESC = {
-    "A-1-a": "Stone fragments, gravel, and sand",
-    "A-1-b": "Stone fragments, gravel, and sand",
-    "A-3": "Fine sand",
-    "A-2-4": "Silty or clayey gravel and sand",
-    "A-2-5": "Silty or clayey gravel and sand",
-    "A-2-6": "Silty or clayey gravel and sand",
-    "A-2-7": "Silty or clayey gravel and sand",
-    "A-4": "Silty soils",
-    "A-5": "Silty soils",
-    "A-6": "Clayey soils",
-    "A-7-5": "Clayey soils",
-    "A-7-6": "Clayey soils",
-}
-
-#: Descriptions for various USCS soil classes.
-USCS_SOIL_DESC = {
-    "GW": "Well graded gravels",
-    "GP": "Poorly graded gravels",
-    "GM": "Silty gravels",
-    "GC": "Clayey gravels",
-    "GM-GC": "Gravelly clayey silt",
-    "GW-GM": "Well graded gravel with silt",
-    "GP-GM": "Poorly graded gravel with silt",
-    "GW-GC": "Well graded gravel with clay",
-    "GP-GC": "Poorly graded gravel with clay",
-    "SW": "Well graded sands",
-    "SP": "Poorly graded sands",
-    "SM": "Silty sands",
-    "SC": "Clayey sands",
-    "SM-SC": "Sandy clayey silt",
-    "SW-SM": "Well graded sand with silt",
-    "SP-SM": "Poorly graded sand with silt",
-    "SW-SC": "Well graded sand with clay",
-    "SP-SC": "Poorly graded sand with clay",
-    "ML": "Inorganic silts with low plasticity",
-    "CL": "Inorganic clays with low plasticity",
-    "ML-CL": "Clayey silt with low plasticity",
-    "OL": "Organic clays with low plasticity",
-    "MH": "Inorganic silts with high plasticity",
-    "CH": "Inorganic clays with high plasticity",
-    "OH": "Organic silts with high plasticity",
-    "Pt": "Highly organic soils",
-}
+__all__ = ["AtterbergLimits", "PSD", "AASHTO", "USCS"]
 
 
-class PSDError(ValueError):
-    """
-    Exception raised when soil aggregates does not approximately sum up to
-    100%.
-    """
+class PSDAggSumError(ValueError):
+    pass
 
 
-class AtterbergLimits:
-    """
-    Water contents at which soil changes from one state to the other.
-
-    In 1911, a Swedish agriculture engineer ``Atterberg`` mentioned that a fined-grained
-    soil can exist in four states, namely, liquid, plastic, semi-solid or solid state.
-
-    The main use of Atterberg Limits is in the classification of soils.
+class SoilGradationError(ZeroDivisionError):
+    pass
 
-    :param float liquid_limit: Water content beyond which soils flows under their own weight.
-        It can also be defined as the minimum moisture content at which a soil flows upon
-        application of a very small shear force.
-    :param float plastic_limit: Water content at which plastic deformation can be initiated.
-        It is also the minimum water content at which soil can be rolled into a thread 3mm
-        thick (molded without breaking)
-    """
 
-    def __init__(self, liquid_limit: float, plastic_limit: float):
-        self.liquid_limit = liquid_limit
-        self.plastic_limit = plastic_limit
+class _SoilClassifier(Protocol):
 
     @property
-    def plasticity_index(self) -> float:
-        """
-        Return the plasticity index of the soil.
-
-        Plasticity index is the range of water content over which the soil remains in the
-        plastic state. It is also the numerical difference between the liquid limit and
-        plastic limit of the soil.
-
-        .. math::
-
-            PI = LL - PL
-        """
-        return self.liquid_limit - self.plastic_limit
+    @abstractmethod
+    def soil_class(self): ...
 
     @property
-    @round_(ndigits=2)
-    def A_line(self) -> float:
-        """
-        Return the ``A-line`` which is used to determine if a soil is clayey or
-        silty.
-        """
-        return 0.73 * (self.liquid_limit - 20)
+    @abstractmethod
+    def soil_desc(self): ...
 
-    @property
-    def type_of_fines(self) -> str:
-        """
-        Return the type of fine soil, either ``CLAY`` or ``SILT``.
-        """
-        return CLAY if self.above_A_LINE() else SILT
-
-    def above_A_LINE(self) -> bool:
-        """
-        Checks if the soil sample is above A-Line.
-        """
-        return self.plasticity_index > self.A_line
-
-    def limit_plot_in_hatched_zone(self) -> bool:
-        """
-        Checks if soil sample plot in the hatched zone on the atterberg chart.
-        """
-        return 4 <= self.plasticity_index <= 7 and 10 < self.liquid_limit < 30
-
-    @round_(ndigits=2)
-    def liquidity_index(self, nmc: float) -> float:
-        r"""
-        Return the liquidity index of the soil.
 
-        Liquidity index of a soil indicates the nearness of its water content
-        to its liquid limit. When the soil is at the plastic limit its liquidity
-        index is zero. Negative values of the liquidity index indicate that the
-        soil is in a hard (desiccated) state. It is also known as Water-Plasticity
-        ratio.
+#: USCS symbol for gravel.
+GRAVEL: str = "G"
 
-        :param float nmc: Moisture contents of the soil in natural condition.
-            (Natural Moisture Content)
+#: USCS symbol for sand.
+SAND: str = "S"
 
-        .. math::
+#: USCS symbol for silt.
+SILT: str = "M"
 
-            I_l = \dfrac{w - PL}{PI} \cdot 100
-        """
-        return ((nmc - self.plastic_limit) / self.plasticity_index) * 100
+#: USCS symbol for clay.
+CLAY: str = "C"
 
-    @round_(ndigits=2)
-    def consistency_index(self, nmc: float) -> float:
-        r"""
-        Return the consistency index of the soil.
+#: USCS symbol for organic material.
+ORGANIC: str = "O"
 
-        Consistency index indicates the consistency (firmness) of soil. It shows the
-        nearness of the water content of the soil to its plastic limit. When the soil
-        is at the liquid limit, the consistency index is zero. The soil at consistency
-        index of zero will be extremely soft and has negligible shear strength. A soil
-        at a water content equal to the plastic limit has consistency index of 100%
-        indicating that the soil is relatively firm. A consistency index of greater than
-        100% shows the soil is relatively strong (semi-solid state). A negative value
-        indicate the soil is in the liquid state. It is also known as Relative Consistency.
+#: USCS symbol for well-graded material.
+WELL_GRADED: str = "W"
 
-        :param float nmc: Moisture contents of the soil in natural condition.
-            (Natural Moisture Content)
+#: USCS symbol for poorly-graded material.
+POORLY_GRADED: str = "P"
 
-        .. math::
+#: USCS symbol for low soil plasticity.
+LOW_PLASTICITY: str = "L"
 
-            I_c = \dfrac{LL - w}{PI} \cdot 100
-        """
-        return ((self.liquid_limit - nmc) / self.plasticity_index) * 100.0
+#: USCS symbol for high soil plasticity.
+HIGH_PLASTICITY: str = "H"
 
 
-class _SizeDistribution(NamedTuple):
-    """
-    Features obtained from the Particle Size Distribution graph.
-    """
+class _SoilGradation(NamedTuple):
+    """Features obtained from the Particle Size Distribution graph."""
 
     d_10: float
     d_30: float
     d_60: float
 
+    ERR_MSG: str = "d_10, d_30, and d_60 cannot be 0"
+
     @property
-    @round_(ndigits=2)
+    @round_
     def coeff_of_curvature(self) -> float:
-        """
-        Coefficient of curvature of soil sample.
-        """
-        return (self.d_30**2) / (self.d_60 * self.d_10)
+        try:
+            return (self.d_30**2) / (self.d_60 * self.d_10)
+        except ZeroDivisionError as e:
+            raise SoilGradationError(self.ERR_MSG) from e
 
     @property
-    @round_(ndigits=2)
+    @round_
     def coeff_of_uniformity(self) -> float:
-        """
-        Coefficient of uniformity of soil sample.
-        """
-        return self.d_60 / self.d_10
+        try:
+            return self.d_60 / self.d_10
+        except ZeroDivisionError as e:
+            raise SoilGradationError(self.ERR_MSG) from e
 
     def grade(self, coarse_soil: str) -> str:
-        """
-        Grade of soil sample. Soil grade can either be ``WELL_GRADED`` or
+        """Grade of soil sample. Soil grade can either be ``WELL_GRADED`` or
         ``POORLY_GRADED``.
 
-        :param str coarse_soil: Coarse fraction of the soil sample. Valid arguments
-            are ``GRAVEL`` or ``SAND``.
+        Parameters
+        ----------
+        coarse_soil : str
+            Coarse fraction of the soil sample. Valid arguments are :data:`GRAVEL`
+            or :data:`SAND`.
         """
+
         if coarse_soil == GRAVEL and (
             1 < self.coeff_of_curvature < 3 and self.coeff_of_uniformity >= 4
         ):
             grade = WELL_GRADED
 
         elif coarse_soil == SAND and (
             1 < self.coeff_of_curvature < 3 and self.coeff_of_uniformity >= 6
@@ -244,332 +102,644 @@
 
         else:
             grade = POORLY_GRADED
 
         return grade
 
 
-class PSD:
+class AtterbergLimits:
+    """Water contents at which soil changes from one state to the other.
+
+    In 1911, a Swedish agriculture engineer ``Atterberg`` mentioned that a
+    fined-grained soil can exist in four states, namely, liquid, plastic,
+    semi-solid or solid state.
+
+    The main use of Atterberg Limits is in the classification of soils.
+
+    Parameters
+    ----------
+    liquid_limit : float
+        Water content beyond which soils flows under their own weight.
+        It can also be defined as the minimum moisture content at which
+        a soil flows upon application of a very small shear force.
+
+    plastic_limit : float
+        Water content at which plastic deformation can be initiated. It
+        is also the minimum water content at which soil can be rolled into
+        a thread 3mm thick. (molded without breaking)
+
+    Attributes
+    ----------
+    plasticity_index : float
+    A_line : float
+    type_of_fines : str
+
+    Methods
+    -------
+    above_A_LINE
+    limit_plot_in_hatched_zone
+    liquidity_index
+    consistency_index
+
+    Examples
+    --------
+    >>> from geolysis.core.soil_classifier import AtterbergLimits as AL
+
+    >>> atterberg_limits = AL(liquid_limit=55.44, plastic_limit=33.31)
+    >>> atterberg_limits.plasticity_index
+    22.13
+    >>> atterberg_limits.A_line
+    25.87
+
+    >>> soil_type = atterberg_limits.type_of_fines
+    >>> soil_type
+    'M'
+    >>> USCS.SOIL_DESCRIPTIONS[soil_type]
+    'Silt'
+    >>> atterberg_limits.above_A_LINE()
+    False
+    >>> atterberg_limits.limit_plot_in_hatched_zone()
+    False
+
+    Negative values of liquidity index indicates that the soil is in a hard state.
+
+    >>> atterberg_limits.liquidity_index(nmc=15.26)
+    -81.56
+
+    A consistency index greater than 100% shows the soil is relatively strong.
+
+    >>> atterberg_limits.consistency_index(nmc=15.26)
+    181.56
     """
-    Quantitative proportions by mass of various sizes of particles present in a
-    soil.
+
+    def __init__(self, liquid_limit: float, plastic_limit: float):
+        self.liquid_limit = liquid_limit
+        self.plastic_limit = plastic_limit
+
+    @property
+    @round_
+    def plasticity_index(self) -> float:
+        """Plasticity index (PI) is the range of water content over which the
+        soil remains in the plastic state.
+
+        It is also the numerical difference between the liquid limit and plastic
+        limit of the soil.
+
+        .. math:: PI = LL - PL
+        """
+        return self.liquid_limit - self.plastic_limit
+
+    @property
+    @round_
+    def A_line(self) -> float:
+        """The ``A-line`` is used to determine if a soil is clayey or silty.
+
+        .. math:: A = 0.73(LL - 20)
+        """
+        return 0.73 * (self.liquid_limit - 20)
+
+    @property
+    def type_of_fines(self) -> str:
+        """Determines whether the soil is either :data:`CLAY` or :data:`SILT`."""
+        return CLAY if self.above_A_LINE() else SILT
+
+    def above_A_LINE(self) -> bool:
+        """Checks if the soil sample is above A-Line."""
+        return self.plasticity_index > self.A_line
+
+    def limit_plot_in_hatched_zone(self) -> bool:
+        """Checks if soil sample plot in the hatched zone on the atterberg
+        chart.
+        """
+        return 4 <= self.plasticity_index <= 7 and 10 < self.liquid_limit < 30
+
+    @round_
+    def liquidity_index(self, nmc: float) -> float:
+        r"""Return the liquidity index of the soil.
+
+        Liquidity index of a soil indicates the nearness of its ``natural water
+        content`` to its ``liquid limit``. When the soil is at the plastic limit
+        its liquidity index is zero. Negative values of the liquidity index
+        indicate that the soil is in a hard (desiccated) state. It is also known
+        as Water-Plasticity ratio.
+
+        Parameters
+        ----------
+        nmc : float
+            Moisture contents of the soil in natural condition. (Natural Moisture
+            Content)
+
+        Notes
+        -----
+        The ``liquidity index`` is given by the formula:
+
+        .. math:: I_l = \dfrac{w - PL}{PI} \cdot 100
+        """
+        return ((nmc - self.plastic_limit) / self.plasticity_index) * 100
+
+    @round_
+    def consistency_index(self, nmc: float) -> float:
+        r"""Return the consistency index of the soil.
+
+        Consistency index indicates the consistency (firmness) of soil. It shows
+        the nearness of the ``natural water content`` of the soil to its
+        ``plastic limit``. When the soil is at the liquid limit, the consistency
+        index is zero. The soil at consistency index of zero will be extremely
+        soft and has negligible shear strength. A soil at a water content equal
+        to the plastic limit has consistency index of 100% indicating that the
+        soil is relatively firm. A consistency index of greater than 100% shows
+        the soil is relatively strong (semi-solid state). A negative value indicate
+        the soil is in the liquid state. It is also known as Relative Consistency.
+
+        Parameters
+        ----------
+        nmc : float
+            Moisture contents of the soil in natural condition. (Natural Moisture
+            Content)
+
+        Notes
+        -----
+        The ``consistency index`` is given by the formula:
+
+        .. math:: I_c = \dfrac{LL - w}{PI} \cdot 100
+        """
+        return ((self.liquid_limit - nmc) / self.plasticity_index) * 100.0
+
+
+class PSD:
+    r"""Quantitative proportions by mass of various sizes of particles present
+    in a soil.
 
     Particle Size Distribution is a method of separation of soils into
     different fractions using a stack of sieves to measure the size of the
     particles in a sample and graphing the results to illustrate the
     distribution of the particle sizes.
 
-    :param float fines: Percentage of fines in soil sample i.e. the percentage
-        of soil sample passing through No. 200 sieve (0.075mm)
-    :param float sand: Percentage of sand in soil sample (%)
-    :param float gravel: Percentage of gravel in soil sample (%)
-    :param float d_10: Diameter at which 10% of the soil by weight is finer.
-    :param float d_30: Diameter at which 30% of the soil by weight is finer.
-    :param float d_60: Diameter at which 60% of the soil by weight is finer.
-
-    :raises PSDError: Raised when soil aggregates does not approximately sum up
-        to 100%.
+    Parameters
+    ----------
+    fines : float
+        Percentage of fines in soil sample i.e. the percentage of soil sample
+        passing through No. 200 sieve (0.075mm)
+    sand : float
+        Percentage of sand in soil sample.
+    gravel : float
+        Percentage of gravel in soil sample.
+    d_10 : float, unit=millimetre
+        Diameter at which 10% of the soil by weight is finer.
+    d_30 : float, unit=millimetre
+        Diameter at which 30% of the soil by weight is finer.
+    d_60 : float, unit=millimetre
+        Diameter at which 60% of the soil by weight is finer.
+
+    Attributes
+    ----------
+    coeff_of_curvature : float
+    coeff_of_uniformity : float
+    type_of_coarse : str
+
+
+    Raises
+    ------
+    PSDAggSumError
+        Raised when soil aggregates does not approximately sum up to 100%.
+    SoilGradationError
+        Raised when d_10, d_30, and d_60 are not provided.
+
+    Examples
+    --------
+    >>> from geolysis.core.soil_classifier import PSD
+
+    >>> psd = PSD(fines=30.25, sand=53.55, gravel=16.20)
+    >>> soil_type = psd.type_of_coarse
+    >>> soil_type
+    'S'
+    >>> USCS.SOIL_DESCRIPTIONS[soil_type]
+    'Sand'
+
+    Raises error because parameters d_10, d_30, and d_60 are not provided.
+
+    >>> psd.coeff_of_curvature
+    Traceback (most recent call last):
+        ...
+    SoilGradationError: d_10, d_30, and d_60 cannot be 0
+
+    >>> psd.coeff_of_uniformity
+    Traceback (most recent call last):
+        ...
+    SoilGradationError: d_10, d_30, and d_60 cannot be 0
+
+    >>> psd = PSD(fines=10.29, sand=81.89, gravel=7.83,
+    ...           d_10=0.07, d_30=0.30, d_60=0.8)
+    >>> psd.d_10, psd.d_30, psd.d_60
+    (0.07, 0.3, 0.8)
+    >>> psd.coeff_of_curvature
+    1.61
+    >>> psd.coeff_of_uniformity
+    11.43
+
+    >>> soil_grade = psd.grade()
+    >>> soil_grade
+    'W'
+    >>> USCS.SOIL_DESCRIPTIONS[soil_grade]
+    'Well graded'
     """
 
     def __init__(
         self,
         fines: float,
         sand: float,
         gravel: float,
         d_10: float = 0,
         d_30: float = 0,
         d_60: float = 0,
     ):
         self.fines = fines
         self.sand = sand
         self.gravel = gravel
-        self.size_dist = _SizeDistribution(d_10, d_30, d_60)
+        self.size_dist = _SoilGradation(d_10, d_30, d_60)
+
+        total_agg = self.fines + self.sand + self.gravel
+
+        if not isclose(total_agg, 100.0, rel_tol=ERROR_TOL):
+            err_msg = f"fines + sand + gravels = 100% not {total_agg}"
+            raise PSDAggSumError(err_msg)
+
+    @property
+    def d_10(self) -> float:
+        """Diameter at which 10% of the soil by weight is finer."""
+        return self.size_dist.d_10
+
+    @property
+    def d_30(self) -> float:
+        """Diameter at which 30% of the soil by weight is finer."""
+        return self.size_dist.d_30
 
-        _chk_psd(self.fines, self.sand, self.gravel)
+    @property
+    def d_60(self) -> float:
+        """Diameter at which 60% of the soil by weight is finer."""
+        return self.size_dist.d_60
 
     @property
     def type_of_coarse(self) -> str:
-        """
-        Return the type of coarse material i.e. either ``GRAVEL`` or ``SAND``.
+        """Determines whether the soil is either :data:`GRAVEL` or
+        :data:`SAND`.
         """
         return GRAVEL if self.gravel > self.sand else SAND
 
     @property
     def coeff_of_curvature(self) -> float:
-        r"""
-        Return the coefficient of curvature of the soil.
+        r"""Coefficient of curvature of soil sample.
+
+        Coefficient of curvature :math:`(C_c)` is given by the formula:
 
-        .. math::
+        .. math:: C_c = \dfrac{D^2_{30}}{D_{60} \times D_{10}}
 
-            C_c = \dfrac{D^2_{30}}{D_{60} \times D_{10}}
+        For the soil to be well graded, the value of :math:`C_c` must be
+        between 1 and 3.
         """
         return self.size_dist.coeff_of_curvature
 
     @property
     def coeff_of_uniformity(self) -> float:
-        r"""
-        Return the coefficient of uniformity of the soil.
+        r"""Coefficient of uniformity of soil sample.
+
+        Coefficient of uniformity :math:`(C_u)` is given by the formula:
 
-        .. math::
+        .. math:: C_u = \dfrac{D_{60}}{D_{10}}
 
-            C_u = \dfrac{D_{60}}{D_{10}}
+        :math:`C_u` value greater than 4 to 6 classifies the soil as well
+        graded for gravels and sands respectively. When :math:`C_u` is less
+        than 4, it is classified as poorly graded or uniformly graded soil.
+        Higher values of :math:`C_u` indicates that the soil mass consists
+        of soil particles with different size ranges.
         """
         return self.size_dist.coeff_of_uniformity
 
-    def _has_particle_sizes(self) -> bool:
-        """
-        Checks if soil sample has particle sizes.
-        """
+    def has_particle_sizes(self) -> bool:
+        """Checks if soil sample has particle sizes."""
         return all(self.size_dist)
 
     def grade(self) -> str:
-        r"""
-        Return the grade of the soil sample either ``WELL_GRADED`` or
-        ``POORLY_GRADED``.
+        r"""Return the grade of the soil sample, either :data:`WELL_GRADED`
+        or :data:`POORLY_GRADED`.
 
         Conditions for a well-graded soil:
 
         - :math:`1 \lt C_c \lt 3` and :math:`C_u \ge 4` (for gravels)
         - :math:`1 \lt C_c \lt 3` and :math:`C_u \ge 6` (for sands)
         """
         return self.size_dist.grade(coarse_soil=self.type_of_coarse)
 
 
 class AASHTO:
-    r"""
-    American Association of State Highway and Transportation Officials (AASHTO)
-    classification system.
-
-    The AASHTO classification system is useful for classifying soils for highways. It
-    categorizes soils for highways based on particle size analysis and plasticity
-    characteristics. It classifies both coarse-grained and fine-grained soils into eight
-    main groups (A1-A7) with subgroups, along with a separate category (A8) for organic
-    soils.
+    r"""American Association of State Highway and Transportation Officials
+    (AASHTO) classification system.
+
+    The AASHTO classification system is useful for classifying soils for highways.
+    It categorizes soils for highways based on particle size analysis and
+    plasticity characteristics. It classifies both coarse-grained and fine-grained
+    soils into eight main groups (A1-A7) with subgroups, along with a separate
+    category (A8) for organic soils.
 
     - ``A1 ~ A3`` (Granular Materials) :math:`\le` 35% pass No. 200 sieve
     - ``A4 ~ A7`` (Silt-clay Materials) :math:`\ge` 36% pass No. 200 sieve
+    - ``A8`` (Organic Materials)
 
-    The Group Index ``(GI)`` is used to further evaluate soils with a group (subgroups).
-    When calculating ``GI`` from the equation below, if any term in the parenthesis
-    becomes negative, it is drop and not given a negative value. The maximum values of
-    :math:`(F_{200} - 35)` and :math:`(F_{200} - 15)` are taken as 40 and :math:`(LL - 40)`
-    and :math:`(PI - 10)` as 20.
-
-    If the computed value for ``GI`` is negative, it is reported as zero.
-
-    In general, the rating for the pavement subgrade is inversely proportional to the ``GI``
-    (lower the ``GI``, better the material). For e.g., a ``GI`` of zero indicates a good
-    subgrade, whereas a group index of 20 or greater shows a very poor subgrade.
-
-    .. note::
-
-        The ``GI`` must be mentioned even when it is zero, to indicate that the soil has been
-        classified as per AASHTO system.
-
-    :param float liquid_limit: Water content beyond which soils flows under their own weight.
-    :param float plasticity_index: Range of water content over which soil remains in plastic
-        condition.
-    :param float fines: Percentage of fines in soil sample i.e. the percentage of soil
-        sample passing through No. 200 sieve (0.075mm).
-    :kwparam bool add_group_idx: Used to indicate whether the group index should be added to
-        the classification or not. Defaults to True.
-    """
+    The Group Index ``(GI)`` is used to further evaluate soils within a group.
+
+    Parameters
+    ----------
+    liquid_limit : float
+        Water content beyond which soils flows under their own weight.
+    plasticity_index : float
+        Range of water content over which soil remains in plastic condition.
+    fines : float
+        Percentage of fines in soil sample i.e. the percentage of soil sample
+        passing through No. 200 sieve (0.075mm).
+    add_group_idx : bool, default=True
+        Used to indicate whether the group index should be added to the classification
+        or not. Defaults to True.
+
+    Notes
+    -----
+    The ``GI`` must be mentioned even when it is zero, to indicate that the soil has
+    been classified as per AASHTO system.
+
+    .. math:: GI = (F_{200} - 35)[0.2 + 0.005(LL - 40)] + 0.01(F_{200} - 15)(PI - 10)
+
+    Examples
+    --------
+    >>> from geolysis.core.soil_classifier import AASHTO
+
+    >>> aashto_clf = AASHTO(liquid_limit=30.2, plasticity_index=6.3, fines=11.18)
+    >>> aashto_clf.group_index()
+    0.0
+    >>> aashto_clf.soil_class
+    'A-2-4(0)'
+    >>> aashto_clf.soil_desc
+    'Silty or clayey gravel and sand'
+
+    If you would like to exclude the group index from the classification, you can do
+    the following:
+
+    >>> aashto_clf.add_group_idx = False
+    >>> aashto_clf.soil_class
+    'A-2-4'
+    """
+
+    SOIL_DESCRIPTIONS = {
+        "A-1-a": "Stone fragments, gravel, and sand",
+        "A-1-b": "Stone fragments, gravel, and sand",
+        "A-3": "Fine sand",
+        "A-2-4": "Silty or clayey gravel and sand",
+        "A-2-5": "Silty or clayey gravel and sand",
+        "A-2-6": "Silty or clayey gravel and sand",
+        "A-2-7": "Silty or clayey gravel and sand",
+        "A-4": "Silty soils",
+        "A-5": "Silty soils",
+        "A-6": "Clayey soils",
+        "A-7-5": "Clayey soils",
+        "A-7-6": "Clayey soils",
+    }
 
     def __init__(
         self,
         liquid_limit: float,
         plasticity_index: float,
         fines: float,
         add_group_idx=True,
     ):
         self.liquid_limit = liquid_limit
         self.plasticity_index = plasticity_index
         self.fines = fines
         self.add_group_idx = add_group_idx
 
-    def group_index(self) -> float:
-        """
-        Return the Group Index (GI) of the soil sample.
-
-        .. math::
-
-            GI = (F_{200} - 35)[0.2 + 0.005(LL - 40)] + 0.01(F_{200} - 15)(PI - 10)
-
-        - :math:`F_{200}`: Percentage by mass passing American Sieve No. 200.
-        - LL: Liquid Limit (%), expressed as a whole number.
-        - PI: Plasticity Index (%), expressed as a whole number.
-        """
-        x_1 = 1 if (x_0 := self.fines - 35) < 0 else min(x_0, 40)
-        x_2 = 1 if (x_0 := self.liquid_limit - 40) < 0 else min(x_0, 20)
-        x_3 = 1 if (x_0 := self.fines - 15) < 0 else min(x_0, 40)
-        x_4 = 1 if (x_0 := self.plasticity_index - 10) < 0 else min(x_0, 20)
-
-        grp_idx = round(x_1 * (0.2 + 0.005 * x_2) + 0.01 * x_3 * x_4, 0)
-
-        return 0 if grp_idx <= 0 else ceil(grp_idx)
-
-    @property
-    def soil_class(self) -> str:
-        """
-        Return the AASHTO classification of the soil.
-        """
-        return self._classify()
-
-    @property
-    def soil_desc(self) -> str | None:
-        """
-        Return the AASHTO description of the soil.
-        """
-        tmp_state = self.add_group_idx
-        try:
-            self.add_group_idx = False
-            return AASHTO_SOIL_DESC[self._classify()]
-        finally:
-            self.add_group_idx = tmp_state
-
     def _classify(self) -> str:
         # Silts A4-A7
         if self.fines > 35:
-            return self._fine_soil_classifier()
-
+            soil_class = self._fine_soil_classifier()
         # Coarse A1-A3
-        return self._coarse_soil_classifier()
+        else:
+            soil_class = self._coarse_soil_classifier()
+
+        return (
+            f"{soil_class}({self.group_index():.0f})"
+            if self.add_group_idx
+            else soil_class
+        )
 
     def _coarse_soil_classifier(self) -> str:
         # A-3, Fine sand
         if self.fines <= 10 and isclose(
             self.plasticity_index, 0, rel_tol=ERROR_TOL
         ):
-            clf = "A-3"
+            soil_class = "A-3"
 
         # A-1-a -> A-1-b, Stone fragments, gravel, and sand
         elif self.fines <= 15 and self.plasticity_index <= 6:
-            clf = "A-1-a"
+            soil_class = "A-1-a"
 
         elif self.fines <= 25 and self.plasticity_index <= 6:
-            clf = "A-1-b"
+            soil_class = "A-1-b"
 
         # A-2-4 -> A-2-7, Silty or clayey gravel and sand
         elif self.liquid_limit <= 40:
-            if self.plasticity_index <= 10:
-                clf = "A-2-4"
-            else:
-                clf = "A-2-6"
+            soil_class = "A-2-4" if self.plasticity_index <= 10 else "A-2-6"
 
         else:
-            if self.plasticity_index <= 10:
-                clf = "A-2-5"
-            else:
-                clf = "A-2-7"
+            soil_class = "A-2-5" if self.plasticity_index <= 10 else "A-2-7"
 
-        return f"{clf}({self.group_index()})" if self.add_group_idx else clf
+        return soil_class
 
     def _fine_soil_classifier(self) -> str:
         # A-4 -> A-5, Silty Soils
         # A-6 -> A-7, Clayey Soils
         if self.liquid_limit <= 40:
-            clf = "A-4" if self.plasticity_index <= 10 else "A-6"
-
+            soil_class = "A-4" if self.plasticity_index <= 10 else "A-6"
         else:
             if self.plasticity_index <= 10:
-                clf = "A-5"
+                soil_class = "A-5"
             else:
                 _x = self.liquid_limit - 30
-                clf = "A-7-5" if self.plasticity_index <= _x else "A-7-6"
-
-        return f"{clf}({self.group_index()})" if self.add_group_idx else clf
-
+                soil_class = (
+                    "A-7-5" if self.plasticity_index <= _x else "A-7-6"
+                )
 
-class USCS:
-    """
-    Unified Soil Classification System (USCS).
+        return soil_class
 
-    The Unified Soil Classification System, initially developed by Casagrande in 1948 and
-    later modified in 1952, is widely utilized in engineering projects involving soils. It
-    is the most popular system for soil classification and is similar to Casagrande's
-    Classification System. The system relies on particle size analysis and atterberg limits
-    for classification.
+    @property
+    def soil_class(self) -> str:
+        """Return the AASHTO classification of the soil."""
+        return self._classify()
 
-    In this system, soils are first classified into two categories:
+    @property
+    def soil_desc(self) -> str:
+        """Return the AASHTO description of the soil."""
+        tmp_state = self.add_group_idx
+        try:
+            self.add_group_idx = False
+            soil_cls = self.soil_class
+            return AASHTO.SOIL_DESCRIPTIONS[soil_cls]
+        finally:
+            self.add_group_idx = tmp_state
 
-    - Coarse grained soils: If more than 50% of the soils is retained on No. 200 (0.075 mm)
-      sieve, it is designated as coarse-grained soil.
+    def group_index(self) -> float:
+        """Return the Group Index (GI) of the soil sample."""
+        a = 1 if (x_0 := self.fines - 35) < 0 else min(x_0, 40)
+        b = 1 if (x_0 := self.liquid_limit - 40) < 0 else min(x_0, 20)
+        c = 1 if (x_0 := self.fines - 15) < 0 else min(x_0, 40)
+        d = 1 if (x_0 := self.plasticity_index - 10) < 0 else min(x_0, 20)
 
-    - Fine grained soils: If more than 50% of the soil passes through No. 200 sieve, it is
-      designated as fine grained soil.
+        return round(a * (0.2 + 0.005 * b) + 0.01 * c * d, 0)
 
-    Highly Organic soils are identified by visual inspection. These soils are termed as Peat.
-    (:math:`P_t`)
 
-    Soil symbols:
+class USCS:
+    """Unified Soil Classification System (USCS).
 
-    - G: Gravel
-    - S: Sand
-    - M: Silt
-    - C: Clay
-    - O: Organic Clay
-    - Pt: Peat
+    The Unified Soil Classification System, initially developed by Casagrande in
+    1948 and later modified in 1952, is widely utilized in engineering projects
+    involving soils. It is the most popular system for soil classification and is
+    similar to Casagrande's Classification System. The system relies on particle
+    size analysis and atterberg limits for classification.
 
-    Liquid limit symbols:
+    In this system, soils are first classified into two categories:
 
-    - H: High Plasticity :math:`(LL > 50)`
-    - L: Low Plasticity :math:`(LL < 50)`
+    - Coarse grained soils: If more than 50% of the soils is retained on No. 200
+      (0.075 mm) sieve, it is designated as coarse-grained soil.
 
-    Gradation symbols:
+    - Fine grained soils: If more than 50% of the soil passes through No. 200 sieve,
+      it is designated as fine grained soil.
 
-    - W: Well-graded
-    - P: Poorly-graded
+    Highly Organic soils are identified by visual inspection. These soils are termed
+    as Peat. (:math:`P_t`)
 
-    :param float liquid_limit: Water content beyond which soils flows under their own weight.
-        It can also be defined as the minimum moisture content at which a soil flows upon
+    Parameters
+    ----------
+    liquid_limit : float
+        Water content beyond which soils flows under their own weight. It can also
+        be defined as the minimum moisture content at which a soil flows upon
         application of a very small shear force.
-    :param float plastic_limit: Water content at which plastic deformation can be initiated.
-        It is also the minimum water content at which soil can be rolled into a thread 3mm
-        thick (molded without breaking)
-    :param float fines: Percentage of fines in soil sample i.e. the percentage of soil sample
-        passing through No. 200 sieve (0.075mm)
-    :param float sand: Percentage of sand in soil sample (%)
-    :param float gravel: Percentage of gravel in soil sample (%)
-    :param float d_10: Diameter at which 10% of the soil by weight is finer.
-    :param float d_30: Diameter at which 30% of the soil by weight is finer.
-    :param float d_60: Diameter at which 60% of the soil by weight is finer.
-    :kwparam bool organic: Indicates whether soil is organic or not.
-    """
+    plastic_limit : float
+        Water content at which plastic deformation can be initiated. It is also the
+        minimum water content at which soil can be rolled into a thread 3mm thick
+        (molded without breaking)
+    fines : float
+        Percentage of fines in soil sample i.e. The percentage of soil sample passing
+        through No. 200 sieve (0.075mm)
+    sand : float
+        Percentage of sand in soil sample (%)
+    gravel : float
+        Percentage of gravel in soil sample (%)
+    d_10 : float, mm
+        Diameter at which 10% of the soil by weight is finer.
+    d_30 : float, mm
+        Diameter at which 30% of the soil by weight is finer.
+    d_60 : float, mm
+        Diameter at which 60% of the soil by weight is finer.
+    organic : bool, default=False
+        Indicates whether soil is organic or not.
+
+    Attributes
+    ----------
+    atterberg_limits : AtterbergLimits
+    psd : PSD
+    soil_class : str
+    soil_desc : str
+
+    Examples
+    --------
+    >>> from geolysis.core.soil_classifier import USCS
+
+    >>> uscs_clf = USCS(liquid_limit=34.1, plastic_limit=21.1,
+    ...                 fines=47.88, sand=37.84, gravel=14.28)
+    >>> uscs_clf.soil_class
+    'SC'
+    >>> uscs_clf.soil_desc
+    'Clayey sands'
+
+    >>> uscs_clf = USCS(liquid_limit=27.7, plastic_limit=22.7,
+    ...                 fines=18.95, sand=77.21, gravel=3.84)
+    >>> uscs_clf.soil_class
+    'SM-SC'
+    >>> uscs_clf.soil_desc
+    'Sandy clayey silt'
+
+    >>> uscs_clf = USCS(liquid_limit=30.8, plastic_limit=20.7, fines=10.29,
+    ...                 sand=81.89, gravel=7.83, d_10=0.07, d_30=0.3, d_60=0.8)
+    >>> uscs_clf.soil_class
+    'SW-SC'
+    >>> uscs_clf.soil_desc
+    'Well graded sand with clay'
+
+    Soil gradation (d_10, d_30, d_60) is needed to obtain soil description for
+    certain type of soils.
+
+    >>> uscs_clf = USCS(liquid_limit=30.8, plastic_limit=20.7,
+    ...                 fines=10.29, sand=81.89, gravel=7.83)
+    >>> uscs_clf.soil_class
+    'SW-SC,SP-SC'
+    >>> uscs_clf.soil_desc
+    'Well graded sand with clay or Poorly graded sand with clay'
+    """
+
+    SOIL_DESCRIPTIONS = {
+        "G": "Gravel",
+        "S": "Sand",
+        "M": "Silt",
+        "C": "Clay",
+        "O": "Organic",
+        "W": "Well graded",
+        "P": "Poorly graded",
+        "L": "Low plasticity",
+        "H": "High plasticity",
+        "GW": "Well graded gravels",
+        "GP": "Poorly graded gravels",
+        "GM": "Silty gravels",
+        "GC": "Clayey gravels",
+        "GM-GC": "Gravelly clayey silt",
+        "GW-GM": "Well graded gravel with silt",
+        "GP-GM": "Poorly graded gravel with silt",
+        "GW-GC": "Well graded gravel with clay",
+        "GP-GC": "Poorly graded gravel with clay",
+        "SW": "Well graded sands",
+        "SP": "Poorly graded sands",
+        "SM": "Silty sands",
+        "SC": "Clayey sands",
+        "SM-SC": "Sandy clayey silt",
+        "SW-SM": "Well graded sand with silt",
+        "SP-SM": "Poorly graded sand with silt",
+        "SW-SC": "Well graded sand with clay",
+        "SP-SC": "Poorly graded sand with clay",
+        "ML": "Inorganic silts with low plasticity",
+        "CL": "Inorganic clays with low plasticity",
+        "ML-CL": "Clayey silt with low plasticity",
+        "OL": "Organic clays with low plasticity",
+        "MH": "Inorganic silts with high plasticity",
+        "CH": "Inorganic clays with high plasticity",
+        "OH": "Organic silts with high plasticity",
+        "Pt": "Highly organic soils",
+    }
 
     def __init__(
         self,
         liquid_limit: float,
         plastic_limit: float,
         fines: float,
         sand: float,
         gravel: float,
         *,
         d_10=0,
         d_30=0,
         d_60=0,
         organic=False,
     ):
-        self.atterberg_limits = AtterbergLimits(liquid_limit, plastic_limit)
-        self.psd = PSD(fines, sand, gravel, d_10, d_30, d_60)
+        self._atterberg_limits = AtterbergLimits(liquid_limit, plastic_limit)
+        self._psd = PSD(fines, sand, gravel, d_10, d_30, d_60)
         self.organic = organic
 
-    @property
-    def soil_class(self) -> str:
-        """
-        Return the USCS Classification of the soil.
-        """
-        return self._classify()
-
-    @property
-    def soil_desc(self) -> str | None:
-        """
-        Return the USCS description of the soil.
-        """
-        return USCS_SOIL_DESC[self._classify()]
-
     def _classify(self) -> str:
         # Fine grained, Run Atterberg
         if self.psd.fines > 50:
             return self._fine_soil_classifier()
 
         # Coarse grained, Run Sieve Analysis
         # Gravel or Sand
@@ -596,32 +766,34 @@
 
             # Below A-line
             else:
                 soil_class = f"{coarse_soil}{SILT}"
 
         elif 5 <= self.psd.fines <= 12:
             # Requires dual symbol based on graduation and plasticity chart
-            if self.psd._has_particle_sizes():
+            if self.psd.has_particle_sizes():
                 soil_class = self._dual_soil_classifier()
 
             else:
                 fine_soil = self.atterberg_limits.type_of_fines
                 soil_class = (
                     f"{coarse_soil}{WELL_GRADED}-{coarse_soil}{fine_soil},"
                     f"{coarse_soil}{POORLY_GRADED}-{coarse_soil}{fine_soil}"
                 )
 
         # Less than 5% pass No. 200 sieve
         # Obtain Cc and Cu from grain size graph
         else:
-            if self.psd._has_particle_sizes():
+            if self.psd.has_particle_sizes():
                 soil_class = f"{coarse_soil}{self.psd.grade()}"
 
             else:
-                soil_class = f"{coarse_soil}{WELL_GRADED} or {coarse_soil}{POORLY_GRADED}"
+                soil_class = (
+                    f"{coarse_soil}{WELL_GRADED},{coarse_soil}{POORLY_GRADED}"
+                )
 
         return soil_class
 
     def _fine_soil_classifier(self) -> str:
         if self.atterberg_limits.liquid_limit < 50:
             # Low LL
             # Above A-line and PI > 7
@@ -632,27 +804,56 @@
 
             # Limit plot in hatched area on plasticity chart
             elif self.atterberg_limits.limit_plot_in_hatched_zone():
                 soil_class = f"{SILT}{LOW_PLASTICITY}-{CLAY}{LOW_PLASTICITY}"
 
             # Below A-line or PI < 4
             else:
-                if self.organic:
-                    soil_class = f"{ORGANIC}{LOW_PLASTICITY}"
-
-                else:
-                    soil_class = f"{SILT}{LOW_PLASTICITY}"
+                soil_class = (
+                    f"{ORGANIC}{LOW_PLASTICITY}"
+                    if self.organic
+                    else f"{SILT}{LOW_PLASTICITY}"
+                )
 
         # High LL
         else:
             # Above A-Line
             if self.atterberg_limits.above_A_LINE():
                 soil_class = f"{CLAY}{HIGH_PLASTICITY}"
 
             # Below A-Line
             else:
-                if self.organic:
-                    soil_class = f"{ORGANIC}{HIGH_PLASTICITY}"
-                else:
-                    soil_class = f"{SILT}{HIGH_PLASTICITY}"
+                soil_class = (
+                    f"{ORGANIC}{HIGH_PLASTICITY}"
+                    if self.organic
+                    else f"{SILT}{HIGH_PLASTICITY}"
+                )
 
         return soil_class
+
+    @property
+    def atterberg_limits(self) -> AtterbergLimits:
+        """Return the atterberg limits of soil."""
+        return self._atterberg_limits
+
+    @property
+    def psd(self) -> PSD:
+        """Return the particle size distribution of soil."""
+        return self._psd
+
+    @property
+    def soil_class(self) -> str:
+        """Return the USCS classification of the soil."""
+        return self._classify()
+
+    @property
+    def soil_desc(self) -> str:
+        """Return the USCS description of the soil."""
+        soil_cls = self.soil_class
+        try:
+            soil_descr = USCS.SOIL_DESCRIPTIONS[soil_cls]
+        except KeyError:
+            soil_descr = " or ".join(
+                map(USCS.SOIL_DESCRIPTIONS.get, soil_cls.split(","))
+            )  # type: ignore
+
+        return soil_descr
```

### Comparing `geolysis-0.2.0/geolysis/spt.py` & `geolysis-0.3.0/geolysis/core/spt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,424 +1,633 @@
-import functools
+from abc import abstractmethod
+from dataclasses import KW_ONLY, dataclass
 from statistics import StatisticsError
-from typing import Callable, Iterable, Sequence
+from typing import Protocol, Sequence
 
-from geolysis.constants import ERROR_TOL, UNITS
-from geolysis.utils import FloatOrInt, isclose, log10, mean, round_, sqrt
+from .constants import ERROR_TOL
+from .utils import isclose, log10, mean, round_, sqrt
 
 __all__ = [
-    "weighted_avg_spt_n_val",
-    "avg_uncorrected_spt_n_val",
-    "SPTCorrections",
+    "WeightedSPT",
+    "AverageSPT",
+    "MinSPT",
+    "EnergyCorrection",
+    "GibbsHoltzOPC",
+    "BazaraaPeckOPC",
+    "PeckOPC",
+    "LiaoWhitmanOPC",
+    "SkemptonOPC",
+    "DilatancyCorrection",
 ]
 
 
-class OverburdenPressureError(ValueError):
-    """
-    Exception raised for overburden pressure related errors.
-    """
-
-
-@round_(ndigits=0)
-def weighted_avg_spt_n_val(corrected_spt_vals: Sequence[float]) -> float:
-    r"""
-    Calculates the weighted average of the corrected SPT N-values in the foundation
-    influence zone. (:math:`N_{design}`)
-
-    Due to uncertainty in field procedure in standard penetration test and also
-    to consider all the N-value in the influence zone of a foundation, a method
-    was suggested to calculate the design N-value which should be used in
-    calculating the allowable bearing capacity of shallow foundation rather than
-    using a particular N-value. All the N-value from the influence zone is taken
-    under consideration by giving the highest weightage to the closest N-value
-    from the base.
-
-    The determination of :math:`N_{design}` is given by:
-
-    .. math::
-
-        N_{design} = \dfrac{\sum_{i=1}^{n} \frac{N_i}{i^2}}{\sum_{i=1}^{n} \frac{1}{i^2}}
-
-    - influence zone = :math:`D_f + 2B` or to a depth up to which soil
-      types are approximately the same.
-    - B = width of footing
-    - :math:`n` = number of layers in the influence zone.
-    - :math:`N_i` = corrected N-value at ith layer from the footing base.
-
-    .. note::
-
-        Alternatively, for ease in calculation, the lowest N-value from the influence zone
-        can be taken as the :math:`N_{design}` as suggested by ``Terzaghi & Peck (1948)``.
-
-    :param Sequence[float] corrected_spt_vals: Corrected SPT N-values within the
-        foundation influence zone i.e. :math:`D_f` to :math:`D_f + 2B`
-
-    :return: Weighted average of corrected SPT N-values
-    :rtype: float
-
-    :raises StatisticError: If ``corrected_spt_vals`` is empty, StatisticError is raised.
-    """
-    if not corrected_spt_vals:
-        err_msg = "spt_n_design requires at least one corrected spt n-value"
-        raise StatisticsError(err_msg)
-
-    total_num = 0.0
-    total_den = 0.0
-
-    for i, corrected_spt in enumerate(corrected_spt_vals, start=1):
-        idx_weight = 1 / i**2
-        total_num += idx_weight * corrected_spt
-        total_den += idx_weight
-
-    return total_num / total_den
+class OPCError(ValueError):
+    pass
 
 
-@round_(ndigits=0)
-def avg_uncorrected_spt_n_val(uncorrected_spt_vals: Sequence[float]) -> float:
-    """
-    Calculates the average of the uncorrected SPT N-values in the foundation
-    influence zone.
-
-    :param Sequence[float] uncorrected_spt_vals: Uncorrected SPT N-values within the
-        foundation influence zone i.e. :math:`D_f` |rarr| :math:`D_f + 2B`. Only water
-        table correction suggested.
-
-    :return: Average of corrected SPT N-values
-    :rtype: float
-
-    :raises StatisticError: If ``uncorrected_spt_vals`` is empty, StatisticError is raised.
-    """
-    if not uncorrected_spt_vals:
-        msg = "spt_n_val requires at least one corrected spt n-value"
-        raise StatisticsError(msg)
-
-    return mean(uncorrected_spt_vals)
-
-
-class SPTCorrections:
-    r"""
-    SPT N-value correction for **Overburden Pressure** and **Dilatancy**.
-
-    There are three (3) different SPT corrections namely:
+class _SPTNDesign(Protocol):
+    def spt_n_design(self) -> float: ...
 
-    - Energy Correction / Correction for Field Procedures
-    - Overburden Pressure Corrections
-    - Dilatancy Correction
 
-    Energy correction is used to standardized the SPT N-values for field procedures.
-
-    In cohesionless soils, penetration resistance is affected by overburden pressure.
-    Soils with the same density but different confining pressures have varying penetration
-    numbers, with higher confining pressures leading to higher penetration numbers. As depth
-    increases, confining pressure rises, causing underestimation of penetration numbers
-    at shallow depths and overestimation at deeper depths. The need for corrections in
-    Standard Penetration Test (SPT) values was acknowledged only in 1957 by Gibbs & Holtz,
-    meaning data published before this, like Terzaghi's, are based on uncorrected values.
-
-    The general formula for overburden pressure correction is:
+class _SPTCorrection(Protocol):
+    @property
+    @abstractmethod
+    def corrected_spt_number(self) -> float: ...
+
+
+class _OPC(Protocol):
+    std_spt_number: float
+    eop: float
+
+    @property
+    @abstractmethod
+    def correction(self) -> float: ...
+
+    @property
+    @round_
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        corrected_spt = self.correction * self.std_spt_number
+        return min(corrected_spt, 2 * self.std_spt_number)
+
+
+@dataclass
+class WeightedSPT:
+    r"""Calculates the weighted average of the corrected SPT N-values
+    within the foundation influence zone.
+
+    Due to uncertainty in field procedure in standard penetration test
+    and also to consider all the N-value in the influence zone of a
+    foundation, a method was suggested to calculate the design N-value
+    which should be used in calculating the allowable bearing capacity
+    of shallow foundation rather than using a particular N-value. All
+    the N-value from the influence zone is taken under consideration by
+    giving the highest weightage to the closest N-value from the base.
+
+    Parameters
+    ----------
+    spt_numbers : Sequence[float]
+        SPT N-values within the foundation influence zone. ``spt_numbers``
+        can either be **corrected** or **uncorrected** SPT N-values.
+
+    Notes
+    -----
+    Weighted average is given by the formula:
 
     .. math::
 
-        (N_1)_{60} = C_N \cdot N_{60} \le 2 \cdot N_{60}
-
-    Where:
-
-    - :math:`C_N` = Overburden Pressure Correction Factor
-
-    Available overburden pressure corrections are given by the following authors:
+        N_{design} = \dfrac{\sum_{i=1}^{n} \frac{N_i}{i^2}}{\sum_{i=1}^{n}
+                     \frac{1}{i^2}}
 
-    - Gibbs & Holtz (1957)
-    - Peck et al (1974)
-    - Liao & Whitman (1986)
-    - Skempton (1986)
-    - Bazaraa & Peck (1969)
-
-    **Dilatancy Correction** is a correction for silty fine sands and fine sands below the
-    water table that develop pore pressure which is not easily dissipated. The pore pressure
-    increases the resistance of the soil hence the standard penetration number (N).
-    Correction of silty fine sands recommended by ``Terzaghi and Peck (1948)`` if :math:`N_{60}`
-    exceeds 15.
+    Examples
+    --------
+    >>> from geolysis.core.spt import WeightedSPT
+    >>> wgt = WeightedSPT([7.0, 15.0, 18.0])
+    >>> wgt.spt_n_design()
+    9.3673
     """
 
-    unit = UNITS.unitless
-
-    @staticmethod
-    def map(
-        opc_func: Callable[..., FloatOrInt],
-        standardized_spt_vals: Iterable[float],
-        dc_func: Callable[..., FloatOrInt] | None = None,
-        **kwargs,
-    ):
-        """
-        Returns an iterator from computing functions (``opc_func``, "dc_func") using
-        arguments from the iterable (``standard_spt_vals``).
+    spt_numbers: Sequence[float]
 
-        :param Callable opc_func: Overburden pressure correction function to use.
-        :param Callable | None dc_func: Dilatancy correction function to use.
-        :param dict kwargs: Keyword arguments to pass to ```opc_func`.
+    @round_
+    def spt_n_design(self) -> float:
+        """SPT N-design.
+
+        Raises
+        ------
+        StatisticError
+            Raised if ``spt_numbers`` is empty.
         """
-        opc_func = functools.partial(opc_func, **kwargs)
-        corrected_spt_vals = map(opc_func, standardized_spt_vals)
-
-        if dc_func:
-            corrected_spt_vals = map(dc_func, corrected_spt_vals)
-
-        return corrected_spt_vals
-
-    @staticmethod
-    @round_(ndigits=2)
-    def energy_correction(
-        recorded_spt_val: float,
-        percentage_energy=0.6,
-        *,
-        hammer_efficiency=0.6,
-        borehole_diameter_correction=1,
-        sampler_correction=1,
-        rod_length_correction=0.75,
-    ) -> FloatOrInt:
-        r"""
-        Return SPT N-value standardized for field procedures.
-
-        On the basis of field observations, it appears reasonable to standardize the field
-        SPT N-value as a function of the input driving energy and its dissipation around
-        the sampler around the surrounding soil. The variations in testing procedures may
-        be at least partially compensated by converting the measured N-value to :math:`N_{60}`.
-
-        .. math::
-
-            N_{60} = \dfrac{E_H \cdot C_B \cdot C_S \cdot C_R \cdot N}{0.6}
-
-        Where:
-
-        - :math:`N_{60}` = Corrected SPT N-value for field procedures
-        - :math:`E_{H}`  = Hammer efficiency
-        - :math:`C_{B}`  = Borehole diameter correction
-        - :math:`C_{S}`  = Sampler correction
-        - :math:`C_{R}`  = Rod length correction
-        - N              = Recorded SPT N-value in field
-
-        The values of :math:`E_H`, :math:`C_B`, :math:`C_S`, and :math:`C_R` can be found in
-        the table below.
-
-        .. table:: Correction table for field procedure of SPT N-value
-
-            +--------------------+------------------------------+--------------------------------+
-            | SPT Hammer Efficiencies                                                            |
-            +====================+==============================+================================+
-            | **Hammer Type**    | **Hammer Release Mechanism** | **Efficiency**, :math:`E_H`    |
-            +--------------------+------------------------------+--------------------------------+
-            | Automatic          | Trip                         | 0.70                           |
-            +--------------------+------------------------------+--------------------------------+
-            | Donut              | Hand dropped                 | 0.60                           |
-            +--------------------+------------------------------+--------------------------------+
-            | Donut              | Cathead+2 turns              | 0.50                           |
-            +--------------------+------------------------------+--------------------------------+
-            | Safety             | Cathead+2 turns              | 0.55 - 0.60                    |
-            +--------------------+------------------------------+--------------------------------+
-            | Drop/Pin           | Hand dropped                 | 0.45                           |
-            +--------------------+------------------------------+--------------------------------+
-            | Borehole, Sampler and Rod Correction                                               |
-            +--------------------+------------------------------+--------------------------------+
-            | **Factor**         | **Equipment Variables**      | **Correction Factor**          |
-            +--------------------+------------------------------+--------------------------------+
-            | Borehole Dia       | 65 - 115 mm (2.5-4.5 in)     | 1.00                           |
-            | Factor,            |                              |                                |
-            | :math:`C_B`        |                              |                                |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | 150 mm (6 in)                | 1.05                           |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | 200 mm (8 in)                | 1.15                           |
-            +--------------------+------------------------------+--------------------------------+
-            | Sampler            | Standard sampler             | 1.00                           |
-            | Correction,        |                              |                                |
-            | :math:`C_S`        |                              |                                |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | Sampler without liner        | 1.20                           |
-            |                    | (not recommended)            |                                |
-            +--------------------+------------------------------+--------------------------------+
-            | Rod Length         | 3 - 4 m (10-13 ft)           | 0.75                           |
-            | Correction,        |                              |                                |
-            | :math:`C_R`        |                              |                                |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | 4 - 6 m (13-20 ft)           | 0.85                           |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | 6 - 10 m (20-30 ft)          | 0.95                           |
-            +--------------------+------------------------------+--------------------------------+
-            |                    | >10 m (>30 ft)               | 1.00                           |
-            +--------------------+------------------------------+--------------------------------+
-
-        :param float percentage_energy: Percentage energy reaching the tip of the sampler.
-        :param int recorded_spt_val: Recorded SPT N-value from field.
-        :kwparam float hammer_efficiency: hammer efficiency, defaults to 0.6
-        :kwparam float borehole_diameter_correction: borehole diameter correction,
-            defaults to 1.0
-        :kwparam float sampler_correction: sampler correction, defaults to 1.0
-        :kwparam float rod_length_correction: rod Length correction, defaults to 0.75
-
-        .. note::
-
-            The ``energy correction`` is to be applied irrespective of the type of soil.
-        """
-        correction = (
-            hammer_efficiency
-            * borehole_diameter_correction
-            * sampler_correction
-            * rod_length_correction
-        )
-
-        return (correction * recorded_spt_val) / percentage_energy
-
-    @staticmethod
-    @round_(ndigits=2)
-    def terzaghi_peck_dc_1948(corrected_spt_val: float) -> float:
-        r"""
-        Return the dilatancy spt correction.
-
-        :param float corrected_spt_val: Corrected SPT N-value. This should be corrected
-            using any of the overburden pressure corrections.
-
-        .. math::
-
-            (N_1)_{60} &= 15 + \dfrac{1}{2}((N_1)_{60} - 15) \, , \, (N_1)_{60} \gt 15
-
-            (N_1)_{60} &= (N_1)_{60} \, , \, (N_1)_{60} \le 15
+        if not self.spt_numbers:
+            err_msg = "method requires at least one data point."
+            raise StatisticsError(err_msg)
+
+        sum_total = 0.0
+        total_wgts = 0.0
+
+        for i, corrected_spt in enumerate(self.spt_numbers, start=1):
+            wgt = 1 / i**2
+            sum_total += wgt * corrected_spt
+            total_wgts += wgt
+
+        return sum_total / total_wgts
+
+
+@dataclass
+class AverageSPT:
+    r"""Calculates the average of the corrected SPT N-values within the
+    foundation influence zone.
+
+    Parameters
+    ----------
+    spt_numbers : Sequence[float]
+        SPT N-values within the foundation influence zone. ``spt_numbers``
+        can either be **corrected** or **uncorrected** SPT N-values.
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import AverageSPT
+    >>> wgt = AverageSPT([7.0, 15.0, 18.0])
+    >>> wgt.spt_n_design()
+    13.3333
+    """
 
-        .. note::
+    spt_numbers: Sequence[float]
 
-            For coarse sand, this correction is not required. In applying this correction,
-            overburden pressure correction is applied first and then dilatancy correction
-            is applied.
+    @round_
+    def spt_n_design(self) -> float:
+        """SPT N-design.
+
+        Raises
+        ------
+        StatisticError
+            Raised if ``spt_numbers`` is empty.
         """
+        try:
+            return mean(self.spt_numbers)
+        except StatisticsError as e:
+            err_msg = "method requires at least one data point."
+            raise StatisticsError(err_msg) from None
+
+
+@dataclass
+class MinSPT:
+    """The lowest N-value within the influence zone can be taken as the
+    :math:`N_{design}` as suggested by ``Terzaghi & Peck (1948)``.
+
+    Parameters
+    ----------
+    spt_numbers : Sequence[float]
+        SPT N-values within the foundation influence zone. i.e. ``spt_numbers``
+        can either be **corrected** or **uncorrected** SPT N-values.
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import MinSPT
+    >>> wgt = MinSPT([7.0, 15.0, 18.0])
+    >>> wgt.spt_n_design()
+    7.0
+    """
 
-        if corrected_spt_val <= 15:
-            return corrected_spt_val
-
-        return 15 + 0.5 * (corrected_spt_val - 15)
-
-    @staticmethod
-    @round_(ndigits=2)
-    def gibbs_holtz_opc_1957(spt_n_60: float, eop: float) -> float:
-        r"""
-        Return the overburden pressure correction given by ``Gibbs and Holtz
-        (1957)``.
-
-        :param float spt_n_60: SPT N-value standardized for field procedures.
-        :param float eop: Effective overburden pressure (:math:`kN/m^2`).
-
-        .. math::
-
-            C_N = \dfrac{350}{\sigma_o + 70} \, \sigma_o \le 280kN/m^2
-
-        .. note::
+    spt_numbers: Sequence[float]
 
-            :math:`\frac{N_c}{N_{60}}` should lie between 0.45 and 2.0, if :math:`\frac{N_c}{N_{60}}`
-            is greater than 2.0, :math:`N_c` should be divided by 2.0 to obtain the design value
-            used in finding the bearing capacity of the soil.
+    @round_
+    def spt_n_design(self) -> float:
+        """SPT N-design.
+
+        Raises
+        ------
+        StatisticError
+            Raised if ``spt_numbers`` is empty.
         """
+        try:
+            return min(self.spt_numbers)
+        except ValueError as e:
+            err_msg = "method requires at least one data point."
+            raise StatisticsError(err_msg) from e
+
+
+@dataclass
+class EnergyCorrection:
+    r"""SPT N-value standardized for field procedures.
+
+    On the basis of field observations, it appears reasonable to standardize
+    the field SPT N-value as a function of the input driving energy and its
+    dissipation around the sampler around the surrounding soil. The variations
+    in testing procedures may be at least partially compensated by converting
+    the measured N-value to :math:`N_{60}` assuming 60% hammer energy being
+    transferred to the tip of the standard split spoon.
+
+    Parameters
+    ----------
+    recorded_spt_number : int
+        Recorded SPT N-value from field.
+    energy_percentage : float, default=0.6
+        Energy percentage reaching the tip of the sampler.
+    hammer_efficiency : float, default=0.6
+        Hammer efficiency, defaults to 0.6
+    borehole_diameter_correction : float, default=1.0
+        Borehole diameter correction
+    sampler_correction : float, default=1.0
+        Sampler correction
+    rod_length_correction : float, default=0.75
+        Rod length correction
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Energy correction is given by the formula:
 
-        std_pressure = 280
+    .. math::
 
-        if eop <= 0 or eop > std_pressure:
-            err_msg = (
-                f"eop: {eop} should be less than or equal to {std_pressure}"
-                "but not less than or equal to 0"
-            )
-            raise OverburdenPressureError(err_msg)
+        N_{ENERGY} = \dfrac{E_H \cdot C_B \cdot C_S \cdot C_R \cdot N}{ENERGY}
 
-        corrected_spt = spt_n_60 * (350 / (eop + 70))
-        spt_ratio = corrected_spt / spt_n_60
+    ``ENERGY``: 0.6, 0.55, etc
 
-        if 0.45 < spt_ratio < 2.0:
-            return corrected_spt
+    Examples
+    --------
+    >>> from geolysis.core.spt import EnergyCorrection
+    >>> energy_cor = EnergyCorrection(recorded_spt_number=30)
+    >>> energy_cor.correction
+    0.75
+    >>> energy_cor.corrected_spt_number
+    22.5
+    """
 
-        corrected_spt = corrected_spt / 2 if spt_ratio > 2.0 else corrected_spt
-        return min(corrected_spt, 2 * spt_n_60)
+    recorded_spt_number: float
 
-    @staticmethod
-    @round_(ndigits=2)
-    def peck_et_al_opc_1974(spt_n_60: float, eop: float) -> float:
-        r"""
-        Return the overburden pressure given by ``Peck et al (1974)``.
+    _: KW_ONLY
 
-        :param float spt_n_60: SPT N-value standardized for field procedures.
-        :param float eop: Effective overburden pressure (:math:`kN/m^2`).
+    energy_percentage: float = 0.6
+    hammer_efficiency: float = 0.6
+    borehole_diameter_correction: float = 1.0
+    sampler_correction: float = 1.0
+    rod_length_correction: float = 0.75
+
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        return (
+            self.hammer_efficiency
+            * self.borehole_diameter_correction
+            * self.sampler_correction
+            * self.rod_length_correction
+        ) / self.energy_percentage
+
+    @property
+    @round_
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        return self.correction * self.recorded_spt_number
+
+
+@dataclass
+class GibbsHoltzOPC(_OPC):
+    r"""Overburden Pressure Correction according to ``Gibbs & Holtz (1957)``.
+
+    Parameters
+    ----------
+    std_spt_number : float
+        SPT N-value standardized for field procedures.
+    eop : float, :math:`kN/m^2`
+        Effective overburden pressure.
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Overburden Pressure Correction is given by the formula:
+
+    .. math:: C_N = \dfrac{350}{\sigma_o + 70} \, \sigma_o \le 280kN/m^2
+
+    :math:`\frac{N_c}{N_{60}}` should lie between 0.45 and 2.0, if
+    :math:`\frac{N_c}{N_{60}}` is greater than 2.0, :math:`N_c` should be
+    divided by 2.0 to obtain the design value used in finding the bearing
+    capacity of the soil.
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import GibbsHoltzOPC
+    >>> opc_cor = GibbsHoltzOPC(std_spt_number=22.5, eop=100.0)
+    >>> opc_cor.correction
+    2.0588
+    >>> opc_cor.corrected_spt_number
+    23.1615
+    """
 
-        .. math::
+    #: Maximum effective overburden pressure. |rarr| :math:`kN/m^2`
+    STD_PRESSURE = 280.0
 
-            C_N = 0.77 \log \left( \dfrac{2000}{\sigma_o} \right)
-        """
-        std_pressure = 24
+    def __init__(self, std_spt_number: float, eop: float) -> None:
+        self.std_spt_number = std_spt_number
+        self.eop = eop
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.std_spt_number=}, {self.eop=})"
+
+    @property
+    def eop(self) -> float:
+        return self._eop
+
+    @eop.setter
+    def eop(self, __val: float):
+        if __val <= 0:
+            err_msg = f"eop = {__val} cannot be less than or equal to 0"
+            raise OPCError(err_msg)
+
+        if __val > self.STD_PRESSURE:
+            err_msg = f"eop = {__val} should be less than {self.STD_PRESSURE}"
+            raise OPCError(err_msg)
+        self._eop = __val
+
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        return 350.0 / (self.eop + 70)
+
+    @property
+    @round_
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        corrected_spt = self.correction * self.std_spt_number
+        spt_ratio = corrected_spt / self.std_spt_number
+
+        if spt_ratio > 2.0:
+            corrected_spt /= 2
+
+        return min(corrected_spt, 2 * self.std_spt_number)
+
+
+@dataclass
+class BazaraaPeckOPC(_OPC):
+    r"""Overburden Pressure Correction according to ``Bazaraa (1967)``, and
+    also by ``Peck and Bazaraa (1969)``.
+
+    Parameters
+    ----------
+    std_spt_number : float
+        SPT N-value standardized for field procedures.
+    eop : float, :math:`kN/m^2`
+        Effective overburden pressure.
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Overburden Pressure Correction is given by the formula:
 
-        if eop <= 0 or eop < std_pressure:
-            err_msg = f"eop: {eop} >= {std_pressure}"
-            raise OverburdenPressureError(err_msg)
+    .. math::
 
-        corrected_spt = 0.77 * log10(2000 / eop) * spt_n_60
-        return min(corrected_spt, 2 * spt_n_60)
+        C_N &= \dfrac{4}{1 + 0.0418 \cdot \sigma_o}, \, \sigma_o \lt 71.8kN/m^2
 
-    @staticmethod
-    @round_(ndigits=2)
-    def liao_whitman_opc_1986(spt_n_60: float, eop: float) -> float:
-        r"""
-        Return the overburden pressure given by ``Liao Whitman (1986)``.
+        C_N &= \dfrac{4}{3.25 + 0.0104 \cdot \sigma_o}, \, \sigma_o \gt 71.8kN/m^2
 
-        :param float spt_n_60: SPT N-value standardized for field procedures.
-        :param float eop: Effective overburden pressure (:math:`kN/m^2`).
+        C_N &= 1 \, , \, \sigma_o = 71.8kN/m^2
 
-        .. math::
+    Examples
+    --------
+    >>> from geolysis.core.spt import BazaraaPeckOPC
+    >>> opc_cor = BazaraaPeckOPC(std_spt_number=22.5, eop=100.0)
+    >>> opc_cor.correction
+    0.9324
+    >>> opc_cor.corrected_spt_number
+    20.979
+    """
 
-            C_N = \sqrt{\dfrac{100}{\sigma_o}}
-        """
-        if eop <= 0:
-            err_msg = f"eop: {eop} > 0"
-            raise OverburdenPressureError(err_msg)
+    std_spt_number: float
+    eop: float
 
-        corrected_spt = sqrt(100 / eop) * spt_n_60
-        return min(corrected_spt, 2 * spt_n_60)
+    #: Maximum effective overburden pressure. |rarr| :math:`kN/m^2`
+    STD_PRESSURE = 71.8
 
-    @staticmethod
-    @round_(ndigits=2)
-    def skempton_opc_1986(spt_n_60: float, eop: float) -> float:
-        r"""
-        Return the overburden pressure correction given by ``Skempton (1986).``
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        if isclose(self.eop, self.STD_PRESSURE, rel_tol=ERROR_TOL):
+            correction = 1.0
+        elif self.eop < self.STD_PRESSURE:
+            correction = 4 / (1 + 0.0418 * self.eop)
+        else:
+            correction = 4 / (3.25 + 0.0104 * self.eop)
 
-        :param float spt_n_60: SPT N-value standardized for field procedures.
-        :param float eop: Effective overburden pressure (:math:`kN/m^2`).
+        return correction
 
-        .. math::
+    @property
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        return super().corrected_spt_number
+
+
+@dataclass
+class PeckOPC(_OPC):
+    r"""Overburden Pressure Correction according to ``Peck et al (1974)``.
+
+    Parameters
+    ----------
+    std_spt_number : float
+        SPT N-value standardized for field procedures.
+    eop : float, :math:`kN/m^2`
+        Effective overburden pressure.
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Overburden Pressure Correction is given by the formula:
+
+    .. math:: C_N = 0.77 \log \left( \dfrac{2000}{\sigma_o} \right)
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import PeckOPC
+    >>> opc_cor = PeckOPC(std_spt_number=22.5, eop=100.0)
+    >>> opc_cor.correction
+    1.0
+    >>> opc_cor.corrected_spt_number
+    22.5
+    """
 
-            C_N = \dfrac{2}{1 + 0.01044 \cdot \sigma_o}
-        """
-        corrected_spt = (2 / (1 + 0.01044 * eop)) * spt_n_60
-        return min(corrected_spt, 2 * spt_n_60)
+    #: Maximum effective overburden pressure. |rarr| :math:`kN/m^2`
+    STD_PRESSURE = 24.0
 
-    @staticmethod
-    @round_(ndigits=2)
-    def bazaraa_peck_opc_1969(spt_n_60: float, eop: float) -> float:
-        r"""
-        Return the overburden pressure correction given by ``Bazaraa (1967)``
-        and also by ``Peck and Bazaraa (1969)``.
+    def __init__(self, std_spt_number: float, eop: float) -> None:
+        self.std_spt_number = std_spt_number
+        self.eop = eop
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.std_spt_number=}, {self.eop=})"
+
+    @property
+    def eop(self) -> float:
+        return self._eop
+
+    @eop.setter
+    def eop(self, __val: float):
+        if __val < self.STD_PRESSURE:
+            err_msg = f"eop = {__val} cannot be less than 24"
+            raise OPCError(err_msg)
+        self._eop = __val
+
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        return 0.77 * log10(2000 / self.eop)
+
+    @property
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        return super().corrected_spt_number
+
+
+@dataclass
+class LiaoWhitmanOPC(_OPC):
+    r"""Overburden Pressure Correction according to ``Liao & Whitman (1986)``.
+
+    Parameters
+    ----------
+    std_spt_number : float
+        SPT N-value standardized for field procedures.
+    eop : float, :math:`kN/m^2`
+        Effective overburden pressure.
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Overburden Pressure Correction is given by the formula:
+
+    .. math:: C_N = \sqrt{\dfrac{100}{\sigma_o}}
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import LiaoWhitmanOPC
+    >>> opc_cor = LiaoWhitmanOPC(std_spt_number=22.5, eop=100.0)
+    >>> opc_cor.correction
+    1.0
+    >>> opc_cor.corrected_spt_number
+    22.5
+    """
 
-        :param float spt_n_60: SPT N-value standardized for field procedures.
-        :param float eop: Effective overburden pressure (:math:`kN/m^2`).
+    def __init__(self, std_spt_number: float, eop: float) -> None:
+        self.std_spt_number = std_spt_number
+        self.eop = eop
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.std_spt_number=}, {self.eop=})"
+
+    @property
+    def eop(self) -> float:
+        return self._eop
+
+    @eop.setter
+    def eop(self, __val: float):
+        if __val <= 0:
+            err_msg = f"eop = {__val} cannot be less than or equal to 0"
+            raise OPCError(err_msg)
+        self._eop = __val
+
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        return sqrt(100 / self.eop)
+
+    @property
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        return super().corrected_spt_number
+
+
+@dataclass
+class SkemptonOPC(_OPC):
+    r"""Overburden Pressure Correction according to ``Skempton (1986)``.
+
+    Parameters
+    ----------
+    std_spt_number : float
+        SPT N-value standardized for field procedures.
+    eop : float, :math:`kN/m^2`
+        Effective overburden pressure.
+
+    Attributes
+    ----------
+    correction : float
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Overburden Pressure Correction is given by the formula:
+
+    .. math:: C_N = \dfrac{2}{1 + 0.01044 \cdot \sigma_o}
+
+    Examples
+    --------
+    >>> from geolysis.core.spt import SkemptonOPC
+    >>> opc_cor = SkemptonOPC(std_spt_number=22.5, eop=100.0)
+    >>> opc_cor.correction
+    0.9785
+    >>> opc_cor.corrected_spt_number
+    22.0163
+    """
 
-        .. math::
+    std_spt_number: float
+    eop: float
 
-            C_N &= \dfrac{4}{1 + 0.0418 \cdot \sigma_o}, \, \sigma_o \lt 71.8kN/m^2
+    @property
+    @round_
+    def correction(self) -> float:
+        """SPT Correction."""
+        return 2 / (1 + 0.01044 * self.eop)
+
+    @property
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        return super().corrected_spt_number
+
+
+@dataclass
+class DilatancyCorrection:
+    r"""Dilatancy SPT Correction according to ``Terzaghi & Peck (1948)``.
+
+    For coarse sand, this correction is not required. In applying this
+    correction, overburden pressure correction is applied first and then
+    dilatancy correction is applied.
+
+    Parameters
+    ----------
+    spt_number : float
+        SPT N-value standardized for field procedures or corrected for
+        overburden pressure.
+
+    Attributes
+    ----------
+    corrected_spt_number : float
+
+    Notes
+    -----
+    Dilatancy correction is given by the formula:
 
-            C_N &= \dfrac{4}{3.25 + 0.0104 \cdot \sigma_o}, \, \sigma_o \gt 71.8kN/m^2
+    .. math::
 
-            C_N &= 1 \, , \, \sigma_o = 71.8kN/m^2
-        """
+        (N_1)_{60} &= 15 + \dfrac{1}{2}((N_1)_{60} - 15) \, , \,
+                      (N_1)_{60} \gt 15
 
-        std_pressure = 71.8
+        (N_1)_{60} &= (N_1)_{60} \, , \, (N_1)_{60} \le 15
 
-        if isclose(eop, std_pressure, rel_tol=ERROR_TOL):
-            return spt_n_60
+    Examples
+    --------
+    >>> from geolysis.core.spt import DilatancyCorrection
+    >>> dil_cor = DilatancyCorrection(spt_number=22.5)
+    >>> dil_cor.corrected_spt_number
+    18.75
+    """
 
-        if eop < std_pressure:
-            corrected_spt = 4 * spt_n_60 / (1 + 0.0418 * eop)
+    spt_number: float
 
-        else:
-            corrected_spt = 4 * spt_n_60 / (3.25 + 0.0104 * eop)
+    @property
+    @round_
+    def corrected_spt_number(self) -> float:
+        """Corrected SPT N-value."""
+        if self.spt_number <= 15:
+            return self.spt_number
 
-        return min(corrected_spt, 2 * spt_n_60)
+        return 15 + 0.5 * (self.spt_number - 15)
```

### Comparing `geolysis-0.2.0/geolysis.egg-info/PKG-INFO` & `geolysis-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,20 @@
 Metadata-Version: 2.1
 Name: geolysis
-Version: 0.2.0
-Summary: geolysis is an opensource software for geotechnical engineering analysis and modeling.
+Version: 0.3.0
+Summary: geolysis.core is an opensource software for geotechnical engineering analysis and modeling.
 Author-email: Patrick Boateng <boatengpato.pb@gmail.com>
-Maintainer-email: Patrick Boateng <boatengpato.pb@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2023 geolysis
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://github.com/patrickboateng/geolysis
 Project-URL: Repository, https://github.com/patrickboateng/geolysis
 Project-URL: Changelog, https://github.com/patrickboateng/geolysis/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/patrickboateng/geolysis/issues
 Project-URL: Discussions, https://github.com/patrickboateng/geolysis/discussions
 Keywords: discrete-element-method,geotechnical-engineering,soil-classification,settlement-analysis,bearing-capacity-analysis
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -48,146 +26,198 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
 
 [code_of_conduct_url]: https://github.com/patrickboateng/geolysis/blob/main/CODE_OF_CONDUCT.md/
 [contributing_url]: https://github.com/patrickboateng/geolysis/blob/main/docs/CONTRIBUTING.md#how-to-contribute
-[changelog_url]: https://github.com/patrickboateng/geolysis/blob/main/CHANGELOG.md
 [license_url]: https://github.com/patrickboateng/geolysis/blob/main/LICENSE.txt
 
-<h1 align="center">
-<img src="https://raw.githubusercontent.com/patrickboateng/geolysis/main/docs/source/_static/geolysis_logo.png" alt="logo" width="300">
-</h1><br>
+# geolysis
 
 <div align="center">
 
-[![GitHub Repo stars](https://img.shields.io/github/stars/patrickboateng/geolysis?style=flat&logo=github)](https://github.com/patrickboateng/geolysis/stargazers)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/geolysis?style=flat&logo=pypi)](https://pypi.org/project/geolysis/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/geolysis.svg?logo=python&style=flat)](https://pypi.python.org/pypi/geolysis/)
-[![GitHub last commit](https://img.shields.io/github/last-commit/patrickboateng/geolysis?logo=github&style=flat)](https://github.com/patrickboateng/geolysis/commits)
 [![license](https://img.shields.io/pypi/l/geolysis?style=flat&logo=opensourceinitiative)](https://opensource.org/license/mit/)
 
-#
-
 ![Coveralls Status](https://img.shields.io/coverallsCoverage/github/patrickboateng/geolysis?logo=coveralls)
-[![CI-Unit-Test](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml)
-[![CI-Build-Test](https://github.com/patrickboateng/geolysis/actions/workflows/build.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/build.yml)
+[![Unit-Tests](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/unit-tests.yml)
+[![Pkg Build](https://github.com/patrickboateng/geolysis/actions/workflows/pkg_build.yml/badge.svg)](https://github.com/patrickboateng/geolysis/actions/workflows/pkg_build.yml)
+[![Documentation Status](https://readthedocs.org/projects/geolysis/badge/?version=latest)](https://geolysis.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-## Project Links
+#
+
+`geolysis` is your one-stop shop for all your geotechnical engineering
+solutions, ranging from site investigation and laboratory test analysis
+to advanced geotechnical designs.
+
+`geolysis` is divided into four (4) main parts:
+
+1. `geolyis.core (Python Package)`
+
+   `geolysis.core` is an open-source Python package that provides features
+   for analyzing geotechnical results obtained from field and laboratory
+   tests. `geolysis.core` is designed specifically to assist developers
+   in building applications that can solve complex geotechnical
+   problems.
+
+   Whether you're working on soil mechanics, rock mechanics, or any other
+   geotechnical field, `geolysis.core` provides a powerful set of tools
+   that can help you design and develop robust solutions. With an
+   intuitive API and a wide range of features, this software is an
+   essential tool for anyone who needs to work with geotechnical data on
+   a regular basis. Whether you're a seasoned geotechnical engineer or a
+   new developer just getting started in the field, `geolysis.core` is
+   the ideal solution for all your software development needs.
+
+   Some of the features implemented so far include soil classification,
+   standard penetration test analysis (such as SPT N-design and SPT
+   N-value corrections), and calculating the allowable bearing capacity of
+   soils from Standard Penetration Test N-values. There are more features
+   underway, which include settlement analysis, ultimate bearing capacity
+   analysis, etc.
+
+   `geolysis.core` is the foundation application on which other parts of the
+   application will depend. Developers can also use `geolysis.core` to power
+   their applications.
+
+1. `geolysis.ui (Qt, PySide6)`
+
+   `geolysis.ui` is a Graphical User Interface (GUI) which will enable
+   users to graphically interact with `geolysis`. User will be able to
+   input data and view generated plots, such as `PSD` curves,
+   `Atterberg Limits` plots, `Compaction` curves, etc within the application.
+
+1. `geolysis.excel (Javascript & Others)`
+
+   `geolysis.excel` provides a Microsoft Excel add-in for simple geotechnical
+   analysis. _More on this later._
+
+1. `geolysis.ai (Python, Pytorch & Others)`
 
-<!-- - [Documentation](/docs) -->
+   `geolysis.ai` explores the use of Artificial Intelligence (**AI**) in
+   enhancing productivity in Geotechnical Engineering.
 
-- [Homepage](https://github.com/patrickboateng/geolysis)
+## Project Links
+
+- [Documentation](https://geolysis.readthedocs.org/en/latest)
+- [Repo](https://github.com/patrickboateng/geolysis)
 - [PyPi](https://pypi.org/project/geolysis/)
 - [Bug Reports](https://github.com/patrickboateng/geolysis/issues)
 - [Discussions](https://github.com/patrickboateng/geolysis/discussions)
 
-> [!IMPORTANT]
-> Project documentation is underway
+<!-- > [!IMPORTANT]
+> Project documentation is underway -->
 
 ## Table of Contents
 
-- [What is geolysis?](#what-is-geolysis)
+- [Motivation](#motivation)
 - [Installation](#installation)
-- [Soil Classification Example](#soil-classification-example)
-  - [AASHTO Classification](#aashto-classification)
-  - [USCS Classification](#uscs-classification)
+- [Getting Started](#getting-started)
+  - [Soil Classification Example](#soil-classification-example)
 - [Release History](#release-history)
 - [Code of Conduct](#code-of-conduct)
 - [Contributing](#contributing)
 - [License](#license)
+- [Governance of this project](#governance-of-this-project)
 - [Contact Information](#contact-information)
 
-## What is geolysis?
+## Motivation
 
-`geolysis` is an open-source software for geotechnical analysis and modeling.
-It provides features such as `soil classifications`
-(based on the USCS and AASHTO classification standards), `estimating soil
-bearing capacity` using SPT N-value, and `estimating of soil engineering parameters`
-such as `Soil Unit Weight` (moist, saturated, and submerged), `Compression index`,
-`soil internal angle of friction`, and `undrained shear strength of soil`.
-
-**Features to include in upcoming versions:**
-
-- Settlement analysis
-- Discrete element method (DEM)
-
-The motivation behind `geolysis` is to provide free software to assist
-geotechnical engineers in their day-to-day work and to expose civil
-engineering students (especially geotechnical students) to tools that
-can make them industry-ready geotechnical engineers right from college.
+`geolysis` is a software solution that aims to support geotechnical
+engineers in their daily work by providing a set of tools that makes
+them perform their tasks in a more efficient and effective manner.
+Moreover, the platform is designed to educate civil engineering
+students, especially those who specialize in geotechnical engineering,
+by exposing them to industry-relevant tools and techniques that will
+help them become industry-ready professionals as soon as they graduate.
+With `geolysis`, users will be better equipped to handle geotechnical
+challenges, make informed decisions, and improve their overall
+productivity.
 
 ## Installation
 
 ```shell
 pip install geolysis
 ```
 
-## Soil Classification Example
+## Getting Started
+
+### Soil Classification Example
 
-### AASHTO Classification
+AASHTO classification
 
 ```python
 
->>> from geolysis.soil_classifier import AASHTO
+>>> from geolysis.core.soil_classifier import AASHTO
 >>> aashto_cls = AASHTO(liquid_limit=30.2, plasticity_index=6.3, fines=11.18)
 >>> aashto_cls.soil_class
 'A-2-4(0)'
 >>> aashto_cls.soil_desc
 'Silty or clayey gravel and sand'
 
 ```
 
-### USCS Classification
+USCS Classification
 
 ```python
 
->>> from geolysis.soil_classifier import USCS
->>> uscs_cls = USCS(liquid_limit=34.1, plastic_limit=21.1, fines=47.88,
-...                 sand=37.84, gravel=14.8)
+>>> from geolysis.core.soil_classifier import USCS
+>>> uscs_cls = USCS(liquid_limit=34.1, plastic_limit=21.1,
+...                 fines=47.88, sand=37.84, gravel=14.8)
 >>> uscs_cls.soil_class
 'SC'
 >>> uscs_cls.soil_desc
 'Clayey sands'
 >>> uscs_cls = USCS(liquid_limit=30.8, plastic_limit=20.7, fines=10.29,
 ...                 sand=81.89, gravel=7.83, d_10=0.07, d_30=0.3, d_60=0.8)
 >>> uscs_cls.soil_class
 'SW-SC'
 >>> uscs_cls.soil_desc
 'Well graded sand with clay'
 
 ```
 
+<!-- See the [Quick start section] of the docs for more examples. -->
+
 ## Release History
 
-Check the [changelog][changelog_url] for release history.
+Check out the [release notes](https://geolysis.rtfd.io/en/latest/release_notes/index.html)
+for features.
 
 ## Code of Conduct
 
-This project has a [code of conduct][code_of_conduct_url] that we
-expect all contributors to adhere to. Please read and follow it
-when participating in this project.
+This project has a [code of conduct][code_of_conduct_url] that
+we expect all contributors to adhere to. Please read and follow
+it when participating in this project.
 
 ## Contributing
 
-If you would like to contribute to this project, please read the
-[contributing guidelines][contributing_url]
+If you would like to contribute to this project, please read
+the [contributing guidelines][contributing_url]
 
 ## License
 
 Distributed under the [**MIT**][license_url] license. By using,
 distributing, or contributing to this project, you agree to the
 terms and conditions of this license.
 
+## Governance of this project
+
+`geolysis.core` is still developing relatively rapidly, so please
+be patient if things change or features iterate and change quickly.
+Once `geolysis.core` hits `1.0.0`, it will slow down considerably.
+
 ## Contact Information
 
 - [**LinkedIn**](https://linkedin.com/in/patrickboateng/)
 
 > [!IMPORTANT]
 > For questions or comments about `geolysis`, please ask them in the
 > [discussions forum](https://github.com/patrickboateng/geolysis/discussions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geolysis-0.2.0/pyproject.toml` & `geolysis-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geolysis"
-description = "geolysis is an opensource software for geotechnical engineering analysis and modeling."
+description = "geolysis.core is an opensource software for geotechnical engineering analysis and modeling."
 readme = { file = "README.md", content-type = "text/markdown" }
-license = { file = "LICENSE.txt" }
+license = { text = "MIT License" }
 requires-python = ">=3.10"
 keywords = [
     "discrete-element-method",
     "geotechnical-engineering",
     "soil-classification",
     "settlement-analysis",
     "bearing-capacity-analysis",
 ]
 authors = [{ name = "Patrick Boateng", email = "boatengpato.pb@gmail.com" }]
-maintainers = [{ name = "Patrick Boateng", email = "boatengpato.pb@gmail.com" }]
 dependencies = []
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
@@ -47,20 +46,21 @@
 
 [tool.setuptools.packages.find]
 include = ["geolysis*"]
 exclude = ["tests*"]
 namespaces = false
 
 [project.optional-dependencies]
-dev = ["black", "pytest", "mypy", "pytest-cov"]
+dev = ["black", "pytest", "mypy", "pytest-cov", "coverage"]
 
 [tool.pytest.ini_options]
-addopts = "-ra --verbose --color=auto --code-highlight=yes --strict-markers"
+addopts = "-ra --verbose --strict-markers --doctest-modules"
 minversion = "6.0"
-testpaths = ["tests"]
+testpaths = ["tests", "geolysis"]
+doctest_optionflags = ["IGNORE_EXCEPTION_DETAIL", "NUMBER"]
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
 profile = "black"
 
@@ -68,31 +68,26 @@
 ignore_missing_imports = true
 
 [tool.docformatter]
 style = "sphinx"
 black = true
 wrap-summaries = 79
 wrap-descriptions = 79
-pre-summary-newline = true
-make-summary-multi-line = true
+pre-summary-newline = false
+make-summary-multi-line = false
 close-quotes-on-newline = true
 
 [tool.pydocstyle]
 # convention = "pep257"
 ignore = ["D107", "D200"]
 
-[tool.tox]
-legacy_tox_ini = """
-    [tox]
-    isolated_build = True
-    min_version = 4.0
-    env_list =
-        py310
-        py39
-
-    [testenv]
-    deps = 
-        pytest 
-        pytest-cov
+[tool.coverage.report]
+exclude_also = [
+    "def __repr__",
+    "class .*\\bProtocol\\):",
+    "@(abc\\.)?abstractmethod",
+]
+show_missing = true
+skip_covered = true
 
-    commands = pytest {posargs} tests
-"""
+[tool.coverage.run]
+branch = true
```

### Comparing `geolysis-0.2.0/tests/test_soil_classifier.py` & `geolysis-0.3.0/tests/test_soil_classifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,52 @@
+import unittest
 from typing import Sequence
 
 import pytest
 
-from geolysis.soil_classifier import AASHTO, PSD, USCS
-from geolysis.soil_classifier import AtterbergLimits as AL
-from geolysis.soil_classifier import PSDError
+from geolysis.core.soil_classifier import AASHTO, PSD, USCS
+from geolysis.core.soil_classifier import AtterbergLimits as AL
+from geolysis.core.soil_classifier import PSDAggSumError
 
 
-class TestAtterbergLimits:
-    @classmethod
-    def setup_class(cls):
-        cls.atterberg_limits = AL(liquid_limit=25, plastic_limit=15)
+class TestAL(unittest.TestCase):
+    def setUp(self) -> None:
+        self.atterberg_limits = AL(liquid_limit=25, plastic_limit=15)
 
-    def test_plasticity_index(self):
+    def testPlasticityIndex(self):
         plasticity_index = self.atterberg_limits.plasticity_index
-        assert plasticity_index == 10
+        self.assertAlmostEqual(plasticity_index, 10)
 
-    def test_liquidity_index(self):
+    def testLiquidityIndex(self):
         liquidity_index = self.atterberg_limits.liquidity_index(nmc=20)
-        assert liquidity_index == 50
+        self.assertAlmostEqual(liquidity_index, 50)
 
-    def test_consistency_index(self):
+    def testConsistencyIndex(self):
         consistency_index = self.atterberg_limits.consistency_index(nmc=20)
-        assert consistency_index == 50
+        self.assertAlmostEqual(consistency_index, 50)
 
 
-class TestParticleSizeDistribution:
-    @classmethod
-    def setup_class(cls):
-        cls.psd = PSD(
+class TestPSD(unittest.TestCase):
+    def setUp(self) -> None:
+        self.psd = PSD(
             fines=0, sand=0, gravel=100, d_10=0.115, d_30=0.53, d_60=1.55
         )
 
-    def test_coeff_of_uniformity(self):
-        assert self.psd.coeff_of_uniformity == 13.48
+    def testCoeffOfUniformity(self):
+        self.assertAlmostEqual(self.psd.coeff_of_uniformity, 13.4783)
 
-    def test_coeff_of_curvature(self):
-        assert self.psd.coeff_of_curvature == 1.58
+    def testCoeffOfCurvature(self):
+        self.assertAlmostEqual(self.psd.coeff_of_curvature, 1.5759)
 
-    def test_PSDError(self):
-        with pytest.raises(PSDError):
+    def testPSDError(self):
+        with self.assertRaises(PSDAggSumError):
             PSD(fines=30, sand=30, gravel=30)
 
 
-class TestAASHTOClassificationSystem:
+class TestAASHTO:
     @pytest.mark.parametrize(
         "soil_params,clf",
         [
             ((30, 5, 10), "A-1-a(0)"),
             ((17.9, 3.4, 24.01), "A-1-b(0)"),
             ((0, 0, 9.5), "A-3(0)"),
             ((30.2, 6.3, 11.18), "A-2-4(0)"),
@@ -76,15 +75,15 @@
     )
     def test_aashto_without_grp_idx(self, soil_params: Sequence, clf: str):
         asshto_classifier = AASHTO(*soil_params)
         asshto_classifier.add_group_idx = False
         assert asshto_classifier.soil_class == clf
 
 
-class TestUnifiedSoilClassificationSystem:
+class TestUSCS:
     @pytest.mark.parametrize(
         "al,psd,size_dist,clf",
         [
             ((30.8, 20.7), (10.29, 81.89, 7.83), (0.07, 0.3, 0.8), "SW-SC"),
             ((24.4, 14.7), (9.77, 44.82, 45.41), (0.06, 0.6, 7), "GP-GC"),
             ((49.5, 33.6), (6.93, 91.79, 1.28), (0.153, 0.4, 1.2), "SP-SM"),
             ((30.33, 23.42), (8.93, 7.69, 83.38), (0.15, 18, 44), "GP-GM"),
@@ -111,15 +110,15 @@
         [
             ((30.8, 20.7), (10.29, 81.89, 7.83), "SW-SC,SP-SC"),
             ((24.4, 14.7), (9.77, 44.82, 45.41), "GW-GC,GP-GC"),
             ((49.5, 33.6), (6.93, 91.79, 1.28), "SW-SM,SP-SM"),
             ((30.33, 23.42), (8.93, 7.69, 83.38), "GW-GM,GP-GM"),
             ((35.32, 25.57), (9.70, 5.63, 84.67), "GW-GM,GP-GM"),
             ((26.17, 19.69), (12.00, 8.24, 79.76), "GW-GC,GP-GC"),
-            ((32.78, 22.99), (3.87, 15.42, 80.71), "GW or GP"),
+            ((32.78, 22.99), (3.87, 15.42, 80.71), "GW,GP"),
         ],
     )
     def test_dual_classification_no_psd_coeff(
         self,
         al: Sequence,
         psd: Sequence,
         clf: str,
```

### Comparing `geolysis-0.2.0/tests/test_utils.py` & `geolysis-0.3.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pytest
 
-from geolysis.constants import ERROR_TOL
-from geolysis.utils import (
+from geolysis.core.constants import ERROR_TOL
+from geolysis.core.utils import (
     PI,
     cos,
     cot,
     deg2rad,
     log10,
     rad2deg,
-    round_,
     sin,
     sqrt,
     tan,
 )
 
 
 def test_deg2rad():
@@ -41,12 +40,7 @@
 
 def test_log():
     assert log10(10) == pytest.approx(1, ERROR_TOL)
 
 
 def test_sqrt():
     assert sqrt(25) == pytest.approx(5, ERROR_TOL)
-
-
-def test_round():
-    with pytest.raises(TypeError):
-        round_(ndigits=2.02)  # type: ignore
```

