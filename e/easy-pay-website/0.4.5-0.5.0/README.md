# Comparing `tmp/easy_pay_website-0.4.5.tar.gz` & `tmp/easy_pay_website-0.5.0.tar.gz`

## Comparing `easy_pay_website-0.4.5.tar` & `easy_pay_website-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/mkdocs.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/__init__.py
--rw-r--r--   0        0        0    15688 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/src/easy_pay_website/py.typed
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/LICENSE
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/README.md
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easy_pay_website-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/src/easy_pay_website/__init__.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/src/easy_pay_website/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/src/easy_pay_website/py.typed
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/LICENSE
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/README.md
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 easy_pay_website-0.5.0/PKG-INFO
```

### Comparing `easy_pay_website-0.4.5/mkdocs.yml` & `easy_pay_website-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.5/.gitignore` & `easy_pay_website-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.5/LICENSE` & `easy_pay_website-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_pay_website-0.4.5/pyproject.toml` & `easy_pay_website-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 dependencies = [
   "Pillow == 9.5.0",
   "ddddocr >= 1.4.7",
   "requests >= 2.31.0",
   "beautifulsoup4 >= 4.12.2",
   "pytz >= 2023.3",
   "odin-functions == 0.0.3",
+  "httpx == 0.27.0",
 ]
 description = "easy pay website"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "easy_pay_website"
 readme = "README.md"
```

### Comparing `easy_pay_website-0.4.5/PKG-INFO` & `easy_pay_website-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: easy_pay_website
-Version: 0.4.5
+Version: 0.5.0
 Summary: easy pay website
 Project-URL: Documentation, https://asmitul.github.io/easy_pay_website
 Project-URL: Issues, https://github.com/asmitul/easy_pay_website/issues
 Project-URL: Source, https://github.com/asmitul/easy_pay_website
 Author: asmitul
 License-Expression: MIT
 License-File: LICENSE
@@ -22,14 +22,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.8
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: ddddocr>=1.4.7
+Requires-Dist: httpx==0.27.0
 Requires-Dist: odin-functions==0.0.3
 Requires-Dist: pillow==9.5.0
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests>=2.31.0
 Provides-Extra: docs
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
```

