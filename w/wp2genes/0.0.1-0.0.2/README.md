# Comparing `tmp/wp2genes-0.0.1.tar.gz` & `tmp/wp2genes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wp2genes-0.0.1.tar", last modified: Sun May 26 17:51:09 2024, max compression
+gzip compressed data, was "wp2genes-0.0.2.tar", last modified: Sun May 26 18:01:02 2024, max compression
```

## Comparing `wp2genes-0.0.1.tar` & `wp2genes-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 17:51:09.253808 wp2genes-0.0.1/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      643 2024-05-26 17:51:09.253808 wp2genes-0.0.1/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      380 2024-05-26 17:37:01.000000 wp2genes-0.0.1/README.md
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 17:51:09.253808 wp2genes-0.0.1/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      532 2024-05-26 17:49:41.000000 wp2genes-0.0.1/setup.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 17:51:09.253808 wp2genes-0.0.1/wp2genes.egg-info/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      643 2024-05-26 17:51:09.000000 wp2genes-0.0.1/wp2genes.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      177 2024-05-26 17:51:09.000000 wp2genes-0.0.1/wp2genes.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 17:51:09.000000 wp2genes-0.0.1/wp2genes.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       24 2024-05-26 17:51:09.000000 wp2genes-0.0.1/wp2genes.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 17:51:09.000000 wp2genes-0.0.1/wp2genes.egg-info/top_level.txt
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:01:02.037704 wp2genes-0.0.2/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      813 2024-05-26 18:01:02.037704 wp2genes-0.0.2/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      380 2024-05-26 17:56:14.000000 wp2genes-0.0.2/README.md
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 18:01:02.037704 wp2genes-0.0.2/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      725 2024-05-26 18:00:27.000000 wp2genes-0.0.2/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:01:02.033704 wp2genes-0.0.2/wp2genes/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 wp2genes-0.0.2/wp2genes/__init__.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1088 2024-05-26 17:26:59.000000 wp2genes-0.0.2/wp2genes/wp2genes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:01:02.037704 wp2genes-0.0.2/wp2genes.egg-info/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      813 2024-05-26 18:01:01.000000 wp2genes-0.0.2/wp2genes.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      219 2024-05-26 18:01:02.000000 wp2genes-0.0.2/wp2genes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 18:01:01.000000 wp2genes-0.0.2/wp2genes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       24 2024-05-26 18:01:01.000000 wp2genes-0.0.2/wp2genes.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-26 18:01:01.000000 wp2genes-0.0.2/wp2genes.egg-info/top_level.txt
```

