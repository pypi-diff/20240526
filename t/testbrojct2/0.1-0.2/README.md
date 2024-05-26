# Comparing `tmp/testbrojct2-0.1.tar.gz` & `tmp/testbrojct2-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testbrojct2-0.1.tar", last modified: Sun May 26 11:51:46 2024, max compression
+gzip compressed data, was "dist\testbrojct2-0.2.tar", last modified: Sun May 26 12:04:19 2024, max compression
```

## Comparing `testbrojct2-0.1.tar` & `testbrojct2-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:51:46.290697 testbrojct2-0.1/
--rw-rw-rw-   0        0        0      337 2024-05-26 11:51:46.289694 testbrojct2-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 11:51:46.274631 testbrojct2-0.1/code/
--rw-rw-rw-   0        0        0      104 2024-05-26 11:50:14.000000 testbrojct2-0.1/code/__init__.py
--rw-rw-rw-   0        0        0     3503 2024-05-25 21:47:44.000000 testbrojct2-0.1/code/dsgsfdgdfg.py
--rw-rw-rw-   0        0        0       42 2024-05-26 11:51:46.291805 testbrojct2-0.1/setup.cfg
--rw-rw-rw-   0        0        0      404 2024-05-26 11:50:48.000000 testbrojct2-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:51:46.287646 testbrojct2-0.1/testbrojct2.egg-info/
--rw-rw-rw-   0        0        0      337 2024-05-26 11:51:46.000000 testbrojct2-0.1/testbrojct2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-26 11:51:46.000000 testbrojct2-0.1/testbrojct2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:51:46.000000 testbrojct2-0.1/testbrojct2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 11:51:46.000000 testbrojct2-0.1/testbrojct2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 11:51:46.000000 testbrojct2-0.1/testbrojct2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 12:04:19.387470 testbrojct2-0.2/
+-rw-rw-rw-   0        0        0      353 2024-05-26 12:04:19.385388 testbrojct2-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 12:04:19.367822 testbrojct2-0.2/code/
+-rw-rw-rw-   0        0        0      122 2024-05-26 12:02:33.000000 testbrojct2-0.2/code/__init__.py
+-rw-rw-rw-   0        0        0     3503 2024-05-25 21:47:44.000000 testbrojct2-0.2/code/dsgsfdgdfg.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 12:03:00.000000 testbrojct2-0.2/code/x.py
+-rw-rw-rw-   0        0        0       42 2024-05-26 12:04:19.387470 testbrojct2-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      421 2024-05-26 12:03:32.000000 testbrojct2-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:04:19.382354 testbrojct2-0.2/testbrojct2.egg-info/
+-rw-rw-rw-   0        0        0      353 2024-05-26 12:04:19.000000 testbrojct2-0.2/testbrojct2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-05-26 12:04:19.000000 testbrojct2-0.2/testbrojct2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 12:04:19.000000 testbrojct2-0.2/testbrojct2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 12:04:19.000000 testbrojct2-0.2/testbrojct2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 12:04:19.000000 testbrojct2-0.2/testbrojct2.egg-info/top_level.txt
```

### Comparing `testbrojct2-0.1/code/dsgsfdgdfg.py` & `testbrojct2-0.2/code/dsgsfdgdfg.py`

 * *Files identical despite different names*

