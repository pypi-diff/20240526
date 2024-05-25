# Comparing `tmp/coltrane-0.35.1.tar.gz` & `tmp/coltrane-0.35.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coltrane-0.35.1.tar", max compression
+gzip compressed data, was "coltrane-0.35.2.tar", max compression
```

## Comparing `coltrane-0.35.1.tar` & `coltrane-0.35.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.1/LICENSE
--rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.1/README.md
--rw-r--r--   0        0        0    14466 2024-05-24 12:44:20.769647 coltrane-0.35.1/coltrane/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.1/coltrane/config/__init__.py
--rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.1/coltrane/config/cache.py
--rw-r--r--   0        0        0     2918 2024-05-24 12:44:28.808968 coltrane-0.35.1/coltrane/config/paths.py
--rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.1/coltrane/config/redirects.py
--rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.1/coltrane/config/settings.py
--rw-r--r--   0        0        0     5204 2024-05-24 12:48:22.833819 coltrane-0.35.1/coltrane/console.py
--rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.1/coltrane/context_processors.py
--rw-r--r--   0        0        0     1612 2024-05-25 14:38:06.294883 coltrane-0.35.1/coltrane/default-files/Dockerfile
--rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.1/coltrane/default-files/README.md
--rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.1/coltrane/default-files/app.py
--rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.1/coltrane/default-files/env
--rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.1/coltrane/default-files/gitignore
--rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.1/coltrane/default-files/gunicorn.conf.py
--rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.1/coltrane/default-files/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.1/coltrane/default-files/watchmanconfig
--rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.1/coltrane/feeds.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.1/coltrane/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.1/coltrane/management/commands/__init__.py
--rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.1/coltrane/management/commands/build.py
--rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.1/coltrane/manifest.py
--rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.1/coltrane/middleware.py
--rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.1/coltrane/module_finder.py
--rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.1/coltrane/renderer.py
--rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.1/coltrane/retriever.py
--rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.1/coltrane/sitemaps.py
--rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.1/coltrane/templates/coltrane/base.html
--rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.1/coltrane/templates/coltrane/content.html
--rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.1/coltrane/templatetags/__init__.py
--rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.1/coltrane/templatetags/coltrane_tags.py
--rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.1/coltrane/urls.py
--rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.1/coltrane/utils.py
--rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.1/coltrane/views.py
--rw-r--r--   0        0        0     5559 2024-05-25 14:39:09.446568 coltrane-0.35.1/pyproject.toml
--rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.2/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.2/README.md
+-rw-r--r--   0        0        0    14434 2024-05-25 14:47:51.348246 coltrane-0.35.2/coltrane/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.2/coltrane/config/__init__.py
+-rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.2/coltrane/config/cache.py
+-rw-r--r--   0        0        0     2918 2024-05-24 12:44:28.808968 coltrane-0.35.2/coltrane/config/paths.py
+-rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.2/coltrane/config/redirects.py
+-rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.2/coltrane/config/settings.py
+-rw-r--r--   0        0        0     5204 2024-05-24 12:48:22.833819 coltrane-0.35.2/coltrane/console.py
+-rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.2/coltrane/context_processors.py
+-rw-r--r--   0        0        0     1612 2024-05-25 14:38:06.294883 coltrane-0.35.2/coltrane/default-files/Dockerfile
+-rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.2/coltrane/default-files/README.md
+-rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.2/coltrane/default-files/app.py
+-rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.2/coltrane/default-files/env
+-rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.2/coltrane/default-files/gitignore
+-rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.2/coltrane/default-files/gunicorn.conf.py
+-rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.2/coltrane/default-files/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.2/coltrane/default-files/watchmanconfig
+-rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.2/coltrane/feeds.py
+-rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.2/coltrane/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.2/coltrane/management/commands/__init__.py
+-rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.2/coltrane/management/commands/build.py
+-rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.2/coltrane/manifest.py
+-rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.2/coltrane/middleware.py
+-rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.2/coltrane/module_finder.py
+-rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.2/coltrane/renderer.py
+-rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.2/coltrane/retriever.py
+-rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.2/coltrane/sitemaps.py
+-rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.2/coltrane/templates/coltrane/base.html
+-rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.2/coltrane/templates/coltrane/content.html
+-rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.2/coltrane/templatetags/__init__.py
+-rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.2/coltrane/templatetags/coltrane_tags.py
+-rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.2/coltrane/urls.py
+-rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.2/coltrane/utils.py
+-rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.2/coltrane/views.py
+-rw-r--r--   0        0        0     5559 2024-05-25 17:57:25.226179 coltrane-0.35.2/pyproject.toml
+-rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.2/PKG-INFO
```

### Comparing `coltrane-0.35.1/LICENSE` & `coltrane-0.35.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/README.md` & `coltrane-0.35.2/README.md`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/__init__.py` & `coltrane-0.35.2/coltrane/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import sys
 from copy import deepcopy
-from os import getenv
+from os import environ, getenv
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from django import setup as django_setup
 from django.conf import settings
 from django.core.handlers.wsgi import WSGIHandler
 from django.template.library import InvalidTemplateLibrary, import_library
-from dotenv.main import DotEnv
+from dotenv import load_dotenv
 
 from coltrane.config.settings import (
     DEFAULT_COLTRANE_SETTINGS,
 )
 from coltrane.module_finder import (
     is_django_compressor_installed,
     is_django_unicorn_installed,
@@ -401,21 +401,20 @@
     Configures the settings in Django.
     """
 
     settings.configure(**django_settings)
 
 
 def _load_environment_variables(base_dir: Path, django_settings: Dict[str, Any]) -> None:
-    dot_env = DotEnv(base_dir / ".env")
-    dot_env.set_as_environment_variables()
+    load_dotenv(base_dir / ".env")
 
     if "ENV" not in django_settings:
         django_settings["ENV"] = {}
 
-    django_settings["ENV"].update(dot_env.dict())
+    django_settings["ENV"].update(dict(environ.items()))
 
 
 def initialize(**django_settings) -> WSGIHandler:
     """
     Initializes the Django static site.
     """
```

### Comparing `coltrane-0.35.1/coltrane/config/cache.py` & `coltrane-0.35.2/coltrane/config/cache.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/config/paths.py` & `coltrane-0.35.2/coltrane/config/paths.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/config/redirects.py` & `coltrane-0.35.2/coltrane/config/redirects.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/config/settings.py` & `coltrane-0.35.2/coltrane/config/settings.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/console.py` & `coltrane-0.35.2/coltrane/console.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/default-files/Dockerfile` & `coltrane-0.35.2/coltrane/default-files/Dockerfile`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/feeds.py` & `coltrane-0.35.2/coltrane/feeds.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/management/commands/build.py` & `coltrane-0.35.2/coltrane/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/manifest.py` & `coltrane-0.35.2/coltrane/manifest.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/middleware.py` & `coltrane-0.35.2/coltrane/middleware.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/module_finder.py` & `coltrane-0.35.2/coltrane/module_finder.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/renderer.py` & `coltrane-0.35.2/coltrane/renderer.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/retriever.py` & `coltrane-0.35.2/coltrane/retriever.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/templatetags/coltrane_tags.py` & `coltrane-0.35.2/coltrane/templatetags/coltrane_tags.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/urls.py` & `coltrane-0.35.2/coltrane/urls.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/utils.py` & `coltrane-0.35.2/coltrane/utils.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/coltrane/views.py` & `coltrane-0.35.2/coltrane/views.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.1/pyproject.toml` & `coltrane-0.35.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "coltrane"
 authors = [{name = "Adam Hill", email = "adam@adamghill.com"}]
 dynamic = ["version", "description"]
 
 [tool.poetry]
 name = "coltrane"
-version = "0.35.1"
+version = "0.35.2"
 description = "A minimal app framework for content sites 🎵"
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 packages = [{ include = "coltrane" }]
 repository = "https://github.com/adamghill/coltrane/"
```

### Comparing `coltrane-0.35.1/PKG-INFO` & `coltrane-0.35.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coltrane
-Version: 0.35.1
+Version: 0.35.2
 Summary: A minimal app framework for content sites 🎵
 Home-page: https://github.com/adamghill/coltrane/
 License: MIT
 Keywords: django,python,static,markdown
 Author: adamghill
 Author-email: adam@adamghill.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coltrane Version: 0.35.1 Summary: A minimal app
+Metadata-Version: 2.1 Name: coltrane Version: 0.35.2 Summary: A minimal app
 framework for content sites ðµ Home-page: https://github.com/adamghill/
 coltrane/ License: MIT Keywords: django,python,static,markdown Author:
 adamghill Author-email: adam@adamghill.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

