# Comparing `tmp/aioreqs-1.0.0.tar.gz` & `tmp/aioreqs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioreqs-1.0.0.tar", max compression
+gzip compressed data, was "aioreqs-1.0.1.tar", max compression
```

## Comparing `aioreqs-1.0.0.tar` & `aioreqs-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     3591 2024-05-26 21:15:33.559438 aioreqs-1.0.0/aioreqs/__init__.py
--rw-r--r--   0        0        0      316 2024-05-26 21:16:34.278462 aioreqs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 21:16:45.746607 aioreqs-1.0.0/README.md
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 aioreqs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2384 2024-05-26 21:21:29.286601 aioreqs-1.0.1/aioreqs/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-26 21:19:57.298419 aioreqs-1.0.1/aioreqs/async/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-26 21:21:48.579151 aioreqs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-26 21:16:45.746607 aioreqs-1.0.1/README.md
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 aioreqs-1.0.1/PKG-INFO
```

### Comparing `aioreqs-1.0.0/aioreqs/__init__.py` & `aioreqs-1.0.1/aioreqs/async/__init__.py`

 * *Files identical despite different names*

