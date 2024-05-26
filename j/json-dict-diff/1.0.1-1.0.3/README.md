# Comparing `tmp/json_dict_diff-1.0.1.tar.gz` & `tmp/json_dict_diff-1.0.3.tar.gz`

## Comparing `json_dict_diff-1.0.1.tar` & `json_dict_diff-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/build.sh
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/json_dict_diff.py
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/upload.sh
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/tests/test.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/LICENCE
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 json_dict_diff-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/build.sh
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/json_dict_diff.py
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/upload.sh
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/tests/test.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/LICENCE
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/README.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 json_dict_diff-1.0.3/PKG-INFO
```

### Comparing `json_dict_diff-1.0.1/json_dict_diff.py` & `json_dict_diff-1.0.3/json_dict_diff.py`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.1/.github/workflows/test.yaml` & `json_dict_diff-1.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.1/LICENCE` & `json_dict_diff-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `json_dict_diff-1.0.1/README.md` & `json_dict_diff-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Json Dict Diff
 
-Library for creating a minimal diff of two json-compatible python dictionaries.
+Library for creating a minimal diff of two json-compatible Python dictionaries.
 
-This library can be used to compare two json-compatible python dictionaries (i.e. dictionaries/lists/... containing only the following primitives: `int, float, str, list, dict, set, tuple, bool`) and generates a "minimal" diff.
-The diff is represented as a dictionary where insertions/deletions/substititons are represented as tuples.
-E.g the following two dictionaries:
+This library can be used to compare two json-compatible Python dictionaries (i.e. dictionaries, lists, ... containing only the following primitives: `int`, `float`, `str`, `list`, `dict`, `set`, `tuple`, `bool`) and generates a "minimal" diff.
+The diff is represented as a dictionary where insertions/deletions/substitutions are represented as tuples.
+For example the following two dictionaries:
 
 ```py
 diff(
   { "a": [ { "b": 1, "c": True }, 1.0, "x" ], "d": 1 },
   { "a": [ { "b": 2, "c": True }, 1.0, "y", True ] }
 )
 ```
@@ -16,22 +16,22 @@
 will result in the following diff:
 
 ```py
 { "a": [ { "b": (1, 2) }, ("x", "y"), (None, True) ], "d": (1, None) }
 ```
 
 Here the tuples `(1, 2), ("x", "y"), (None, True), (1, None)` represent the substitions that happened.
-`None` implies that a object was either removed or added.
+`None` implies that an object was either removed or added.
 
 If there is no diff (e.g.: `diff({ "a": 1 }, { "a": 1 })`) the result will be `None`. In this sense,
 the library can also be used to compare two json-compatible dictionaries.
 
 ---
 
-If a object of any different type is used anywhere in a dict/list/..., a `ValidationException` will be raised.
+If an object of any other type is used in a dict, list, ..., a `ValidationException` will be raised.
 
 ## Exports
 
 ```py
 JDict = Union[int, float, str, List["Result"], Dict[str, "Result"], Tuple["Result"], Set["Result"], None]
 
 class ValidationException
@@ -39,41 +39,41 @@
 def validate(a: JDict):
 
 def diff(a: JDict, b: JDict) -> JDict:
 ```
 
 ## Notes
 
-Primitive objects such as ints/floats/... can also be diffed which will result in a single tuple of a substition.
-E.g:
+Primitive objects such as ints, floats, ... can also be diffed which will result in a single tuple of a substition.
+For example:
 
 ```py
 diff("a", "b") == ("a", "b")
 diff("a", "a") is None
 ```
 
 ---
 
-The diff will treat lists, sets and tuples as lists which means that the result will contain lists instead of sets or tuples.
+The diff will treat lists, sets and tuples as lists, which means that the result will contain lists instead of sets or tuples.
 This is due to tuples being reserved for the substitution results.
 
 ---
 
-If it might not be clear which element in a list might be substituted, this library makes no guarantees on the actual substitution. E.g:
+If it is not clear which element in a list might be substituted this library makes no guarantees on the actual substitution.
+For example:
 
 ```py
 diff([1, 2, 3], [1, 4, 5])
 ```
 
 can result either in: `[ (2, 4), (3, 5) ]` or `[ (3, 4), (2, 5) ]`.
 
 ---
 
-`None` elements might or might not show up as a diff
-
-E.g:
+`None` elements might or might not show up as a diff.
+For example:
 
 ```py
 diff([ None, 1 ], [1])
 ```
 
 might result in `[ (None, 1) ]` or `None` (i.e. no diff).
```

### Comparing `json_dict_diff-1.0.1/pyproject.toml` & `json_dict_diff-1.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "json_dict_diff"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
   { name="Gerrit Proessl", email="gerrit.proessl@gmail.com" },
 ]
 description = "A simple library to create a minimal diff of two json compatible dictionaries"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `json_dict_diff-1.0.1/PKG-INFO` & `json_dict_diff-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.3
 Name: json_dict_diff
-Version: 1.0.1
+Version: 1.0.3
 Summary: A simple library to create a minimal diff of two json compatible dictionaries
 Project-URL: Homepage, https://github.com/g3rrit/json_dict_diff
 Project-URL: Issues, https://github.com/g3rrit/json_dict_diff/issues
 Author-email: Gerrit Proessl <gerrit.proessl@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Json Dict Diff
 
-Library for creating a minimal diff of two json-compatible python dictionaries.
+Library for creating a minimal diff of two json-compatible Python dictionaries.
 
-This library can be used to compare two json-compatible python dictionaries (i.e. dictionaries/lists/... containing only the following primitives: `int, float, str, list, dict, set, tuple, bool`) and generates a "minimal" diff.
-The diff is represented as a dictionary where insertions/deletions/substititons are represented as tuples.
-E.g the following two dictionaries:
+This library can be used to compare two json-compatible Python dictionaries (i.e. dictionaries, lists, ... containing only the following primitives: `int`, `float`, `str`, `list`, `dict`, `set`, `tuple`, `bool`) and generates a "minimal" diff.
+The diff is represented as a dictionary where insertions/deletions/substitutions are represented as tuples.
+For example the following two dictionaries:
 
 ```py
 diff(
   { "a": [ { "b": 1, "c": True }, 1.0, "x" ], "d": 1 },
   { "a": [ { "b": 2, "c": True }, 1.0, "y", True ] }
 )
 ```
@@ -30,22 +30,22 @@
 will result in the following diff:
 
 ```py
 { "a": [ { "b": (1, 2) }, ("x", "y"), (None, True) ], "d": (1, None) }
 ```
 
 Here the tuples `(1, 2), ("x", "y"), (None, True), (1, None)` represent the substitions that happened.
-`None` implies that a object was either removed or added.
+`None` implies that an object was either removed or added.
 
 If there is no diff (e.g.: `diff({ "a": 1 }, { "a": 1 })`) the result will be `None`. In this sense,
 the library can also be used to compare two json-compatible dictionaries.
 
 ---
 
-If a object of any different type is used anywhere in a dict/list/..., a `ValidationException` will be raised.
+If an object of any other type is used in a dict, list, ..., a `ValidationException` will be raised.
 
 ## Exports
 
 ```py
 JDict = Union[int, float, str, List["Result"], Dict[str, "Result"], Tuple["Result"], Set["Result"], None]
 
 class ValidationException
@@ -53,41 +53,41 @@
 def validate(a: JDict):
 
 def diff(a: JDict, b: JDict) -> JDict:
 ```
 
 ## Notes
 
-Primitive objects such as ints/floats/... can also be diffed which will result in a single tuple of a substition.
-E.g:
+Primitive objects such as ints, floats, ... can also be diffed which will result in a single tuple of a substition.
+For example:
 
 ```py
 diff("a", "b") == ("a", "b")
 diff("a", "a") is None
 ```
 
 ---
 
-The diff will treat lists, sets and tuples as lists which means that the result will contain lists instead of sets or tuples.
+The diff will treat lists, sets and tuples as lists, which means that the result will contain lists instead of sets or tuples.
 This is due to tuples being reserved for the substitution results.
 
 ---
 
-If it might not be clear which element in a list might be substituted, this library makes no guarantees on the actual substitution. E.g:
+If it is not clear which element in a list might be substituted this library makes no guarantees on the actual substitution.
+For example:
 
 ```py
 diff([1, 2, 3], [1, 4, 5])
 ```
 
 can result either in: `[ (2, 4), (3, 5) ]` or `[ (3, 4), (2, 5) ]`.
 
 ---
 
-`None` elements might or might not show up as a diff
-
-E.g:
+`None` elements might or might not show up as a diff.
+For example:
 
 ```py
 diff([ None, 1 ], [1])
 ```
 
 might result in `[ (None, 1) ]` or `None` (i.e. no diff).
```

