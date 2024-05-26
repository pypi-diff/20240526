# Comparing `tmp/comicon-1.1.0.tar.gz` & `tmp/comicon-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-1.1.0.tar", max compression
+gzip compressed data, was "comicon-1.2.0.tar", max compression
```

## Comparing `comicon-1.1.0.tar` & `comicon-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-1.1.0/LICENSE
--rw-r--r--   0        0        0     1752 2023-06-22 01:19:15.083880 comicon-1.1.0/README.md
--rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-1.1.0/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-1.1.0/comicon/api.py
--rw-r--r--   0        0        0     1894 2024-05-14 15:26:27.479130 comicon-1.1.0/comicon/base.py
--rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-1.1.0/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.1.0/comicon/common/__init__.py
--rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-1.1.0/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.1.0/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.1.0/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.1.0/comicon/common/pdf.py
--rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-1.1.0/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-1.1.0/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4807 2023-06-21 22:40:25.769680 comicon-1.1.0/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-1.1.0/comicon/inputs/cir.py
--rw-r--r--   0        0        0     6845 2023-06-21 22:57:31.844781 comicon-1.1.0/comicon/inputs/epub.py
--rw-r--r--   0        0        0     3034 2023-06-21 22:56:41.986407 comicon-1.1.0/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1905 2023-06-22 00:47:58.838468 comicon-1.1.0/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-1.1.0/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-1.1.0/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-1.1.0/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1971 2023-06-22 01:17:24.469271 comicon-1.1.0/comicon/outputs/mobi.py
--rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-1.1.0/comicon/outputs/pdf.py
--rw-r--r--   0        0        0     1007 2024-05-14 15:25:33.791489 comicon-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 comicon-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1752 2023-06-22 01:19:15.083880 comicon-1.2.0/README.md
+-rw-r--r--   0        0        0      362 2024-05-26 16:49:22.008268 comicon-1.2.0/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-26 16:49:14.158367 comicon-1.2.0/comicon/api.py
+-rw-r--r--   0        0        0     2246 2024-05-26 16:50:51.636142 comicon-1.2.0/comicon/base.py
+-rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-1.2.0/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.2.0/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-1.2.0/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.2.0/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.2.0/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-1.2.0/comicon/common/pdf.py
+-rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-1.2.0/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-1.2.0/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4807 2023-06-21 22:40:25.769680 comicon-1.2.0/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-1.2.0/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     6845 2023-06-21 22:57:31.844781 comicon-1.2.0/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     3034 2023-06-21 22:56:41.986407 comicon-1.2.0/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1905 2023-06-22 00:47:58.838468 comicon-1.2.0/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-1.2.0/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-1.2.0/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-1.2.0/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1971 2023-06-22 01:17:24.469271 comicon-1.2.0/comicon/outputs/mobi.py
+-rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-1.2.0/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0     1007 2024-05-26 16:49:47.217951 comicon-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 comicon-1.2.0/PKG-INFO
```

### Comparing `comicon-1.1.0/LICENSE` & `comicon-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/README.md` & `comicon-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/api.py` & `comicon-1.2.0/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/base.py` & `comicon-1.2.0/comicon/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import json
 from dataclasses import asdict, dataclass, field
 from typing import Any, cast
 
 from slugify import slugify
 
 
+SLUGIFY_ARGS = {
+    "allow_unicode": True,
+    "regex_pattern": r'["<:\?\*\|/>\\]+',
+    "replacements": [
+        [":", ";"],
+        ["/", ""],
+        ["?", ""],
+        ["*", "x"],
+        ["|", ""],
+        ["<", ""],
+        [">", ""],
+        ['"', ""],
+        ["!", ""],
+        ["'", "`"],
+    ],
+    "lowercase": False,
+}
+
+
 @dataclass
 class Chapter:
     title: str
     slug: str  # on the filesystem
 
 
 @dataclass
@@ -18,15 +37,15 @@
     description: str | None = None
     genres: list[str] = field(default_factory=list)
     cover_path_rel: str | None = None
     extra_metadata: dict[str, Any] = field(default_factory=dict)
     title_slug: str = ""
 
     def __post_init__(self):
-        self.title_slug = slugify(self.title)
+        self.title_slug = slugify(self.title, **SLUGIFY_ARGS)
 
     def merge_with(self, other: "Metadata") -> "Metadata":
         """
         Merge metadata from two comics. The new comic's metadata takes precedence,
         as long as it exists. This updates the current metadata in place.
         """
         if other.title:
```

### Comparing `comicon-1.1.0/comicon/cirtools.py` & `comicon-1.2.0/comicon/cirtools.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/errors.py` & `comicon-1.2.0/comicon/errors.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/inputs/__init__.py` & `comicon-1.2.0/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/inputs/cbz.py` & `comicon-1.2.0/comicon/inputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/inputs/cir.py` & `comicon-1.2.0/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/inputs/epub.py` & `comicon-1.2.0/comicon/inputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/inputs/pdf.py` & `comicon-1.2.0/comicon/inputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/__init__.py` & `comicon-1.2.0/comicon/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/cbz.py` & `comicon-1.2.0/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/cir.py` & `comicon-1.2.0/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/epub.py` & `comicon-1.2.0/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/mobi.py` & `comicon-1.2.0/comicon/outputs/mobi.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/comicon/outputs/pdf.py` & `comicon-1.2.0/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-1.1.0/pyproject.toml` & `comicon-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicon"
-version = "1.1.0"
+version = "1.2.0"
 description = "A simple comic conversion library between CBZ/EPUB/MOBI/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
 keywords = ["converter", "comic", "cbz", "epub", "pdf", "mobi"]
```

### Comparing `comicon-1.1.0/PKG-INFO` & `comicon-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple comic conversion library between CBZ/EPUB/MOBI/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
 Keywords: converter,comic,cbz,epub,pdf,mobi
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
```

