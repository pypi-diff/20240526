# Comparing `tmp/class_cache-0.0.1.tar.gz` & `tmp/class_cache-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.0.1.tar` & `class_cache-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0     1070 2024-01-16 02:08:00.803203 class_cache-0.0.1/LICENSE
--rw-r--r--   0        0        0       12 2024-01-16 02:07:27.695225 class_cache-0.0.1/README.md
--rw-r--r--   0        0        0       64 2024-01-16 02:07:02.663238 class_cache-0.0.1/class_cache/__init__.py
--rw-r--r--   0        0        0     2101 2024-01-16 02:09:20.635130 class_cache-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 class_cache-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      993 2024-05-26 18:56:24.079492 class_cache-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-26 18:56:24.079492 class_cache-0.1.0/LICENSE
+-rw-r--r--   0        0        0       12 2024-05-26 18:56:24.083492 class_cache-0.1.0/README.md
+-rw-r--r--   0        0        0      123 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/__init__.py
+-rw-r--r--   0        0        0     3981 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/backends.py
+-rw-r--r--   0        0        0     2523 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/types.py
+-rw-r--r--   0        0        0      225 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/utils.py
+-rw-r--r--   0        0        0     2278 2024-05-26 18:56:24.083492 class_cache-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 class_cache-0.1.0/PKG-INFO
```

### Comparing `class_cache-0.0.1/LICENSE` & `class_cache-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.0.1/pyproject.toml` & `class_cache-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 [project]
 name = "class-cache"
 maintainers = [{ name = "Artem Vasenin", email = "vasart169@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["description", "version"]
-dependencies = []
+dependencies = ["Pympler", "replete", "marisa-trie"]
 
 [project.urls]
 Home = "https://github.com/Rizhiy/class-cache"
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-cov"]
+test = ["pytest", "pytest-cov", "replete[testing]"]
 dev = ["black", "class-cache[test]", "ruff"]
 
 [tool.flit.sdist]
 include = ["README.md"]
 exclude = [".github", ".gitignore", "tests/*"]
 
 [tool.semantic_release]
@@ -27,15 +27,15 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules"
 
 [tool.black]
 line-length = 120
-skip-magic-trailing-comma = true
+# skip-magic-trailing-comma = true
 
 [tool.yamlfix]
 line_length = 120
 section_whitelines = 1
 
 [tool.pyright]
 strictParameterNoneValue = false
@@ -43,81 +43,81 @@
 
 [tool.ruff]
 target-version = "py39"
 line-length = 120
 [tool.ruff.lint]
 preview = true
 select = [
-  "A",
-  "ARG",
-  "B",
-  "BLE",
-  "C4",
-  "COM",
-  "E",
-  "ERA",
-  "F",
-  "FBT",
-  "FIX",
-  "FLY",
-  "FURB",
-  "I",
-  "IC",
-  "INP",
-  "ISC",
-  "LOG",
-  "N",
-  "NPY",
-  "PERF",
-  "PIE",
-  "PT",
-  "PTH",
-  "Q",
-  "R",
-  "RET",
-  "RSE",
-  "S",
-  "SIM",
-  "SLF",
-  "T20",
-  "TCH",
-  "TD",
-  "TID",
-  "TRY",
-  "UP",
-  "W",
+    "A",
+    "ARG",
+    "B",
+    "BLE",
+    "C4",
+    "COM",
+    "E",
+    "ERA",
+    "F",
+    "FBT",
+    "FIX",
+    "FLY",
+    "FURB",
+    "I",
+    "IC",
+    "INP",
+    "ISC",
+    "LOG",
+    "N",
+    "NPY",
+    "PERF",
+    "PIE",
+    "PT",
+    "PTH",
+    "Q",
+    "R",
+    "RET",
+    "RSE",
+    "S",
+    "SIM",
+    "SLF",
+    "T20",
+    "TCH",
+    "TD",
+    "TID",
+    "TRY",
+    "UP",
+    "W",
 ]
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 ignore = [
-  "A003",
-  "E203",
-  "FIX002",
-  "FURB113",
-  "N817",
-  "PTH123",
-  "RET503",
-  "S113",
-  "TD002",
-  "TD003",
-  "TRY003",
-  "UP007",
-  "UP035",
+    "A003",
+    "E203",
+    "FIX002",
+    "FURB113",
+    "N817",
+    "PTH123",
+    "RET503",
+    "S113",
+    "TD002",
+    "TD003",
+    "TRY003",
+    "UP007",
+    "UP035",
 ]
 [tool.ruff.per-file-ignores]
 "**/__init__.py" = [
-  "F401", # Allow unused imports in module files
+    "F401", # Allow unused imports in module files
 ]
 "tests/**/*.py" = [
-  "E501",   # Test strings can be long
-  "S101",   # Asserts in tests are fine
-  "T201",   # Prints are useful for debugging
-  "TCH001",
-  "TCH002",
-  "TCH003", # Tests don't need to be super performant, prefer simpler code
+    "E501",   # Test strings can be long
+    "S101",   # Asserts in tests are fine
+    "T201",   # Prints are useful for debugging
+    "TCH001",
+    "TCH002",
+    "TCH003", # Tests don't need to be super performant, prefer simpler code
 ]
 "tests/pickle.py" = [
-  "S301", # Testing pickle so have to use it
+    "S301", # Testing pickle so have to use it
 ]
 "tests/data/**/*.py" = [
-  "TID252", # Have to use relative imports in configs
+    "TID252", # Have to use relative imports in configs
 ]
```

