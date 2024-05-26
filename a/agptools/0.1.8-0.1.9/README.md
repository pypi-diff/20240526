# Comparing `tmp/agptools-0.1.8-py2.py3-none-any.whl.zip` & `tmp/agptools-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 74741 bytes, number of entries: 22
--rw-rw-r--  2.0 unx      139 b- defN 24-Feb-26 08:11 agptools/__init__.py
+Zip file size: 75133 bytes, number of entries: 23
+-rw-rw-r--  2.0 unx      139 b- defN 24-Mar-14 14:07 agptools/__init__.py
 -rw-rw-r--  2.0 unx      553 b- defN 24-Jan-15 06:21 agptools/agptools.py
 -rw-rw-r--  2.0 unx     1500 b- defN 24-Jan-15 06:28 agptools/colors.py
 -rw-rw-r--  2.0 unx    22581 b- defN 24-Jan-16 19:23 agptools/configurations.py
 -rw-rw-r--  2.0 unx    68817 b- defN 24-Jan-25 04:58 agptools/containers.py
 -rw-rw-r--  2.0 unx    69519 b- defN 24-Jan-23 16:09 agptools/containers.review.merge.py
 -rw-rw-r--  2.0 unx    68670 b- defN 24-Jan-23 19:59 agptools/containers.safe.py
 -rw-rw-r--  2.0 unx     6272 b- defN 24-Feb-26 07:42 agptools/files.py
--rw-rw-r--  2.0 unx     8183 b- defN 24-Feb-17 18:54 agptools/helpers.py
+-rw-rw-r--  2.0 unx     8624 b- defN 24-Mar-13 20:21 agptools/helpers.py
 -rw-rw-r--  2.0 unx    16563 b- defN 24-Feb-26 08:11 agptools/logs.py
+-rw-rw-r--  2.0 unx      360 b- defN 24-Mar-09 08:34 agptools/progress.py
 -rw-rw-r--  2.0 unx      849 b- defN 24-Jan-15 06:21 agptools/cli/__init__.py
 -rw-rw-r--  2.0 unx     3708 b- defN 24-Jan-15 06:21 agptools/cli/config.py
 -rw-rw-r--  2.0 unx     1559 b- defN 24-Jan-15 06:21 agptools/cli/main.py
 -rw-rw-r--  2.0 unx       39 b- defN 24-Jan-15 06:21 agptools/cli/wingdbstub.py
 -rw-rw-r--  2.0 unx     3118 b- defN 24-Jan-15 06:21 agptools/cli/workspace.py
--rw-rw-r--  2.0 unx      168 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/AUTHORS.rst
--rw-rw-r--  2.0 unx     1075 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1933 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1771 b- defN 24-Feb-26 08:11 agptools-0.1.8.dist-info/RECORD
-22 files, 277183 bytes uncompressed, 71891 bytes compressed:  74.1%
+-rw-rw-r--  2.0 unx      168 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/AUTHORS.rst
+-rw-rw-r--  2.0 unx     1075 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1933 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1847 b- defN 24-Mar-14 14:07 agptools-0.1.9.dist-info/RECORD
+23 files, 278060 bytes uncompressed, 72167 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: agptools/helpers.py
 Comment: 
 
 Filename: agptools/logs.py
 Comment: 
 
+Filename: agptools/progress.py
+Comment: 
+
 Filename: agptools/cli/__init__.py
 Comment: 
 
 Filename: agptools/cli/config.py
 Comment: 
 
 Filename: agptools/cli/main.py
@@ -39,29 +42,29 @@
 
 Filename: agptools/cli/wingdbstub.py
 Comment: 
 
 Filename: agptools/cli/workspace.py
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/AUTHORS.rst
+Filename: agptools-0.1.9.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/LICENSE
+Filename: agptools-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/METADATA
+Filename: agptools-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/WHEEL
+Filename: agptools-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/entry_points.txt
+Filename: agptools-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/top_level.txt
+Filename: agptools-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: agptools-0.1.8.dist-info/RECORD
+Filename: agptools-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agptools/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Top-level package for agp Tools."""
 
 __author__ = """Asterio Gonzalez"""
 __email__ = "asterio.gonzalez@gmail.com"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## agptools/helpers.py

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import uuid
 import yaml
 
 import string
 from datetime import timedelta
 from dateutil import parser
 from glom import glom, assign
@@ -161,15 +162,15 @@
 # CHAR_LOOKUP = list(string.digits + string.ascii_letters)
 
 #  avoid use of numbers (so can be used as regular attribute names with ".")
 CHAR_LOOKUP = list(string.ascii_letters)
 INV_LOOKUP = {c: i for i, c in enumerate(CHAR_LOOKUP)}
 
 
-def convert_base(number, base, padding=-1, lookup=CHAR_LOOKUP):
+def convert_base(number, base, padding=-1, lookup=CHAR_LOOKUP) -> str:
     """Coding a number into a string in base 'base'
 
     results will be padded with '0' until minimal 'padding'
     length is reached.
 
     lookup is the char map available for coding.
     """
@@ -207,14 +208,28 @@
 
 def new_uid(base=50):
     global SEED
     SEED += 1
     return convert_base(SEED, base)
 
 
+# ------------------------------------------------
+# File and config helpers
+# ------------------------------------------------
+def replace(text):
+    text = str(text)
+    text = text.lower()
+    text = text.replace("á", "a")
+    text = text.replace("é", "e")
+    text = text.replace("í", "i")
+    text = text.replace("ó", "o")
+    text = text.replace("ú", "u")
+    return text
+
+
 # from xml.sax.saxutils import escape
 # ------------------------------------------------
 # jinja2 filters
 # ------------------------------------------------
 def escape(text: str):
     text = text.replace("&", "&amp;")
     text = text.replace("<", "&lt;")
@@ -243,14 +258,16 @@
         return val
     return current
 
 
 # ------------------------------------------------
 # Converter functions
 # ------------------------------------------------
+
+
 def I(x):
     return x
 
 
 def INT(x):
     return int(x)
 
@@ -263,14 +280,18 @@
     return x.lower() in ("true", "yes")
 
 
 def TEXT(x):
     return x.text
 
 
+def STRIP(x):
+    return x.strip()
+
+
 def DATE(x):  # TODO
     return parser.parse(x)
 
 
 def DURATION(x):  # TODO
     return timedelta(days=float(x))
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `agptools-0.1.8.dist-info/LICENSE` & `agptools-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `agptools-0.1.8.dist-info/METADATA` & `agptools-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agptools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Minimal Tools not found in python library
 Home-page: https://github.com/asterio/agptools
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: MIT license
 Keywords: agptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `agptools-0.1.8.dist-info/RECORD` & `agptools-0.1.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-agptools/__init__.py,sha256=pEWxCwSg-H_Sb4V0e5Ezz58EKK4jrwSF4EZ_gpe6qr4,139
+agptools/__init__.py,sha256=7iO8rHwt1XCGkip8DU7IxVu9vCswAxeXiRhMgSwYvj4,139
 agptools/agptools.py,sha256=xy6OsXtn5IbPB5lN0CwQcykGRu00i0Fti8NraeVBdS4,553
 agptools/colors.py,sha256=PrquojMjHxldTFNk0F5kKaELd9WnabtTL0tVJ-JhBLQ,1500
 agptools/configurations.py,sha256=NWl_8BWyMUvLuiCQaFI678EAWOoPq5B89VowCWnWpgw,22581
 agptools/containers.py,sha256=8M2qm3WKj3W7q9XvhShT4H1BqWBhaequoDC9WPAxQCE,68817
 agptools/containers.review.merge.py,sha256=ginWFwdQhiMbGC8q2QJ0tf9k3qksQytRVVxzd4HSmFE,69519
 agptools/containers.safe.py,sha256=JqRPxnn3QXENWDDWHd1hdnTI85my3ClLFmJMODZvYfc,68670
 agptools/files.py,sha256=9rbOsyVjPTZFpX6tCq-1OyHKD__kk6ZzlK6dpsEXiiY,6272
-agptools/helpers.py,sha256=3RoNXbBQiW8RlAkjK6INfk0mc_Eog_bxaDuTWwfL_t4,8183
+agptools/helpers.py,sha256=L5gQ_gbcIK3ujROq84cKvP8szFP3gKXajZjHUxwEtxw,8624
 agptools/logs.py,sha256=M94ztySsdf1kibhRlMBXkNxG0tNmlu6yubWeJUyA1_Y,16563
+agptools/progress.py,sha256=ermVYUUjp1tQZFtVdCH0FZ1rn2eJ72V1RDtV2XQg1zc,360
 agptools/cli/__init__.py,sha256=HUI6I2dGa8D1_k0RfZRc-VZZ4m4it0UItIzkNzUeM-Y,849
 agptools/cli/config.py,sha256=1ofGVKtYi3yXMiwrxGmXhLTUxf0zHlJP8oyXJ4X_n0M,3708
 agptools/cli/main.py,sha256=anezHuse4KfEJiHmv_I_5hW21FIERpo02CM0OLBN6NY,1559
 agptools/cli/wingdbstub.py,sha256=3jzRnyg351_Z898pxFfEZvfr93m3msCf4rQYBAKMRjQ,39
 agptools/cli/workspace.py,sha256=Bouxt2sqDKzEHkD4lfxTChvnS_SNdU5A2XcV9Tf31bU,3118
-agptools-0.1.8.dist-info/AUTHORS.rst,sha256=3ZPoqg8Aav8DSYKd0fwcwn4_5HwSiMLart0E5Un00-U,168
-agptools-0.1.8.dist-info/LICENSE,sha256=JqzQ9S4hVjQBOM8SiUG9-qhokt1oKfE2qJMRNa3t410,1075
-agptools-0.1.8.dist-info/METADATA,sha256=U4cky_3S83SrQfW8uKUZ9n17lZBzU7t_BQSzw_b60DI,1933
-agptools-0.1.8.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-agptools-0.1.8.dist-info/entry_points.txt,sha256=zbovPO5BmPiuD4Iqevmok0c6MM0o_FaeByIVaiO25_0,47
-agptools-0.1.8.dist-info/top_level.txt,sha256=ukN3Z00rxhQVlAnwCqEYzW6QhQuK6JOE21aaupcVGzg,9
-agptools-0.1.8.dist-info/RECORD,,
+agptools-0.1.9.dist-info/AUTHORS.rst,sha256=3ZPoqg8Aav8DSYKd0fwcwn4_5HwSiMLart0E5Un00-U,168
+agptools-0.1.9.dist-info/LICENSE,sha256=JqzQ9S4hVjQBOM8SiUG9-qhokt1oKfE2qJMRNa3t410,1075
+agptools-0.1.9.dist-info/METADATA,sha256=Ui9APJy3XgljQO2XnRE_9EZm7i6S3J2ku5vRRDTiT_k,1933
+agptools-0.1.9.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+agptools-0.1.9.dist-info/entry_points.txt,sha256=zbovPO5BmPiuD4Iqevmok0c6MM0o_FaeByIVaiO25_0,47
+agptools-0.1.9.dist-info/top_level.txt,sha256=ukN3Z00rxhQVlAnwCqEYzW6QhQuK6JOE21aaupcVGzg,9
+agptools-0.1.9.dist-info/RECORD,,
```

