# Comparing `tmp/annonition-0.0.9.tar.gz` & `tmp/annonition-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.0.9.tar", last modified: Sun May 19 22:20:52 2024, max compression
+gzip compressed data, was "annonition-0.1.0.tar", last modified: Sun May 26 00:10:08 2024, max compression
```

## Comparing `annonition-0.0.9.tar` & `annonition-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.360000 annonition-0.0.9/
--rw-rw-rw-   0        0        0      452 2024-05-19 22:20:54.000000 annonition-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.390000 annonition-0.0.9/annonition/
--rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.9/annonition/__init__.py
--rw-rw-rw-   0        0        0     5352 2024-05-19 22:20:16.000000 annonition-0.0.9/annonition/logger.py
--rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.9/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.410000 annonition-0.0.9/annonition.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 22:20:54.000000 annonition-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      843 2024-05-19 22:20:32.000000 annonition-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:10:08.480000 annonition-0.1.0/
+-rw-rw-rw-   0        0        0     2911 2024-05-26 00:10:10.000000 annonition-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2541 2024-05-26 00:07:52.000000 annonition-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 00:10:08.510000 annonition-0.1.0/annonition/
+-rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.1.0/annonition/__init__.py
+-rw-rw-rw-   0        0        0     9895 2024-05-26 00:02:42.000000 annonition-0.1.0/annonition/logger.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.1.0/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:10:08.530000 annonition-0.1.0/annonition.egg-info/
+-rw-rw-rw-   0        0        0     2911 2024-05-26 00:10:10.000000 annonition-0.1.0/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-26 00:10:10.000000 annonition-0.1.0/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 00:10:10.000000 annonition-0.1.0/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-26 00:10:10.000000 annonition-0.1.0/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 00:10:10.000000 annonition-0.1.0/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 00:10:10.000000 annonition-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-05-26 00:09:28.000000 annonition-0.1.0/setup.py
```

