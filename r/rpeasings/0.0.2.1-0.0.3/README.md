# Comparing `tmp/rpeasings-0.0.2.1.tar.gz` & `tmp/rpeasings-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpeasings-0.0.2.1.tar", last modified: Mon Aug 14 07:14:35 2023, max compression
+gzip compressed data, was "rpeasings-0.0.3.tar", last modified: Sun May 26 09:41:01 2024, max compression
```

## Comparing `rpeasings-0.0.2.1.tar` & `rpeasings-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-14 07:14:35.116414 rpeasings-0.0.2.1/
--rw-rw-rw-   0        0        0     1342 2023-08-13 13:32:44.000000 rpeasings-0.0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2845 2023-08-14 07:14:35.116414 rpeasings-0.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2217 2023-08-13 15:26:37.000000 rpeasings-0.0.2.1/README.md
--rw-rw-rw-   0        0        0      817 2023-08-14 07:12:30.000000 rpeasings-0.0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-14 07:14:35.117421 rpeasings-0.0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-14 07:14:35.101442 rpeasings-0.0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-14 07:14:35.105288 rpeasings-0.0.2.1/src/rpeasings/
--rw-rw-rw-   0        0        0     6061 2023-08-13 14:32:24.000000 rpeasings-0.0.2.1/src/rpeasings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-14 07:14:35.115121 rpeasings-0.0.2.1/src/rpeasings.egg-info/
--rw-rw-rw-   0        0        0     2845 2023-08-14 07:14:35.000000 rpeasings-0.0.2.1/src/rpeasings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-08-14 07:14:35.000000 rpeasings-0.0.2.1/src/rpeasings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-14 07:14:35.000000 rpeasings-0.0.2.1/src/rpeasings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-14 07:14:35.000000 rpeasings-0.0.2.1/src/rpeasings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-14 07:14:35.115121 rpeasings-0.0.2.1/tests/
--rw-rw-rw-   0        0        0      326 2023-08-13 14:54:35.000000 rpeasings-0.0.2.1/tests/test_FIXME.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:01.280161 rpeasings-0.0.3/
+-rw-rw-rw-   0        0        0     1313 2024-05-26 09:15:21.000000 rpeasings-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2843 2024-05-26 09:41:01.279163 rpeasings-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2024-05-26 09:15:21.000000 rpeasings-0.0.3/README.md
+-rw-rw-rw-   0        0        0      779 2024-05-26 09:35:05.000000 rpeasings-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:41:01.280161 rpeasings-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:01.256222 rpeasings-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:01.260657 rpeasings-0.0.3/src/rpeasings/
+-rw-rw-rw-   0        0        0     6323 2024-05-26 09:24:24.000000 rpeasings-0.0.3/src/rpeasings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:01.279163 rpeasings-0.0.3/src/rpeasings.egg-info/
+-rw-rw-rw-   0        0        0     2843 2024-05-26 09:41:01.000000 rpeasings-0.0.3/src/rpeasings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-26 09:41:01.000000 rpeasings-0.0.3/src/rpeasings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:41:01.000000 rpeasings-0.0.3/src/rpeasings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 09:41:01.000000 rpeasings-0.0.3/src/rpeasings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:01.277162 rpeasings-0.0.3/tests/
+-rw-rw-rw-   0        0        0      314 2024-05-26 09:15:21.000000 rpeasings-0.0.3/tests/test_FIXME.py
```

### Comparing `rpeasings-0.0.2.1/LICENSE` & `rpeasings-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Note: github and pypi want me to add a license, but my "contribution" is
-simply transfering the long existing functions to python syntax.
-
-Credit must go to R. Penner to release the original function set unter
-the BSD and MIT licenses.
-
---
-
-MIT License
-
-Copyright (c) 2023 Michael Lamertz
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Note: github and pypi want me to add a license, but my "contribution" is
+simply transfering the long existing functions to python syntax.
+
+Credit must go to R. Penner to release the original function set unter
+the BSD and MIT licenses.
+
+--
+
+MIT License
+
+Copyright (c) 2023 Michael Lamertz
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `rpeasings-0.0.2.1/PKG-INFO` & `rpeasings-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpeasings
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Robert Penner's easings functions in python
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Project-URL: homepage, https://github.com/dickerdackel/rpeasings
 Project-URL: bugtracker, https://github.com/DickerDackel/rpeasings/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rpeasings-0.0.2.1/README.md` & `rpeasings-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# Robert Penner's Easing Functions
-
-There are a plethora of versions available of these, many of which provide an
-object oriented interface, while most of the original easing functions could
-be simple inline expressions.
-
-This library takes the purely functional approach.  No class instantiation,
-just a function call.
-
-See https://easings.net for a good visualisation of these to chose the right
-one.
-
-## Module contents
-
-With the exception of `null`, `in_expx` and `out_expx`, this is a pure python
-port of "Penner's Easing Functions", based on the js code from
-https://easings.net where you can also see a catalog of them in action to
-chose the right one.
-
-The following functions are included:
-
-    in_back         out_back        in_out_back
-    in_bounce       out_bounce      in_out_bounce
-    in_circ         out_circ        in_out_circ
-    in_cubic        out_cubic       in_out_cubic
-    in_elastic      out_elastic     in_out_elastic
-    in_expo         out_expo        in_out_expo
-    in_quad         out_quad        in_out_quad
-    in_quart        out_quart       in_out_quart
-    in_quint        out_quint       in_out_quint
-    in_sine         out_sine        in_out_sine
-
-Additionally, I added a 'null' function, so easing can be disabled without
-changing the interface in the application.  It's basically a `nop`.
-
-    null(t) -> t
-
-In case you want to control the easing function by user input, the `easings`
-dictionary provides a map from function names to functions, e.g.
-
-    eased = rpeasings.easings['out_elastic']
-
-To use any of the included functions, create a `t` (for 'time') value in the
-range 0-1 from your required range (e.g. `t = current / max`).
-
-Putting this `t` into most(!) easing function, will give you a new 'eased'
-value in the range 0-1.
-
-Note: the following functions over-/undershoot:
-
-    `in_back`     `out_back`     `in_out_back`
-    `in_elastic`  `out_elastic`  `in_out_elastic`
-
-Additionally, you can then put that eased value as input into a `lerp`
-function to add dynamics to an otherwise linear range.
-
-Have fun, once you started using one, you'll probably find usecases for them
-everywhere in your game...
+# Robert Penner's Easing Functions
+
+There are a plethora of versions available of these, many of which provide an
+object oriented interface, while most of the original easing functions could
+be simple inline expressions.
+
+This library takes the purely functional approach.  No class instantiation,
+just a function call.
+
+See https://easings.net for a good visualisation of these to chose the right
+one.
+
+## Module contents
+
+With the exception of `null`, `in_expx` and `out_expx`, this is a pure python
+port of "Penner's Easing Functions", based on the js code from
+https://easings.net where you can also see a catalog of them in action to
+chose the right one.
+
+The following functions are included:
+
+    in_back         out_back        in_out_back
+    in_bounce       out_bounce      in_out_bounce
+    in_circ         out_circ        in_out_circ
+    in_cubic        out_cubic       in_out_cubic
+    in_elastic      out_elastic     in_out_elastic
+    in_expo         out_expo        in_out_expo
+    in_quad         out_quad        in_out_quad
+    in_quart        out_quart       in_out_quart
+    in_quint        out_quint       in_out_quint
+    in_sine         out_sine        in_out_sine
+
+Additionally, I added a 'null' function, so easing can be disabled without
+changing the interface in the application.  It's basically a `nop`.
+
+    null(t) -> t
+
+In case you want to control the easing function by user input, the `easings`
+dictionary provides a map from function names to functions, e.g.
+
+    eased = rpeasings.easings['out_elastic']
+
+To use any of the included functions, create a `t` (for 'time') value in the
+range 0-1 from your required range (e.g. `t = current / max`).
+
+Putting this `t` into most(!) easing function, will give you a new 'eased'
+value in the range 0-1.
+
+Note: the following functions over-/undershoot:
+
+    `in_back`     `out_back`     `in_out_back`
+    `in_elastic`  `out_elastic`  `in_out_elastic`
+
+Additionally, you can then put that eased value as input into a `lerp`
+function to add dynamics to an otherwise linear range.
+
+Have fun, once you started using one, you'll probably find usecases for them
+everywhere in your game...
```

### Comparing `rpeasings-0.0.2.1/pyproject.toml` & `rpeasings-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[project]
-name = "rpeasings"
-description = "Robert Penner's easings functions in python"
-version = "0.0.2.1"
-readme = "README.md"
-
-authors = [
-    { name="Michael Lamertz", email="michael.lamertz@gmail.com" }
-]
-
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Games/Entertainment",
-    "Topic :: Software Development :: Libraries :: pygame",
-]
-
-dependencies = []
-
-[project.scripts]
-
-[project.urls]
-homepage = "https://github.com/dickerdackel/rpeasings"
-bugtracker = "https://github.com/DickerDackel/rpeasings/issues"
-
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.pytest.ini_options]
-addopts = "-rA -s"
-testpaths = [
-    "tests",
-]
-
+[project]
+name = "rpeasings"
+description = "Robert Penner's easings functions in python"
+version = "0.0.3"
+readme = "README.md"
+
+authors = [
+    { name="Michael Lamertz", email="michael.lamertz@gmail.com" }
+]
+
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Games/Entertainment",
+    "Topic :: Software Development :: Libraries :: pygame",
+]
+
+dependencies = []
+
+[project.scripts]
+
+[project.urls]
+homepage = "https://github.com/dickerdackel/rpeasings"
+bugtracker = "https://github.com/DickerDackel/rpeasings/issues"
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.pytest.ini_options]
+addopts = "-rA -s"
+testpaths = [
+    "tests",
+]
+
```

### Comparing `rpeasings-0.0.2.1/src/rpeasings.egg-info/PKG-INFO` & `rpeasings-0.0.3/src/rpeasings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpeasings
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Robert Penner's easings functions in python
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Project-URL: homepage, https://github.com/dickerdackel/rpeasings
 Project-URL: bugtracker, https://github.com/DickerDackel/rpeasings/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

