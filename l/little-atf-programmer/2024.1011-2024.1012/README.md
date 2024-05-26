# Comparing `tmp/little_atf_programmer-2024.1011.tar.gz` & `tmp/little_atf_programmer-2024.1012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "little_atf_programmer-2024.1011.tar", last modified: Fri May 24 21:43:13 2024, max compression
+gzip compressed data, was "little_atf_programmer-2024.1012.tar", last modified: Sun May 26 12:22:43 2024, max compression
```

## Comparing `little_atf_programmer-2024.1011.tar` & `little_atf_programmer-2024.1012.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.703222 little_atf_programmer-2024.1011/
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-24 21:43:13.703222 little_atf_programmer-2024.1011/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:43:13.703222 little_atf_programmer-2024.1011/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.699222 little_atf_programmer-2024.1011/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.699222 little_atf_programmer-2024.1011/src/atfu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.699222 little_atf_programmer-2024.1011/src/atfu/converter/
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/fuseconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/jed2svf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/jesd3.py
--rw-r--r--   0 runner    (1001) docker     (127)    31144 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/svf2xsvf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/converter/svfeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/erase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.699222 little_atf_programmer-2024.1011/src/atfu/little_board/
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/little_board/jtag_programmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/programmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.703222 little_atf_programmer-2024.1011/src/atfu/standard_vectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-24 21:42:58.000000 little_atf_programmer-2024.1011/src/atfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:43:13.703222 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 21:43:13.000000 little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.722056 little_atf_programmer-2024.1012/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 12:22:43.722056 little_atf_programmer-2024.1012/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/fuseconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/jed2svf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/jesd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31144 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/svf2xsvf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/svfeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/erase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/little_board/
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/little_board/jtag_programmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/programmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/src/atfu/standard_vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/top_level.txt
```

### Comparing `little_atf_programmer-2024.1011/LICENSE.md` & `little_atf_programmer-2024.1012/LICENSE.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/PKG-INFO` & `little_atf_programmer-2024.1012/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1011
+Version: 2024.1012
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

### Comparing `little_atf_programmer-2024.1011/README.md` & `little_atf_programmer-2024.1012/README.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/pyproject.toml` & `little_atf_programmer-2024.1012/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "little-atf-programmer"
-version = "2024.1011"
+version = "2024.1012"
 description = "Little ATF150x Programmer Board utility programs"
 readme = "README.md"
 authors = [{ name = "The Really Old-School Company Limited", email = "info@rosco-m68k.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -34,15 +34,15 @@
 [project.urls]
 Homepage = "https://github.com/roscopeco/atfprog-tools"
 
 [tool.setuptools.package-data]
 "atfu.standard_vectors" = ["*.xsvf"]
 
 [tool.bumpver]
-current_version = "2024.1011"
+current_version = "2024.1012"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `little_atf_programmer-2024.1011/src/atfu/check.py` & `little_atf_programmer-2024.1012/src/atfu/check.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/command.py` & `little_atf_programmer-2024.1012/src/atfu/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import atfu.program
 import atfu.erase
 import atfu.check
 import atfu.programmer
 
 BOARDNAME = "Little ATF150x Programmer Board"
 PROGNAME = f"{BOARDNAME} Utility"
-VERSION = "2024.1011"
+VERSION = "2024.1012"
 
 
 def main():
     args = _arg_parser().parse_args()
     args.func(args)
```

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/device.py` & `little_atf_programmer-2024.1012/src/atfu/converter/device.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/fuseconv.py` & `little_atf_programmer-2024.1012/src/atfu/converter/fuseconv.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/jed2svf.py` & `little_atf_programmer-2024.1012/src/atfu/converter/jed2svf.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/jesd3.py` & `little_atf_programmer-2024.1012/src/atfu/converter/jesd3.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/svf2xsvf.py` & `little_atf_programmer-2024.1012/src/atfu/converter/svf2xsvf.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/converter/svfeventhandler.py` & `little_atf_programmer-2024.1012/src/atfu/converter/svfeventhandler.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/erase.py` & `little_atf_programmer-2024.1012/src/atfu/erase.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/little_board/jtag_programmer.py` & `little_atf_programmer-2024.1012/src/atfu/little_board/jtag_programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/output.py` & `little_atf_programmer-2024.1012/src/atfu/output.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/program.py` & `little_atf_programmer-2024.1012/src/atfu/program.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,10 +51,15 @@
     return jed2svf(device=device, infile=file, output=output)
 
 
 def _process_input_svf(output: Output, file: io.BufferedReader) -> io.BufferedReader:
     with file:  # ensure this stays open until we're done so it doesn't get deleted...
         # Bit of weirdness here, the underlying code needs the file to be text...
         inname = file.name
-        infile = open(inname, "r")
+
+        try:
+            infile = open(inname, "r")
+        except PermissionError:
+            # _Probably_ on Windows, where it doesn't matter anyway...
+            infile = file
 
         return svf2xsvf(output=output, infile=infile)
```

### Comparing `little_atf_programmer-2024.1011/src/atfu/programmer.py` & `little_atf_programmer-2024.1012/src/atfu/programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/__init__.py` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/__init__.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1502.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1504.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/bc1508.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1502.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1504.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/atfu/standard_vectors/e1508.xsvf` & `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/PKG-INFO` & `little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1011
+Version: 2024.1012
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

### Comparing `little_atf_programmer-2024.1011/src/little_atf_programmer.egg-info/SOURCES.txt` & `little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

