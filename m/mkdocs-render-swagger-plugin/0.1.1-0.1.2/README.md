# Comparing `tmp/mkdocs_render_swagger_plugin-0.1.1-py3-none-any.whl.zip` & `tmp/mkdocs_render_swagger_plugin-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5959 bytes, number of entries: 7
--rw-r--r--  2.0 unx     5185 b- defN 23-Oct-07 04:57 render_swagger.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4048 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      681 b- defN 23-Oct-07 05:20 mkdocs_render_swagger_plugin-0.1.1.dist-info/RECORD
-7 files, 11150 bytes uncompressed, 4721 bytes compressed:  57.7%
+Zip file size: 5988 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     5250 b- defN 24-May-26 19:21 render_swagger.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4048 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 24-May-26 19:25 mkdocs_render_swagger_plugin-0.1.2.dist-info/RECORD
+7 files, 11215 bytes uncompressed, 4750 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: render_swagger.py
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/LICENSE
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/METADATA
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/WHEEL
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/entry_points.txt
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/top_level.txt
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mkdocs_render_swagger_plugin-0.1.1.dist-info/RECORD
+Filename: mkdocs_render_swagger_plugin-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## render_swagger.py

```diff
@@ -6,15 +6,15 @@
 from xml.sax.saxutils import escape
 
 import mkdocs.plugins
 from mkdocs.config import config_options
 from mkdocs.config.base import Config as MkDocsConfig
 from mkdocs.structure.files import File
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 USAGE_MSG = (
     "Usage: '!!swagger <filename>!!' or '!!swagger-http <url>!!'. "
     "File must either exist locally and be placed next to the .md that "
     "contains the swagger statement, or be an http(s) URL.")
 
 TEMPLATE = string.Template("""
@@ -60,14 +60,15 @@
     """
     Provides the actual swagger library used
     """
     lib_swagger = DEFAULT_SWAGGER_LIB.copy()
     extra_javascript = config.get('extra_javascript', [])
     extra_css = config.get('extra_css', [])
     for lib in extra_javascript:
+        lib = str(lib)  # Can be an instance of ExtraScriptValue
         if os.path.basename(
                 urllib.parse.urlparse(lib).path) == 'swagger-ui-bundle.js':
             import warnings
             warnings.warn(
                 "Please use the javascript configuration option for "
                 "mkdocs-render-swagger-plugin instead of extra_javascript.",
                 FutureWarning)
```

## Comparing `mkdocs_render_swagger_plugin-0.1.1.dist-info/LICENSE` & `mkdocs_render_swagger_plugin-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mkdocs_render_swagger_plugin-0.1.1.dist-info/METADATA` & `mkdocs_render_swagger_plugin-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-render-swagger-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: MKDocs plugin for rendering swagger & openapi files.
 Home-page: https://github.com/bharel/mkdocs-render-swagger-plugin
 Author: Bar Harel
 Author-email: bzvi7919@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `mkdocs_render_swagger_plugin-0.1.1.dist-info/RECORD` & `mkdocs_render_swagger_plugin-0.1.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-render_swagger.py,sha256=4-FrxdVrXB67uct-ik20QhKg04gjs-Mf9FcM03S4MeU,5185
-mkdocs_render_swagger_plugin-0.1.1.dist-info/LICENSE,sha256=PN-eDuinpkD9KmXW96dih-SNJe6_AIFatxjNwg2nUu8,1066
-mkdocs_render_swagger_plugin-0.1.1.dist-info/METADATA,sha256=QacMwWyLicrx3MAfIZJEY-es6wDu6EXy1Kq9x4_g0BQ,4048
-mkdocs_render_swagger_plugin-0.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-mkdocs_render_swagger_plugin-0.1.1.dist-info/entry_points.txt,sha256=LsrdNHcm_Jx2Bc7lgliGykFABcMPgAIRSd966pegIJU,63
-mkdocs_render_swagger_plugin-0.1.1.dist-info/top_level.txt,sha256=C8r_cRMAN1EOaaJZ19_zVLprM6ZFUfYMVGrubzFuczA,15
-mkdocs_render_swagger_plugin-0.1.1.dist-info/RECORD,,
+render_swagger.py,sha256=2906yjlTQzFvBEyRcB7YOznB7qMR5V7J97DqA6FkDDo,5250
+mkdocs_render_swagger_plugin-0.1.2.dist-info/LICENSE,sha256=PN-eDuinpkD9KmXW96dih-SNJe6_AIFatxjNwg2nUu8,1066
+mkdocs_render_swagger_plugin-0.1.2.dist-info/METADATA,sha256=TXa8vSZOfLBhL8raW0Pi5TfZ6nSCV9_LIUYxmUhzHoc,4048
+mkdocs_render_swagger_plugin-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mkdocs_render_swagger_plugin-0.1.2.dist-info/entry_points.txt,sha256=LsrdNHcm_Jx2Bc7lgliGykFABcMPgAIRSd966pegIJU,63
+mkdocs_render_swagger_plugin-0.1.2.dist-info/top_level.txt,sha256=C8r_cRMAN1EOaaJZ19_zVLprM6ZFUfYMVGrubzFuczA,15
+mkdocs_render_swagger_plugin-0.1.2.dist-info/RECORD,,
```

