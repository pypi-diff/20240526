# Comparing `tmp/pip2deb-1.2.tar.gz` & `tmp/pip2deb-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2deb-1.2.tar", last modified: Sun May 26 17:25:16 2024, max compression
+gzip compressed data, was "pip2deb-1.3.tar", last modified: Sun May 26 20:13:52 2024, max compression
```

## Comparing `pip2deb-1.2.tar` & `pip2deb-1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 17:25:16.669480 pip2deb-1.2/
--rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 17:25:16.669480 pip2deb-1.2/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      146 2024-05-26 11:26:10.000000 pip2deb-1.2/README.rst
--rwxr-xr-x   0 whoami    (1002) whoami    (1002)     1813 2024-05-26 17:24:21.000000 pip2deb-1.2/pip2deb
-drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 17:25:16.669480 pip2deb-1.2/pip2deb.egg-info/
--rw-r--r--   0 whoami    (1002) whoami    (1002)      911 2024-05-26 17:25:16.000000 pip2deb-1.2/pip2deb.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (1002) whoami    (1002)      151 2024-05-26 17:25:16.000000 pip2deb-1.2/pip2deb.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 17:25:16.000000 pip2deb-1.2/pip2deb.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 17:25:16.000000 pip2deb-1.2/pip2deb.egg-info/top_level.txt
--rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 17:25:16.669480 pip2deb-1.2/setup.cfg
--rw-r--r--   0 whoami    (1002) whoami    (1002)     1009 2024-05-26 17:24:38.000000 pip2deb-1.2/setup.py
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 20:13:51.996651 pip2deb-1.3/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     3397 2024-05-26 20:11:06.000000 pip2deb-1.3/LICENSE
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 20:13:51.996651 pip2deb-1.3/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      976 2024-05-26 20:09:37.000000 pip2deb-1.3/README.rst
+-rwxr-xr-x   0 whoami    (1002) whoami    (1002)     2518 2024-05-26 19:58:08.000000 pip2deb-1.3/pip2deb
+drwxr-xr-x   0 whoami    (1002) whoami    (1002)        0 2024-05-26 20:13:51.996651 pip2deb-1.3/pip2deb.egg-info/
+-rw-r--r--   0 whoami    (1002) whoami    (1002)     1415 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      159 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)        1 2024-05-26 20:13:51.000000 pip2deb-1.3/pip2deb.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (1002) whoami    (1002)       38 2024-05-26 20:13:51.996651 pip2deb-1.3/setup.cfg
+-rw-r--r--   0 whoami    (1002) whoami    (1002)      788 2024-05-26 20:13:43.000000 pip2deb-1.3/setup.py
```

