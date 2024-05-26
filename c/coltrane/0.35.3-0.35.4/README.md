# Comparing `tmp/coltrane-0.35.3.tar.gz` & `tmp/coltrane-0.35.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coltrane-0.35.3.tar", max compression
+gzip compressed data, was "coltrane-0.35.4.tar", max compression
```

## Comparing `coltrane-0.35.3.tar` & `coltrane-0.35.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.3/LICENSE
--rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.3/README.md
--rw-r--r--   0        0        0    14551 2024-05-25 23:40:21.086949 coltrane-0.35.3/coltrane/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.3/coltrane/config/__init__.py
--rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.3/coltrane/config/cache.py
--rw-r--r--   0        0        0     2918 2024-05-24 12:44:28.808968 coltrane-0.35.3/coltrane/config/paths.py
--rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.3/coltrane/config/redirects.py
--rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.3/coltrane/config/settings.py
--rw-r--r--   0        0        0     5204 2024-05-24 12:48:22.833819 coltrane-0.35.3/coltrane/console.py
--rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.3/coltrane/context_processors.py
--rw-r--r--   0        0        0     1612 2024-05-25 14:38:06.294883 coltrane-0.35.3/coltrane/default-files/Dockerfile
--rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.3/coltrane/default-files/README.md
--rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.3/coltrane/default-files/app.py
--rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.3/coltrane/default-files/env
--rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.3/coltrane/default-files/gitignore
--rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.3/coltrane/default-files/gunicorn.conf.py
--rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.3/coltrane/default-files/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.3/coltrane/default-files/watchmanconfig
--rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.3/coltrane/feeds.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.3/coltrane/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.3/coltrane/management/commands/__init__.py
--rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.3/coltrane/management/commands/build.py
--rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.3/coltrane/manifest.py
--rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.3/coltrane/middleware.py
--rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.3/coltrane/module_finder.py
--rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.3/coltrane/renderer.py
--rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.3/coltrane/retriever.py
--rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.3/coltrane/sitemaps.py
--rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.3/coltrane/templates/coltrane/base.html
--rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.3/coltrane/templates/coltrane/content.html
--rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.3/coltrane/templatetags/__init__.py
--rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.3/coltrane/templatetags/coltrane_tags.py
--rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.3/coltrane/urls.py
--rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.3/coltrane/utils.py
--rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.3/coltrane/views.py
--rw-r--r--   0        0        0     5559 2024-05-25 23:44:44.488054 coltrane-0.35.3/pyproject.toml
--rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.4/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.4/README.md
+-rw-r--r--   0        0        0    15633 2024-05-26 02:50:53.616419 coltrane-0.35.4/coltrane/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.4/coltrane/config/__init__.py
+-rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.4/coltrane/config/cache.py
+-rw-r--r--   0        0        0     2918 2024-05-24 12:44:28.808968 coltrane-0.35.4/coltrane/config/paths.py
+-rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.4/coltrane/config/redirects.py
+-rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.4/coltrane/config/settings.py
+-rw-r--r--   0        0        0     5204 2024-05-24 12:48:22.833819 coltrane-0.35.4/coltrane/console.py
+-rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.4/coltrane/context_processors.py
+-rw-r--r--   0        0        0     1665 2024-05-26 02:38:33.589463 coltrane-0.35.4/coltrane/default-files/Dockerfile
+-rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.4/coltrane/default-files/README.md
+-rw-r--r--   0        0        0      166 2024-05-26 02:37:31.700420 coltrane-0.35.4/coltrane/default-files/app.py
+-rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.4/coltrane/default-files/env
+-rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.4/coltrane/default-files/gitignore
+-rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.4/coltrane/default-files/gunicorn.conf.py
+-rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.4/coltrane/default-files/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.4/coltrane/default-files/watchmanconfig
+-rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.4/coltrane/feeds.py
+-rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.4/coltrane/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.4/coltrane/management/commands/__init__.py
+-rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.4/coltrane/management/commands/build.py
+-rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.4/coltrane/manifest.py
+-rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.4/coltrane/middleware.py
+-rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.4/coltrane/module_finder.py
+-rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.4/coltrane/renderer.py
+-rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.4/coltrane/retriever.py
+-rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.4/coltrane/sitemaps.py
+-rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.4/coltrane/templates/coltrane/base.html
+-rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.4/coltrane/templates/coltrane/content.html
+-rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.4/coltrane/templatetags/__init__.py
+-rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.4/coltrane/templatetags/coltrane_tags.py
+-rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.4/coltrane/urls.py
+-rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.4/coltrane/utils.py
+-rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.4/coltrane/views.py
+-rw-r--r--   0        0        0     5559 2024-05-26 02:54:25.550124 coltrane-0.35.4/pyproject.toml
+-rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.4/PKG-INFO
```

### Comparing `coltrane-0.35.3/LICENSE` & `coltrane-0.35.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/README.md` & `coltrane-0.35.4/README.md`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/__init__.py` & `coltrane-0.35.4/coltrane/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
 import sys
+from contextlib import redirect_stdout
 from copy import deepcopy
+from io import StringIO
 from os import environ, getenv
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from django import setup as django_setup
 from django.conf import settings
 from django.core.handlers.wsgi import WSGIHandler
+from django.core.management import execute_from_command_line
 from django.template.library import InvalidTemplateLibrary, import_library
 from dotenv import load_dotenv
 
 from coltrane.config.settings import (
     DEFAULT_COLTRANE_SETTINGS,
 )
 from coltrane.module_finder import (
@@ -22,14 +25,15 @@
 )
 from coltrane.utils import dict_merge
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "initialize",
+    "run",
 ]
 
 
 DEFAULT_CACHES_SETTINGS = {
     "default": {
         "BACKEND": "django.core.cache.backends.dummy.DummyCache",
     }
@@ -58,14 +62,19 @@
 COLTRANE_SETTINGS_THAT_ARE_BOOLEANS = (
     "DISABLE_WILDCARD_TEMPLATES",
     "IS_SECURE",
     "DATA_JSON5",
 )
 
 
+def _get_current_command():
+    if len(sys.argv) > 1:
+        return sys.argv[1]
+
+
 def _get_base_dir(base_dir: Optional[Path]) -> Path:
     """
     Gets the base directory.
     """
 
     if base_dir is None:
         base_dir = Path("site")
@@ -282,15 +291,15 @@
     """
     Merges the passed-in settings into the default `coltrane` settings.
     Passed-in settings will override the defaults.
     """
 
     # Assume that `argv[1] == "build"` means that the `build`
     # management command is currently being run
-    is_build_management_command = len(sys.argv) >= 2 and sys.argv[1] == "build"  # noqa: PLR2004
+    is_build_management_command = _get_current_command() == "build"
 
     debug = django_settings.get("DEBUG", getenv("DEBUG", "True") == "True")
     time_zone = django_settings.get("TIME_ZONE", getenv("TIME_ZONE", "UTC"))
 
     staticfiles_dirs = [
         base_dir / "static",
     ]
@@ -376,15 +385,15 @@
             "django.contrib.staticfiles.finders.FileSystemFinder",
             "django.contrib.staticfiles.finders.AppDirectoriesFinder",
             "compressor.finders.CompressorFinder",
         )
 
         default_settings["TEMPLATES"][0]["OPTIONS"]["builtins"].append("compressor.templatetags.compress")
 
-        if len(sys.argv) > 1 and sys.argv[1] == "compress":
+        if _get_current_command() == "compress":
             default_settings["COMPRESS_OFFLINE"] = True
 
     # Make sure BASE_DIR is a `Path` if it got passed in
     if "BASE_DIR" in django_settings and isinstance(django_settings["BASE_DIR"], str):
         django_settings["BASE_DIR"] = Path(django_settings["BASE_DIR"])
 
     # Override STATIC_ROOT if the output directory is manually set
@@ -426,7 +435,35 @@
 
     django_settings = _merge_settings(base_dir, django_settings)
     _configure_settings(django_settings)
 
     django_setup()
 
     return WSGIHandler()
+
+
+def run() -> None:
+    """
+    Run the Django management command based on `argv`.
+    """
+
+    if _get_current_command() == "compress":
+        try:
+            from compressor.exceptions import OfflineGenerationError
+        except ImportError:
+            logger.error("django-compressor is not installed.")
+        else:
+            try:
+                stdout = StringIO()
+
+                with redirect_stdout(stdout):
+                    execute_from_command_line()
+
+                compress_stdout = stdout.getvalue().replace("Compressing... done\n", "")
+                print(compress_stdout)  # noqa: T201
+            except OfflineGenerationError as e:
+                if "No 'compress' template tags found in templates." in e.args[0]:
+                    logger.error("No compress blocks found.")
+                else:
+                    raise
+    else:
+        execute_from_command_line()
```

### Comparing `coltrane-0.35.3/coltrane/config/cache.py` & `coltrane-0.35.4/coltrane/config/cache.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/config/paths.py` & `coltrane-0.35.4/coltrane/config/paths.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/config/redirects.py` & `coltrane-0.35.4/coltrane/config/redirects.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/config/settings.py` & `coltrane-0.35.4/coltrane/config/settings.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/console.py` & `coltrane-0.35.4/coltrane/console.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/default-files/Dockerfile` & `coltrane-0.35.4/coltrane/default-files/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -42,9 +42,12 @@
 WORKDIR /site
 
 EXPOSE 80
 
 # Collect static assets
 RUN python app.py collectstatic -v 2 --noinput
 
+# Compress static assets
+RUN python app.py compress
+
 # Run gunicorn
 CMD ["gunicorn", "app:wsgi", "--config=gunicorn.conf.py"]
```

### Comparing `coltrane-0.35.3/coltrane/feeds.py` & `coltrane-0.35.4/coltrane/feeds.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/management/commands/build.py` & `coltrane-0.35.4/coltrane/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/manifest.py` & `coltrane-0.35.4/coltrane/manifest.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/middleware.py` & `coltrane-0.35.4/coltrane/middleware.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/module_finder.py` & `coltrane-0.35.4/coltrane/module_finder.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/renderer.py` & `coltrane-0.35.4/coltrane/renderer.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/retriever.py` & `coltrane-0.35.4/coltrane/retriever.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/templatetags/coltrane_tags.py` & `coltrane-0.35.4/coltrane/templatetags/coltrane_tags.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/urls.py` & `coltrane-0.35.4/coltrane/urls.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/utils.py` & `coltrane-0.35.4/coltrane/utils.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/coltrane/views.py` & `coltrane-0.35.4/coltrane/views.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.3/pyproject.toml` & `coltrane-0.35.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "coltrane"
 authors = [{name = "Adam Hill", email = "adam@adamghill.com"}]
 dynamic = ["version", "description"]
 
 [tool.poetry]
 name = "coltrane"
-version = "0.35.3"
+version = "0.35.4"
 description = "A minimal app framework for content sites 🎵"
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 packages = [{ include = "coltrane" }]
 repository = "https://github.com/adamghill/coltrane/"
```

### Comparing `coltrane-0.35.3/PKG-INFO` & `coltrane-0.35.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coltrane
-Version: 0.35.3
+Version: 0.35.4
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
-Metadata-Version: 2.1 Name: coltrane Version: 0.35.3 Summary: A minimal app
+Metadata-Version: 2.1 Name: coltrane Version: 0.35.4 Summary: A minimal app
 framework for content sites ðµ Home-page: https://github.com/adamghill/
 coltrane/ License: MIT Keywords: django,python,static,markdown Author:
 adamghill Author-email: adam@adamghill.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

