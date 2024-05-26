# Comparing `tmp/dlt_init_openapi-0.1.0a1.tar.gz` & `tmp/dlt_init_openapi-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt_init_openapi-0.1.0a1.tar", max compression
+gzip compressed data, was "dlt_init_openapi-0.1.0a2.tar", max compression
```

## Comparing `dlt_init_openapi-0.1.0a1.tar` & `dlt_init_openapi-0.1.0a2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1853 2024-05-23 15:59:04.679770 dlt_init_openapi-0.1.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     1111 2024-05-21 08:48:46.382581 dlt_init_openapi-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     7174 2024-05-23 15:54:53.847387 dlt_init_openapi-0.1.0a1/README.md
--rw-r--r--   0        0        0     4763 2024-05-23 15:54:53.848070 dlt_init_openapi-0.1.0a1/dlt_init_openapi/__init__.py
--rw-r--r--   0        0        0       28 2024-05-21 10:48:17.311493 dlt_init_openapi-0.1.0a1/dlt_init_openapi/__main__.py
--rw-r--r--   0        0        0     4861 2024-05-23 15:54:53.848632 dlt_init_openapi-0.1.0a1/dlt_init_openapi/cli/__init__.py
--rw-r--r--   0        0        0     1197 2024-05-23 15:54:53.849095 dlt_init_openapi-0.1.0a1/dlt_init_openapi/cli/cli_endpoint_selection.py
--rw-r--r--   0        0        0     3445 2024-05-23 15:54:53.850145 dlt_init_openapi-0.1.0a1/dlt_init_openapi/config.py
--rw-r--r--   0        0        0       29 2024-05-21 10:48:17.312788 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/__init__.py
--rw-r--r--   0        0        0      664 2024-05-21 10:48:17.312992 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/base_detector.py
--rw-r--r--   0        0        0    22415 2024-05-23 15:54:53.850824 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/__init__.py
--rw-r--r--   0        0        0     1065 2024-05-23 15:54:53.851684 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/const.py
--rw-r--r--   0        0        0     1774 2024-05-21 10:48:17.313932 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/primary_key.py
--rw-r--r--   0        0        0      686 2024-05-21 10:48:17.314162 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/utils.py
--rw-r--r--   0        0        0     1573 2024-05-21 10:48:17.314794 dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/warnings.py
--rw-r--r--   0        0        0     1903 2024-05-23 15:54:53.852261 dlt_init_openapi-0.1.0a1/dlt_init_openapi/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.315259 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/__init__.py
--rw-r--r--   0        0        0       57 2024-05-21 10:48:17.315501 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/config.py
--rw-r--r--   0        0        0       44 2024-05-21 10:48:17.315659 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/const.py
--rw-r--r--   0        0        0     2839 2024-05-21 10:48:17.315866 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/context.py
--rw-r--r--   0        0        0    10286 2024-05-23 15:54:53.852948 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/endpoints.py
--rw-r--r--   0        0        0     1376 2024-05-21 10:48:17.316256 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/errors.py
--rw-r--r--   0        0        0      704 2024-05-21 10:48:17.316445 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/info.py
--rw-r--r--   0        0        0    12896 2024-05-21 10:48:17.316840 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/models.py
--rw-r--r--   0        0        0     4112 2024-05-23 15:54:53.853568 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/openapi_parser.py
--rw-r--r--   0        0        0      670 2024-05-21 10:48:17.317716 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/pagination.py
--rw-r--r--   0        0        0     2766 2024-05-21 10:48:17.318056 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/parameters.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.318258 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/properties/__init__.py
--rw-r--r--   0        0        0     2365 2024-05-21 10:48:17.318463 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/properties/converter.py
--rw-r--r--   0        0        0      562 2024-05-23 09:23:18.941182 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/security.py
--rw-r--r--   0        0        0     2360 2024-05-21 10:48:17.318971 dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/types.py
--rw-r--r--   0        0        0       26 2024-05-21 10:48:17.319147 dlt_init_openapi-0.1.0a1/dlt_init_openapi/py.typed
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.319244 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/__init__.py
--rw-r--r--   0        0        0      516 2024-05-21 10:48:17.319570 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/base_renderer.py
--rw-r--r--   0        0        0     6155 2024-05-23 15:54:53.854060 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/__init__.py
--rw-r--r--   0        0        0      932 2024-05-23 15:54:53.854540 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/README.md.j2
--rw-r--r--   0        0        0      519 2024-05-22 10:51:36.172746 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
--rw-r--r--   0        0        0      279 2024-05-23 09:23:18.942359 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
--rw-r--r--   0        0        0       62 2024-05-23 09:23:18.942598 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/gitignore.j2
--rw-r--r--   0        0        0      479 2024-05-22 10:51:36.173291 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
--rw-r--r--   0        0        0       11 2024-05-21 10:48:17.321138 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
--rw-r--r--   0        0        0     3939 2024-05-23 15:54:53.855165 dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/source.py.j2
--rw-r--r--   0        0        0      199 2024-05-21 10:48:17.321712 dlt_init_openapi-0.1.0a1/dlt_init_openapi/typing.py
--rw-r--r--   0        0        0        0 2024-05-21 10:48:17.321833 dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/__init__.py
--rw-r--r--   0        0        0     4137 2024-05-22 10:51:36.173648 dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/misc.py
--rw-r--r--   0        0        0     3851 2024-05-21 10:48:17.322279 dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/paths.py
--rw-r--r--   0        0        0     1167 2024-05-23 09:23:18.943730 dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/update_rest_api.py
--rw-r--r--   0        0        0     2539 2024-05-23 15:55:08.136996 dlt_init_openapi-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     8765 1970-01-01 00:00:00.000000 dlt_init_openapi-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     2109 2024-05-26 19:54:27.713247 dlt_init_openapi-0.1.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0     1111 2024-05-10 11:31:42.794290 dlt_init_openapi-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     9996 2024-05-26 19:52:35.277719 dlt_init_openapi-0.1.0a2/README.md
+-rw-r--r--   0        0        0     4763 2024-05-24 15:05:07.637826 dlt_init_openapi-0.1.0a2/dlt_init_openapi/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-23 04:47:13.947847 dlt_init_openapi-0.1.0a2/dlt_init_openapi/__main__.py
+-rw-r--r--   0        0        0     4985 2024-05-26 18:27:39.544319 dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/__init__.py
+-rw-r--r--   0        0        0     1197 2024-05-24 15:05:07.638151 dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/cli_endpoint_selection.py
+-rw-r--r--   0        0        0     3611 2024-05-26 19:52:35.278119 dlt_init_openapi-0.1.0a2/dlt_init_openapi/config.py
+-rw-r--r--   0        0        0       29 2024-05-23 04:47:13.948156 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-23 04:47:13.948219 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/base_detector.py
+-rw-r--r--   0        0        0    22415 2024-05-24 15:05:07.638768 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/__init__.py
+-rw-r--r--   0        0        0     1065 2024-05-24 15:05:07.639104 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/const.py
+-rw-r--r--   0        0        0     1774 2024-05-23 04:47:13.948547 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/primary_key.py
+-rw-r--r--   0        0        0      686 2024-05-23 04:47:13.948609 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/utils.py
+-rw-r--r--   0        0        0     1573 2024-05-23 04:47:13.948668 dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/warnings.py
+-rw-r--r--   0        0        0     1903 2024-05-24 15:05:07.639228 dlt_init_openapi-0.1.0a2/dlt_init_openapi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.948783 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-23 04:47:13.948849 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/config.py
+-rw-r--r--   0        0        0       44 2024-05-23 04:47:13.948951 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/const.py
+-rw-r--r--   0        0        0     2839 2024-05-23 04:47:13.949026 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/context.py
+-rw-r--r--   0        0        0    10764 2024-05-26 19:52:35.278592 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/endpoints.py
+-rw-r--r--   0        0        0     1376 2024-05-23 04:47:13.949244 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/errors.py
+-rw-r--r--   0        0        0      704 2024-05-23 04:47:13.949307 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/info.py
+-rw-r--r--   0        0        0    12896 2024-05-23 04:47:13.949454 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/models.py
+-rw-r--r--   0        0        0     4112 2024-05-24 15:05:07.639975 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/openapi_parser.py
+-rw-r--r--   0        0        0      670 2024-05-23 04:47:13.949606 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/pagination.py
+-rw-r--r--   0        0        0     2766 2024-05-23 04:47:13.949686 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/parameters.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.949744 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-23 04:47:13.949854 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/converter.py
+-rw-r--r--   0        0        0      562 2024-05-23 07:11:02.288112 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/security.py
+-rw-r--r--   0        0        0     2360 2024-05-23 04:47:13.950009 dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/types.py
+-rw-r--r--   0        0        0       26 2024-05-23 04:47:13.950067 dlt_init_openapi-0.1.0a2/dlt_init_openapi/py.typed
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950094 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-23 04:47:13.950163 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/base_renderer.py
+-rw-r--r--   0        0        0     6155 2024-05-24 15:05:07.640152 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/__init__.py
+-rw-r--r--   0        0        0      932 2024-05-24 15:05:07.640271 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/README.md.j2
+-rw-r--r--   0        0        0      519 2024-05-23 05:53:21.142183 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2
+-rw-r--r--   0        0        0      279 2024-05-23 07:43:30.108700 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_secrets.toml.j2
+-rw-r--r--   0        0        0       62 2024-05-23 07:43:30.108831 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/gitignore.j2
+-rw-r--r--   0        0        0      479 2024-05-23 05:53:21.142413 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/pipeline.py.j2
+-rw-r--r--   0        0        0       11 2024-05-23 04:47:13.950645 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/requirements.txt.j2
+-rw-r--r--   0        0        0     4301 2024-05-26 19:52:35.278941 dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/source.py.j2
+-rw-r--r--   0        0        0      199 2024-05-23 04:47:13.950759 dlt_init_openapi-0.1.0a2/dlt_init_openapi/typing.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:47:13.950790 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-23 05:53:21.142935 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/misc.py
+-rw-r--r--   0        0        0     3851 2024-05-23 04:47:13.950988 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/paths.py
+-rw-r--r--   0        0        0     1167 2024-05-23 07:11:02.288801 dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/update_rest_api.py
+-rw-r--r--   0        0        0     2539 2024-05-26 19:53:13.689616 dlt_init_openapi-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0    11587 1970-01-01 00:00:00.000000 dlt_init_openapi-0.1.0a2/PKG-INFO
```

### Comparing `dlt_init_openapi-0.1.0a1/CHANGELOG.md` & `dlt_init_openapi-0.1.0a2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 [Go to GitHub Releases](https://github.com/dlt-hub/dlt-init-openapi/releases)
 
+0.1.0a2 - Getting ready for the first release
+* Updated Readme, reordered content blocks and made example nicer
+* Better rendering of required and non-required query args
+* Do not ask wether output directory should be written when in non-interactive mode
+
 0.1.0a1 - Getting ready for the first release
 * Remove init command from CLI. The same functionality is now the default command, see updated README file.
 * Add better error messages for broken and incompatible specs
 * Add a basic contributing page
 * Improve endpoint selector message and select all endpoints if nothing is selected by the user
 * Add endpoint descriptions as comments to the rendered source
 * Fixes in paginator detection
```

### Comparing `dlt_init_openapi-0.1.0a1/LICENSE` & `dlt_init_openapi-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/__init__.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/cli/__init__.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         raise typer.Exit(code=1)
     if url and path:
         typer.secho("Provide either --url or --path, not both", fg=typer.colors.RED)
         raise typer.Exit(code=1)
 
     try:
 
-        # synch rest api
+        # sync rest api
         update_rest_api.update_rest_api(force=update_rest_api_source)
 
         config = _load_config(
             path=config_path,
             config={
                 "project_name": source,
                 "package_name": source,
@@ -113,15 +113,17 @@
                 "spec_url": url,
                 "spec_path": path,
                 "allow_openapi_2": allow_openapi_2,
             },
         )
 
         if config.project_dir.exists():
-            if not questionary.confirm(
+            if not interactive:
+                logger.info("Non interactive mode selected, overwriting existing source.")
+            elif not questionary.confirm(
                 f"Directory {config.project_dir} exists, do you want to continue and update the generated files? "
                 + "This will overwrite your changes in those files."
             ).ask():
                 logger.warning("Exiting...")
                 exit(0)
 
         create_new_client(
```

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/cli/cli_endpoint_selection.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/cli/cli_endpoint_selection.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/config.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,16 +45,18 @@
     """always name resources by operation id, useful for testing"""
     renderer_class: str = "dlt_init_openapi.renderer.default.DefaultRenderer"
     """Which class to use for rendering"""
     detector_class: str = "dlt_init_openapi.detector.default.DefaultDetector"
     """Which class to use for detecting"""
     global_limit: int = 0
     """Set a limit on how many items are emitted from a resource"""
-    parameter_default_value: str = "FILL_ME_IN"
+    required_parameter_default_value: str = "FILL_ME_IN"
     """default to render for required parameters that do not have a default in the spec"""
+    unrequired_parameter_default_value: str = "OPTIONAL_CONFIG"
+    """default to render for unrequired parameters that do not have a default in the spec"""
     allow_openapi_2: bool = False
     """Allow to use OpenAPI 2 specs"""
 
     # internal, do not set via config file
     project_dir: Path = None
     pipeline_file_name: str = None
     spec_url: str = None
```

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/base_detector.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/base_detector.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/__init__.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/const.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/const.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/primary_key.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/primary_key.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/utils.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/utils.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/detector/default/warnings.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/detector/default/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/exceptions.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/context.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/context.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/endpoints.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,35 +119,44 @@
     def unresolvable_path_param_names(self) -> List[str]:
         """returns a list of path param names with params that are resolvable via the parent excluded"""
         params = get_path_var_names(self.path)
         transformer_param = self.transformer.path_parameter_name if self.transformer else None
         return [p for p in params if p != transformer_param]
 
     @property
-    def unresolvable_query_param_names(self) -> List[str]:
+    def unresolvable_query_params(self) -> List[Parameter]:
         """returns a list of required query param names with params that are used by the paginator excluded"""
+        print("HERE")
         paginator_params = self.detected_pagination.param_names if self.detected_pagination else []
-        query_param_names = []
+        query_params: List[Parameter] = []
         for param in self.list_all_parameters:
             if param.name not in paginator_params and param.location == "query":
-                query_param_names.append(param.name)
-        return query_param_names
+                query_params.append(param)
+        return query_params
 
-    def is_query_param_required(self, param_name: str) -> bool:
-        for key, p in self.parameters.items():
-            if p.name == param_name and p.location == "query":
-                return p.required
-        return False
+    @property
+    def unresolvable_required_query_param_names(self) -> List[str]:
+        """returns a list of required query param names with params that are used by the paginator excluded"""
+        return [param.name for param in self.unresolvable_query_params if param.required]
+
+    @property
+    def unresolvable_unrequired_query_param_names(self) -> List[str]:
+        return [param.name for param in self.unresolvable_query_params if not param.required]
 
     def default_for_param(self, location: Literal["path", "query"], param_name: str) -> str:
         """get's a default value for the given param, returns"""
+        param: Parameter = None
         for key, p in self.parameters.items():
-            if p.name == param_name and p.location == location and p.default:
-                return p.default
-        return self.context.config.parameter_default_value
+            if p.name == param_name and p.location == location:
+                param = p
+        if param and param.default:
+            return param.default
+        if not param or param.required or location == "path":
+            return self.context.config.required_parameter_default_value
+        return self.context.config.unrequired_parameter_default_value
 
     @property
     def render_description(self) -> Optional[str]:
         description = self.description or self.path_description
         if not description:
             return None
         return description.replace("\n", " ")
```

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/errors.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/errors.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/info.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/info.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/models.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/models.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/openapi_parser.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/openapi_parser.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/pagination.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/pagination.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/parameters.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/parameters.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/properties/converter.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/properties/converter.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/security.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/security.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/parser/types.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/parser/types.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/base_renderer.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/base_renderer.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/__init__.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/README.md.j2` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/dlt_config.toml.j2`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/renderer/default/templates/source.py.j2` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/renderer/default/templates/source.py.j2`

 * *Files 7% similar despite different names*

```diff
@@ -56,31 +56,38 @@
             {% endif %}
             {% endif %}
             "endpoint": {
                 {% if endpoint.data_json_path %}
                 "data_selector": "{{ endpoint.data_json_path }}",
                 {% endif %}
                 "path": "{{endpoint.path }}",
-                {% if endpoint.transformer or endpoint.unresolvable_path_param_names or endpoint.unresolvable_query_param_names %}
+                {% if endpoint.transformer or endpoint.unresolvable_path_param_names or endpoint.unresolvable_query_params %}
                 "params": {
                     {% if endpoint.transformer %}
                     {% for key, value in endpoint.transformer.path_params_mapping.items()%}
                     "{{key}}": {
                         "type": "resolve",
                         "resource": "{{endpoint.parent.detected_resource_name }}",
                         "field": "{{value}}",
                     },
                     {% endfor %}
                     {% endif %}
                     {% for param_name in endpoint.unresolvable_path_param_names %}
-                    "{{param_name}}": "{{ endpoint.default_for_param('path', param_name) }}", # TODO: fill in path parameter
+                    "{{param_name}}": "{{ endpoint.default_for_param('path', param_name) }}", # TODO: fill in required path parameter
                     {% endfor %}
-                    {% for param_name in endpoint.unresolvable_query_param_names %}
-                    {% if not endpoint.is_query_param_required(param_name) %}# {% endif %}"{{param_name}}": "{{ endpoint.default_for_param('query', param_name) }}", # TODO: fill in query parameter
+                    {% for param_name in endpoint.unresolvable_required_query_param_names %}
+                    "{{param_name}}": "{{ endpoint.default_for_param('query', param_name) }}", # TODO: fill in required query parameter
                     {% endfor %}
+                    {% if endpoint.unresolvable_unrequired_query_param_names %}
+                    # the parameters below can optionally be configured
+                    {% for param_name in endpoint.unresolvable_unrequired_query_param_names %}
+                    # "{{param_name}}": "{{ endpoint.default_for_param('query', param_name) }}",
+                    {% endfor %}
+                    {% endif %}
+
                 },
                 {% endif %}
                 {% if endpoint.render_pagination_args %}
                 "paginator": {
                     {% for key, value in endpoint.render_pagination_args.items() %}
                     "{{key}}":
                         {% if value is integer %}
```

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/misc.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/paths.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/dlt_init_openapi/utils/update_rest_api.py` & `dlt_init_openapi-0.1.0a2/dlt_init_openapi/utils/update_rest_api.py`

 * *Files identical despite different names*

### Comparing `dlt_init_openapi-0.1.0a1/pyproject.toml` & `dlt_init_openapi-0.1.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt-init-openapi"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Generate dlt Python clients from OpenAPI"
 homepage = "https://dlthub.com"
 repository = "https://github.com/dlt-hub/dlt-init-openapi"
 license = "MIT"
 keywords=["OpenAPI", "Client", "Generator"]
 authors = ["David Scharf <david@dlthub.com>"]
 classifiers = [
```

### Comparing `dlt_init_openapi-0.1.0a1/PKG-INFO` & `dlt_init_openapi-0.1.0a2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt-init-openapi
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Generate dlt Python clients from OpenAPI
 Home-page: https://dlthub.com
 License: MIT
 Keywords: OpenAPI,Client,Generator
 Author: David Scharf
 Author-email: david@dlthub.com
 Requires-Python: >=3.9,<3.13
@@ -34,142 +34,178 @@
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: referencing (>=0.34.0,<0.35.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/dlt-hub/dlt-init-openapi
 Description-Content-Type: text/markdown
 
-# dlt-init-openapi
-`dlt-init-openapi` generates [`dlt`](https://dlthub.com/docs) pipelines from OpenAPI 3.x documents/specs using the [`dlt` `rest_api` `verified source`](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api). If you do not know `dlt` or our `verified sources`, please read:
+# dlt-init-openapi - An OpenAPI Source Generator for the `dlt` Python Library
 
-* [Getting started](https://dlthub.com/docs/getting-started) to learn the `dlt` basics
-* [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) to learn how our `rest_api` source works
-
-> This generator does not support OpenAPI 2.x FKA Swagger. If you need to use an older document, try upgrading it to
-version 3 first with one of many available converters.
-
-
-## Prior work
-This project started as a fork of [openapi-python-client](https://github.com/openapi-generators/openapi-python-client). Pretty much all parts are heavily changed or completely replaced, but some lines of code still exist and we like to acknowledge the many good ideas we got from the original project :)
-
-
-## Support
-If you need support for this tool, [join our slack community](https://dlthub.com/community) and ask for help on the technical help channel. We're usually around to help you out or discuss features :)
+`dlt-init-openapi` generates [`dlt`](https://dlthub.com/docs) data pipelines from OpenAPI 3.x specs using the [`dlt` `rest_api` `verified source`](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) to extract data from any REST API. If you are not familiar with `dlt` or our `verified sources`, please read:
 
+* [Getting started](https://dlthub.com/docs/getting-started) to learn the `dlt` basics.
+* [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) to learn how our `rest_api` source works.
+* We also have a cool [Google Colab example](https://colab.research.google.com/drive/1MRZvguOTZj1MlkEGzjiso8lQ_wr1MJRI?usp=sharing#scrollTo=LHGxzf1Ev_yr) that demonstrates this generator.
 
 ## Features
-The dlt-init-openapi generates code from an OpenAPI spec that you can use to extract data from a `rest_api` into any [`destination`](https://dlthub.com/docs/dlt-ecosystem/destinations/) (e.g. Postgres, BigQuery, Redshift...) `dlt` supports.
-
-Features include
-
-* **[Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery** for each endpoint
-* **Primary key discovery** for each entity
-* **Endpoint relationship mapping** into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g. /users/ -> /user/{id})
-* **Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery** for results nested in the returned json
-* **[Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication)** discovery for an API
+The dlt-init-openapi generates code from an OpenAPI spec that you can use to extract data from a `rest_api` into any [`destination`](https://dlthub.com/docs/dlt-ecosystem/destinations/) (e.g., Postgres, BigQuery, Redshift...) that `dlt` supports. dlt-init-openapi additionally executes a set of heuristics to discover information not explicitly defined in OpenAPI specs.
 
-## Setup
+Features include:
 
-You will need Python 3.9 or higher installed, as well as pip.
+* **[Pagination](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#pagination) discovery** for each endpoint.
+* **Primary key discovery** for each entity.
+* **Endpoint relationship mapping** into `dlt` [`transformers`](https://dlthub.com/docs/general-usage/resource#process-resources-with-dlttransformer) (e.g., /users/ -> /user/{id}).
+* **Payload JSON path [data selector](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#data-selection) discovery** for results nested in the returned JSON.
+* **[Authentication](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api#authentication)** discovery for an API.
 
-```console
-# 1. install this tool locally
-$ pip install dlt-init-openapi
+## Support
+If you need support for this tool or `dlt`, please [join our Slack community](https://dlthub.com/community) and ask for help on the technical help channel. We're usually around to help you out or discuss features :)
 
-# 2. Show the version of the installed package to verify it worked
-$ dlt-init-openapi --version
-```
+## A quick example
 
-## Basic Usage
+You will need Python 3.9 or higher installed, as well as pip. You can run `pip install dlt-init-openapi` to install the current version.
 
-Let's create an example pipeline from the [PokeAPI spec](https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml). You can point to any other OpenAPI Spec instead if you like.
+We will create a simple example pipeline from a [PokeAPI spec](https://pokeapi.co/) in our repo. You can point to any other OpenAPI Spec instead if you prefer.
 
 ```console
-# 1.a. Run the generator with an url:
-$ dlt-init-openapi pokemon --url https://raw.githubusercontent.com/cliffano/pokeapi-clients/ec9a2707ef2a85f41b747d8df013e272ef650ec5/specification/pokeapi.yml
+# 1.a. Run the generator with a URL:
+$ dlt-init-openapi pokemon --url https://raw.githubusercontent.com/dlt-hub/dlt-init-openapi/devel/tests/cases/e2e_specs/pokeapi.yml --global-limit 2
 
 # 1.b. If you have a local file, you can use the --path flag:
 $ dlt-init-openapi pokemon --path ./my_specs/pokeapi.yml
 
-# 2. You can now pick the endpoints you need from the popup
+# 2. You can now pick both of the endpoints from the popup.
 
-# 3. After selecting your pokemon endpoints and hitting Enter, your pipeline will be rendered
+# 3. After selecting your Pokemon endpoints and hitting Enter, your pipeline will be rendered.
 
-# 4. If you have any kind of authentication on your pipeline (this example has not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
+# 4. If you have any kind of authentication on your pipeline (this example does not), open the `.dlt/secrets.toml` and provide the credentials. You can find further settings in the `.dlt/config.toml`.
 
-# 5. Go to the created pipeline folder and run your pipeline
+# 5. Go to the created pipeline folder and run your pipeline.
 $ cd pokemon-pipeline
 $ PROGRESS=enlighten python pipeline.py # we use enlighten for a nice progress bar :)
 
-# 6. Print the pipeline info to console to see what got loaded
+# 6. Print the pipeline info to the console to see what got loaded.
 $ dlt pipeline pokemon_pipeline info
 
-# 7. You can now also install streamlit to see a preview of the data
+# 7. You can now also install Streamlit to see a preview of the data; you should have loaded 40 Pokemons and their details.
 $ pip install pandas streamlit
 $ dlt pipeline pokemon_pipeline show
 
-# 8. You can go to our docs at https://dlthub.com/docs to learn how modify the generated pipeline to load to many destinations, place schema contracts on your pipeline and many other things.
-```
+# 8. You can go to our docs at https://dlthub.com/docs to learn how to modify the generated pipeline to load to many destinations, place schema contracts on your pipeline, and many other things.
 
-## What will be created?
-When you run the `init` command above, the following files will be generated:
+# NOTE: We used the `--global-limit 2` CLI flag to limit the requests to the PokeAPI for this example. This way, the Pokemon collection endpoint only gets queried twice, resulting in 2 x 20 Pokemon
 
-* `./pokemon-pipeline` - a folder containing the full project.
-* `./pokemon-pipeline/pipeline.py` - a file which you can execute to run your pipeline.
-* `./pokemon-pipeline/pokemon/__init__.py` - a file that contains the generated code to connect to the PokeApi, you can inspect this file and manually change it to your liking or to fix incorrectly generated results.
-* `./pokemon-pipeline/.dlt` - a folder with the `config.toml`. You can add your `secrets.toml` with credentials here.
-* `./pokemon-pipeline/rest_api` -  a folder that contains the rest_api source from our verified sources.
+ details being rendered.
+```
 
-> If you re-generate your pipeline, you will be prompted to continue if this folder exists. If you select yes, all generated files will be overwritten. All other files you may have created will remain in this folder.
+## What will be created?
 
-## CLI commands
+When you run the `init` command above, the following files will be generated:
 
-```console
-$ dlt-init-openapi [OPTIONS] <source_name> [ARGS]
-# example:
-$ dlt-init-openapi pokemon --path ./path/to/my_spec.yml
+```
+pokemon_pipeline/
+├── .dlt/
+│   ├── config.toml     # dlt config, learn more at dlthub.com/docs
+│   └── secrets.toml    # your secrets, only needed for APIs with auth
+├── pokemon/
+│   └── __init__.py     # your rest_api dictionary, learn more below
+├── rest_api/
+│   └── ...             # rest_api copied from our verified sources repo
+├── .gitignore
+├── pokemon_pipeline.py # your pipeline file that you can execute
+├── README.md           # a list of your endpoints with some additional info
+└── requirements.txt    # the pip requirements for your pipeline
 ```
 
-**Options**:
-
-- `--version`: Print the version and exit
-- `--help`: Show this message and exit.
+> If you re-generate your pipeline, you will be prompted to continue if this folder exists. If you select yes, all generated files will be overwritten. All other files you may have created will remain in this folder.
 
-**Commands**:
+## A closer look at your rest_api dictionary in pokemon/__init__.py
 
-- `init`: Generate a new `dlt` `rest_api` `source`
+This file contains the configuration dictionary for the [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) source which is the main result of running this generator. For our Pokemon example, we have used an OpenAPI 3 spec that works out of the box. The result of this dictionary depends on the quality of the spec you are using, whether the API you are querying actually adheres to this spec, and whether our heuristics manage to find the right values. You can edit this file to adapt the behavior of the dlt rest_api accordingly. Please read our [dlt rest_api](https://dlthub.com/docs/dlt-ecosystem/verified-sources/rest_api) docs to learn how to do this and play with our detailed [Google Colab example](https://colab.research.google.com/drive/1MRZvguOTZj1MlkEGzjiso8lQ_wr1MJRI?usp=sharing#scrollTo=LHGxzf1Ev_yr).
 
-### `dlt-init-openapi`
+The generated dictionary will look something like this:
 
-Generate a new `dlt` `rest_api` `source`
+```python
+{
+    "client": {
+        "base_url": base_url,
+        # -> the detected common paginator
+        "paginator": {
+            ...
+        },
+    },
+    # -> your two endpoints
+    "resources": [
+        {
+            # -> A primary key could not be inferred from
+            # the spec; usual suspects such as id, pokemon_id, etc.
+            # are not defined. You can add one if you know.
+            "name": "pokemon_list",
+            "table_name": "pokemon",
+            "endpoint": {
+                # -> the results seem to be nested in { results: [...] }
+                "data_selector": "results",
+                "path": "/api/v2/pokemon/",
+            },
+        },
+        {
+            "name": "pokemon_read",
+            "table_name": "pokemon",
+            # -> A primary key *name* is assumed, as it is found in the 
+            # url.
+            "primary_key": "name",
+            "write_disposition": "merge",
+            "endpoint": {
+                "data_selector": "$",
+                "path": "/api/v2/pokemon/{name}/",
+                "params": {
+                    # -> your detected transformer settings
+                    # this is a child endpoint of the pokemon_list
+                    "name": {
+                        "type": "resolve",
+                        "resource": "pokemon_list",
+                        "field": "name",
+                    },
+                },
+            },
+        },
+    ],
+}
+```
 
-**Usage**:
+## CLI command
 
 ```console
-$ dlt-init-openapi pokemon --path ./path/to/my_spec.yml
+$ dlt-init-openapi <source_name> [OPTIONS]
+# example:
+$ dlt-init-openapi pokemon --path ./path/to/my_spec.yml --no-interactive --output-path ./my_pipeline
 ```
 
 **Options**:
 
-- `--url URL`: A url to read the OpenAPI JSON or YAML file from
-- `--path PATH`: A path to read the OpenAPI JSON or YAML file from locally
-- `--output-path PATH`: A path to render the output to
-- `--config PATH`: Path to the config file to use (see below)
+_The only required options are either to supply a path or a URL to a spec_
+
+- `--url URL`: A URL to read the OpenAPI JSON or YAML file from.
+- `--path PATH`: A path to read the OpenAPI JSON or YAML file from locally.
+- `--output-path PATH`: A path to render the output to.
+- `--config PATH`: Path to the config file to use (see below).
 - `--no-interactive`: Skip endpoint selection and render all paths of the OpenAPI spec.
-- `--log-level`: Set logging level for stdout output, defaults to 20 (INFO).
+- `--log-level`: Set the logging level for stdout output, defaults to 20 (INFO).
 - `--global-limit`: Set a global limit on the generated source.
 - `--update-rest-api-source`: Update the locally cached rest_api verified source.
-- `--allow-openapi-2`: Allow to use OpenAPI v2. specs. Migration of the spec to 3.0 is recommended though.
-- `--version`: Show installed version of the generator.
+- `--allow-openapi-2`: Allows the use of OpenAPI v2. specs. Migration of the spec to 3.0 is recommended
+
+ for better results though.
+- `--version`: Show the installed version of the generator and exit.
 - `--help`: Show this message and exit.
 
 ## Config options
 You can pass a path to a config file with the `--config PATH` argument. To see available config values, go to https://github.com/dlt-hub/dlt-init-openapi/blob/devel/dlt_init_openapi/config.py and read the information below each field on the `Config` class.
 
-The config file can be supplied as json or yaml dictionary. For example to change the package name, you can create a yaml file:
+The config file can be supplied as JSON or YAML dictionary. For example, to change the package name, you can create a YAML file:
 
 ```yaml
 # config.yml
 package_name: "other_package_name"
 ```
 
 And use it with the config argument:
@@ -177,11 +213,14 @@
 ```console
 $ dlt-init-openapi pokemon --url ... --config config.yml
 ```
 
 ## Telemetry
 We track your usage of this tool similar to how we track other commands in the dlt core library. Read more about this and how to disable it here: https://dlthub.com/docs/reference/telemetry.
 
-## Implementation notes
-* OAuth Authentication currently is not natively supported, you can supply your own
-* Per endpoint authentication currently is not supported by the generator, only the first globally set securityScheme will be applied. You can add your own per endpoint if you need to.
+## Prior work
+This project started as a fork of [openapi-python-client](https://github.com/openapi-generators/openapi-python-client). Pretty much all parts are heavily changed or completely replaced, but some lines of code still exist, and we like to acknowledge the many good ideas we got from the original project :)
 
+## Implementation notes
+* OAuth Authentication currently is not natively supported. You can supply your own.
+* Per endpoint authentication currently is not supported by the generator. Only the first globally set securityScheme will be applied. You can add your own per endpoint if you need to.
+* Basic OpenAPI 2.0 support is implemented. We recommend updating your specs at https://editor.swagger.io before using `dlt-init-openapi`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

