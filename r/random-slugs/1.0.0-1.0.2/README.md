# Comparing `tmp/random_slugs-1.0.0.tar.gz` & `tmp/random_slugs-1.0.2.tar.gz`

## Comparing `random_slugs-1.0.0.tar` & `random_slugs-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 random_slugs-1.0.0/dev-requirements.txt
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 random_slugs-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 random_slugs-1.0.0/random_slugs/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 random_slugs-1.0.0/random_slugs/generate.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 random_slugs-1.0.0/random_slugs/words.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_slugs-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 random_slugs-1.0.0/tests/test_generate.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 random_slugs-1.0.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_slugs-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 random_slugs-1.0.0/README.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 random_slugs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 random_slugs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 random_slugs-1.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 random_slugs-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 random_slugs-1.0.2/random_slugs/__about__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 random_slugs-1.0.2/random_slugs/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 random_slugs-1.0.2/random_slugs/generate.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 random_slugs-1.0.2/random_slugs/words.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_slugs-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 random_slugs-1.0.2/tests/test_generate.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 random_slugs-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 random_slugs-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 random_slugs-1.0.2/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 random_slugs-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 random_slugs-1.0.2/PKG-INFO
```

### Comparing `random_slugs-1.0.0/random_slugs/generate.py` & `random_slugs-1.0.2/random_slugs/generate.py`

 * *Files identical despite different names*

### Comparing `random_slugs-1.0.0/random_slugs/words.py` & `random_slugs-1.0.2/random_slugs/words.py`

 * *Files identical despite different names*

### Comparing `random_slugs-1.0.0/tests/test_generate.py` & `random_slugs-1.0.2/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `random_slugs-1.0.0/README.md` & `random_slugs-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `random_slugs-1.0.0/pyproject.toml` & `random_slugs-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 [build-system]
 build-backend = "hatchling.build"
-requires = ["hatchling"]
+requires = [
+  "hatchling",
+  "hatch-semver",
+]
 
 [project]
 authors = [{name = "Fabio Kapsahili", email = "fabio.kapsahili@protonmail.com"}]
 description = "A Python package for generating random slugs using a customizable vocabulary of words."
-equires-python = ">=3.8"
+dynamic = [
+  "version",
+]
 keywords = ["sample", "setuptools", "development"]
 license = {file = "LICENSE.txt"}
 maintainers = [
   {name = "Fabio Kapsahili", email = "fabio.kapsahili@protonmail.com"},
 ]
 name = "random-slugs"
 readme = "README.md"
-version = "1.0.0"
+requires-python = ">=3.9"
 
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
-dependencies = ["peppercorn"]
+dependencies = []
 
 [project.optional-dependencies]
 dev = ["check-manifest"]
 test = ["coverage"]
 
 [project.urls]
 "Bug Reports" = "https://github.com/fkapsahili/random-slugs/issues"
 "Homepage" = "https://github.com/fkapsahili/random-slugs"
 "Source" = "https://github.com/fkapsahili/random-slugs/"
 
 [tool.hatch]
 package-data = {"random-slugs" = ["*.txt"]}
 
+[tool.hatch.version]
+path = "random_slugs/__about__.py"
+scheme = "semver"
+validate-bump = true
+
 [tool.hatch.envs.test]
 dependencies = [
   "pytest",
 ]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
@@ -69,7 +78,35 @@
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["ANN"]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_level = "DEBUG"
+
+[tool.semantic_release]
+allow_zero_version = false
+commit_message = "chore(release): release v{version} [skip ci]"
+remove_dist = true
+tag_format = "v{version}"
+version_variables = ["random_slugs/__about__.py:__version__"]
+
+[tool.semantic_release.commit_parser_options]
+allowed_tags = [
+  "build",
+  "chore",
+  "ci",
+  "docs",
+  "feat",
+  "fix",
+  "perf",
+  "style",
+  "refactor",
+  "test",
+]
+major_tags = ["feat!"]
+minor_tags = ["feat"]
+patch_tags = ["fix", "perf", "docs", "style", "refactor", "test", "chore", "ci", "build"]
+
+[tool.semantic_release.branches.main]
+match = '(master|main)'
+prerelease = false
```

### Comparing `random_slugs-1.0.0/PKG-INFO` & `random_slugs-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 Metadata-Version: 2.3
 Name: random-slugs
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python package for generating random slugs using a customizable vocabulary of words.
 Project-URL: Bug Reports, https://github.com/fkapsahili/random-slugs/issues
 Project-URL: Homepage, https://github.com/fkapsahili/random-slugs
 Project-URL: Source, https://github.com/fkapsahili/random-slugs/
 Author-email: Fabio Kapsahili <fabio.kapsahili@protonmail.com>
 Maintainer-email: Fabio Kapsahili <fabio.kapsahili@protonmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2024 Fabio Kapsahili
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
 License-File: LICENSE.txt
 Keywords: development,sample,setuptools
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: peppercorn
+Requires-Python: >=3.9
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Random Slugs
```

