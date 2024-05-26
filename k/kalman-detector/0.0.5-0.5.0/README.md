# Comparing `tmp/kalman_detector-0.0.5.tar.gz` & `tmp/kalman_detector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kalman_detector-0.0.5.tar", last modified: Sun Sep 15 15:51:32 2019, max compression
+gzip compressed data, was "kalman_detector-0.5.0.tar", last modified: Sun May 26 16:27:11 2024, max compression
```

## Comparing `kalman_detector-0.0.5.tar` & `kalman_detector-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,24 @@
-drwxr-xr-x   0 bzackay    (501) staff       (20)        0 2019-09-15 15:51:32.000000 kalman_detector-0.0.5/
--rw-r--r--   0 bzackay    (501) staff       (20)     1124 2019-09-15 15:51:32.000000 kalman_detector-0.0.5/PKG-INFO
--rw-r--r--   0 bzackay    (501) staff       (20)     1140 2019-09-15 15:48:46.000000 kalman_detector-0.0.5/setup.py
-drwxr-xr-x   0 bzackay    (501) staff       (20)        0 2019-09-15 15:51:32.000000 kalman_detector-0.0.5/kalman_detector/
--rw-r--r--   0 bzackay    (501) staff       (20)     3732 2019-08-24 22:50:33.000000 kalman_detector-0.0.5/kalman_detector/test_kalman_detector.py
--rw-r--r--   0 bzackay    (501) staff       (20)       30 2018-08-15 02:06:30.000000 kalman_detector-0.0.5/kalman_detector/__init__.py
--rw-r--r--   0 bzackay    (501) staff       (20)     4388 2019-08-28 19:13:12.000000 kalman_detector-0.0.5/kalman_detector/create_figures.py
--rw-r--r--   0 bzackay    (501) staff       (20)    15285 2019-09-15 15:23:59.000000 kalman_detector-0.0.5/kalman_detector/kalman_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:27:11.219080 kalman_detector-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-26 16:27:11.219080 kalman_detector-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:27:11.215080 kalman_detector-0.5.0/kalman_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16202 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/kalman_detector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:27:11.219080 kalman_detector-0.5.0/kalman_detector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-26 16:27:11.000000 kalman_detector-0.5.0/kalman_detector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-26 16:27:11.000000 kalman_detector-0.5.0/kalman_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 16:27:11.000000 kalman_detector-0.5.0/kalman_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-26 16:27:11.000000 kalman_detector-0.5.0/kalman_detector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 16:27:11.000000 kalman_detector-0.5.0/kalman_detector.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2419 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 16:27:11.219080 kalman_detector-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:27:11.219080 kalman_detector-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/tests/test_kalman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/tests/test_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-26 16:27:03.000000 kalman_detector-0.5.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

