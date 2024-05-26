# Comparing `tmp/crondst-1.0.2.tar.gz` & `tmp/crondst-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crondst-1.0.2.tar", last modified: Sat Jan 13 02:41:32 2024, max compression
+gzip compressed data, was "crondst-1.0.3.tar", last modified: Sun May 26 01:00:16 2024, max compression
```

## Comparing `crondst-1.0.2.tar` & `crondst-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-01-13 02:41:32.490741 crondst-1.0.2/
--rw-r--r--   0 calvin     (501) staff       (20)     1072 2024-01-13 02:07:20.000000 crondst-1.0.2/LICENSE
--rw-r--r--   0 calvin     (501) staff       (20)     3256 2024-01-13 02:41:32.489430 crondst-1.0.2/PKG-INFO
--rw-r--r--   0 calvin     (501) staff       (20)     2620 2024-01-13 02:11:08.000000 crondst-1.0.2/README.md
-drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-01-13 02:41:32.488537 crondst-1.0.2/crondst.egg-info/
--rw-r--r--   0 calvin     (501) staff       (20)     3256 2024-01-13 02:41:32.000000 crondst-1.0.2/crondst.egg-info/PKG-INFO
--rw-r--r--   0 calvin     (501) staff       (20)      167 2024-01-13 02:41:32.000000 crondst-1.0.2/crondst.egg-info/SOURCES.txt
--rw-r--r--   0 calvin     (501) staff       (20)        1 2024-01-13 02:41:32.000000 crondst-1.0.2/crondst.egg-info/dependency_links.txt
--rw-r--r--   0 calvin     (501) staff       (20)        8 2024-01-13 02:41:32.000000 crondst-1.0.2/crondst.egg-info/top_level.txt
--rw-r--r--   0 calvin     (501) staff       (20)    15959 2024-01-13 01:41:17.000000 crondst-1.0.2/crondst.py
--rw-r--r--   0 calvin     (501) staff       (20)      788 2024-01-13 02:39:57.000000 crondst-1.0.2/pyproject.toml
--rw-r--r--   0 calvin     (501) staff       (20)       38 2024-01-13 02:41:32.490923 crondst-1.0.2/setup.cfg
+drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-05-26 01:00:16.844492 crondst-1.0.3/
+-rw-r--r--   0 calvin     (501) staff       (20)     1072 2024-01-13 03:21:42.000000 crondst-1.0.3/LICENSE
+-rw-r--r--   0 calvin     (501) staff       (20)     3348 2024-05-26 01:00:16.842693 crondst-1.0.3/PKG-INFO
+-rw-r--r--   0 calvin     (501) staff       (20)     2712 2024-05-25 23:05:52.000000 crondst-1.0.3/README.md
+drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-05-26 01:00:16.812936 crondst-1.0.3/crondst/
+-rw-r--r--   0 calvin     (501) staff       (20)    16003 2024-05-26 00:59:50.000000 crondst-1.0.3/crondst/__init__.py
+-rw-r--r--   0 calvin     (501) staff       (20)        0 2024-05-25 23:05:32.000000 crondst-1.0.3/crondst/py.typed
+drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-05-26 01:00:16.841333 crondst-1.0.3/crondst.egg-info/
+-rw-r--r--   0 calvin     (501) staff       (20)     3348 2024-05-26 01:00:16.000000 crondst-1.0.3/crondst.egg-info/PKG-INFO
+-rw-r--r--   0 calvin     (501) staff       (20)      215 2024-05-26 01:00:16.000000 crondst-1.0.3/crondst.egg-info/SOURCES.txt
+-rw-r--r--   0 calvin     (501) staff       (20)        1 2024-05-26 01:00:16.000000 crondst-1.0.3/crondst.egg-info/dependency_links.txt
+-rw-r--r--   0 calvin     (501) staff       (20)        8 2024-05-26 01:00:16.000000 crondst-1.0.3/crondst.egg-info/top_level.txt
+-rw-r--r--   0 calvin     (501) staff       (20)      832 2024-05-26 00:18:21.000000 crondst-1.0.3/pyproject.toml
+-rw-r--r--   0 calvin     (501) staff       (20)       38 2024-05-26 01:00:16.844689 crondst-1.0.3/setup.cfg
+drwxr-xr-x   0 calvin     (501) staff       (20)        0 2024-05-26 01:00:16.827411 crondst-1.0.3/tests/
+-rw-r--r--   0 calvin     (501) staff       (20)   132473 2024-05-25 23:01:13.000000 crondst-1.0.3/tests/test_crondst.py
```

### Comparing `crondst-1.0.2/LICENSE` & `crondst-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crondst-1.0.2/PKG-INFO` & `crondst-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crondst
-Version: 1.0.2
+Version: 1.0.3
 Summary: Returns when the next job triggers given a cron expression. Supports DST.
 Author: Calvin Law
 Maintainer: Calvin Law
 License: MIT
 Project-URL: Homepage, https://github.com/lawcal/crondst
 Keywords: cron,crontab,schedule
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CronDst
 
+[![Test](https://github.com/lawcal/crondst/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/lawcal/crondst/actions/workflows/test.yml)
+
 CronDst returns when the next job triggers given a cron expression. Supports time zones and daylight savings time (DST).
 
 Features:
 1. **Built according to [Vixie Cron](https://github.com/vixie/cron).** The popular cron scheduling logic that lives inside *nix systems like Debian, Ubuntu, RHEL and MacOS.
 2. **Lightweight.** Single file, zero dependencies.
 3. **Efficient.** Most expressions require just one constant-time step per iteration.
 
 ## Install
 `pip install crondst`
 
-Or simply copy the `crondst.py` file to your project directory.
-
 ## Usage
 ```
 from datetime import datetime
 from zoneinfo import ZoneInfo
 from crondst import CronDst
 
 # :00 and :01 at 2am and 3am in Pacific Time
```

### Comparing `crondst-1.0.2/README.md` & `crondst-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # CronDst
 
+[![Test](https://github.com/lawcal/crondst/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/lawcal/crondst/actions/workflows/test.yml)
+
 CronDst returns when the next job triggers given a cron expression. Supports time zones and daylight savings time (DST).
 
 Features:
 1. **Built according to [Vixie Cron](https://github.com/vixie/cron).** The popular cron scheduling logic that lives inside *nix systems like Debian, Ubuntu, RHEL and MacOS.
 2. **Lightweight.** Single file, zero dependencies.
 3. **Efficient.** Most expressions require just one constant-time step per iteration.
 
 ## Install
 `pip install crondst`
 
-Or simply copy the `crondst.py` file to your project directory.
-
 ## Usage
 ```
 from datetime import datetime
 from zoneinfo import ZoneInfo
 from crondst import CronDst
 
 # :00 and :01 at 2am and 3am in Pacific Time
```

### Comparing `crondst-1.0.2/crondst.egg-info/PKG-INFO` & `crondst-1.0.3/crondst.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crondst
-Version: 1.0.2
+Version: 1.0.3
 Summary: Returns when the next job triggers given a cron expression. Supports DST.
 Author: Calvin Law
 Maintainer: Calvin Law
 License: MIT
 Project-URL: Homepage, https://github.com/lawcal/crondst
 Keywords: cron,crontab,schedule
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CronDst
 
+[![Test](https://github.com/lawcal/crondst/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/lawcal/crondst/actions/workflows/test.yml)
+
 CronDst returns when the next job triggers given a cron expression. Supports time zones and daylight savings time (DST).
 
 Features:
 1. **Built according to [Vixie Cron](https://github.com/vixie/cron).** The popular cron scheduling logic that lives inside *nix systems like Debian, Ubuntu, RHEL and MacOS.
 2. **Lightweight.** Single file, zero dependencies.
 3. **Efficient.** Most expressions require just one constant-time step per iteration.
 
 ## Install
 `pip install crondst`
 
-Or simply copy the `crondst.py` file to your project directory.
-
 ## Usage
 ```
 from datetime import datetime
 from zoneinfo import ZoneInfo
 from crondst import CronDst
 
 # :00 and :01 at 2am and 3am in Pacific Time
```

### Comparing `crondst-1.0.2/crondst.py` & `crondst-1.0.3/crondst/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CronDst v1.0.2
+# CronDst v1.0.3
 
 # MIT License
 #
 # Copyright (c) 2023-2024 Calvin Law
 #
 # Permission is hereby granted, free of charge, to any person obtaining a
 # copy of this software and associated documentation files (the "Software"),
@@ -25,14 +25,16 @@
 from __future__ import annotations
 # from typing import Self # python >= 3.11
 
 from collections.abc import Generator
 import dataclasses as dc
 import datetime as dt
 
+__all__ = ['CronDst', 'CronDstError']
+
 class CronDstError(Exception):
     pass
 
 # internal structure
 # ********************
 
 MAX_EXPRESSION_LENGTH = 1000
@@ -324,15 +326,15 @@
         datetime.replace(microsecond=0, fold=0).timestamp() - datetime.replace(microsecond=0, fold=1).timestamp()
     )
 
 # public api
 # ********************
 
 class CronDst:
-    def __init__(self, expression):
+    def __init__(self, expression: str):
         self.entry = _CronEntry.from_expression(expression)
 
     def iter(
         self,
         start: dt.datetime | None = None,
         max_years_between_matches: int = MAX_YEARS_BETWEEN_MATCHES
     ) -> Generator[dt.datetime, None, None]:
```

### Comparing `crondst-1.0.2/pyproject.toml` & `crondst-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crondst"
-version = "1.0.2"
+version = "1.0.3"
 description = "Returns when the next job triggers given a cron expression. Supports DST."
 authors = [
     {name = "Calvin Law"}
 ]
 maintainers = [
     {name = "Calvin Law"}
 ]
@@ -24,8 +24,11 @@
 ]
 keywords = ["cron", "crontab", "schedule"]
 
 [project.urls]
 Homepage = "https://github.com/lawcal/crondst"
 
 [tool.setuptools]
-py-modules = ["crondst"]
+packages = ["crondst"]
+
+[tool.pytest.ini_options]
+pythonpath = ["."]
```

