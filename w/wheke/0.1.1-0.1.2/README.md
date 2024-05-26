# Comparing `tmp/wheke-0.1.1.tar.gz` & `tmp/wheke-0.1.2.tar.gz`

## Comparing `wheke-0.1.1.tar` & `wheke-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wheke-0.1.1/.env.example
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wheke-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 wheke-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 wheke-0.1.1/.github/workflows/test-suite.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wheke-0.1.1/docs/api.md
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 wheke-0.1.1/docs/index.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 wheke-0.1.1/docs/pods.md
--rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.1/docs/wheke.png
--rw-r--r--   0        0        0   390125 2020-02-02 00:00:00.000000 wheke-0.1.1/docs/img/wheke-homepage.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/__about__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/__main__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_cli.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_core.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_demo.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_pod.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_service.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/py.typed
--rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.1/src/wheke/static/wheke.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/test_app.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/example_app/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wheke-0.1.1/tests/example_app/static/test.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 wheke-0.1.1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wheke-0.1.1/README.md
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 wheke-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 wheke-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 wheke-0.1.2/.env.example
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wheke-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 wheke-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 wheke-0.1.2/.github/workflows/test-suite.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 wheke-0.1.2/docs/api.md
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 wheke-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 wheke-0.1.2/docs/pods.md
+-rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.2/docs/wheke.png
+-rw-r--r--   0        0        0   390125 2020-02-02 00:00:00.000000 wheke-0.1.2/docs/img/wheke-homepage.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/__about__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/__main__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_cli.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_core.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_demo.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_pod.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_service.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/py.typed
+-rw-r--r--   0        0        0    24960 2020-02-02 00:00:00.000000 wheke-0.1.2/src/wheke/static/wheke.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/test_app.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/example_app/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 wheke-0.1.2/tests/example_app/static/test.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 wheke-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wheke-0.1.2/README.md
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 wheke-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 wheke-0.1.2/PKG-INFO
```

### Comparing `wheke-0.1.1/mkdocs.yml` & `wheke-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/.github/workflows/docs.yml` & `wheke-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/.github/workflows/test-suite.yml` & `wheke-0.1.2/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/docs/index.md` & `wheke-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/docs/pods.md` & `wheke-0.1.2/docs/pods.md`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/docs/wheke.png` & `wheke-0.1.2/docs/wheke.png`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/docs/img/wheke-homepage.png` & `wheke-0.1.2/docs/img/wheke-homepage.png`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/src/wheke/_core.py` & `wheke-0.1.2/src/wheke/_core.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/src/wheke/_demo.py` & `wheke-0.1.2/src/wheke/_demo.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/src/wheke/_pod.py` & `wheke-0.1.2/src/wheke/_pod.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/src/wheke/static/wheke.png` & `wheke-0.1.2/src/wheke/static/wheke.png`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/tests/test_app.py` & `wheke-0.1.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/tests/test_cli.py` & `wheke-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/tests/example_app/__init__.py` & `wheke-0.1.2/tests/example_app/__init__.py`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/LICENSE.txt` & `wheke-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/README.md` & `wheke-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/pyproject.toml` & `wheke-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wheke-0.1.1/PKG-INFO` & `wheke-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wheke
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cute framework for small self-hosted apps
 Project-URL: Documentation, https://wheke.humberto.io/
 Project-URL: Issues, https://github.com/humrochagf/wheke/issues
 Project-URL: Source, https://github.com/humrochagf/wheke
 Author-email: Humberto Rocha <humrochagf@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wheke Version: 0.1.1 Summary: A cute framework for
+Metadata-Version: 2.3 Name: wheke Version: 0.1.2 Summary: A cute framework for
 small self-hosted apps Project-URL: Documentation, https://wheke.humberto.io/
 Project-URL: Issues, https://github.com/humrochagf/wheke/issues Project-URL:
 Source, https://github.com/humrochagf/wheke Author-email: Humberto Rocha
 gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

