# Comparing `tmp/ops-py-cert-report-1.0.1.tar.gz` & `tmp/ops_py_cert_report-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-cert-report-1.0.1.tar", last modified: Sun Feb 11 13:47:24 2024, max compression
+gzip compressed data, was "ops_py_cert_report-2.0.0.tar", last modified: Sun May 26 19:30:44 2024, max compression
```

## Comparing `ops-py-cert-report-1.0.1.tar` & `ops_py_cert_report-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:47:24.420529 ops-py-cert-report-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-11 13:47:17.000000 ops-py-cert-report-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-11 13:47:24.420529 ops-py-cert-report-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-11 13:47:17.000000 ops-py-cert-report-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:47:24.420529 ops-py-cert-report-1.0.1/cert_report/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-11 13:47:12.000000 ops-py-cert-report-1.0.1/cert_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-02-11 13:47:12.000000 ops-py-cert-report-1.0.1/cert_report/cert_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 13:47:24.420529 ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-11 13:47:24.000000 ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-11 13:47:24.000000 ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 13:47:24.000000 ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-11 13:47:24.000000 ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-11 13:47:17.000000 ops-py-cert-report-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 13:47:24.420529 ops-py-cert-report-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-11 13:47:17.000000 ops-py-cert-report-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:30:44.683704 ops_py_cert_report-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-26 19:30:41.000000 ops_py_cert_report-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-26 19:30:44.683704 ops_py_cert_report-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 19:30:41.000000 ops_py_cert_report-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:30:44.683704 ops_py_cert_report-2.0.0/cert_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-26 19:30:35.000000 ops_py_cert_report-2.0.0/cert_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-26 19:30:35.000000 ops_py_cert_report-2.0.0/cert_report/cert_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-26 19:30:35.000000 ops_py_cert_report-2.0.0/cert_report/slack_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:30:44.683704 ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-26 19:30:44.000000 ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-26 19:30:44.000000 ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:30:44.000000 ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 19:30:44.000000 ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-26 19:30:41.000000 ops_py_cert_report-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:30:44.683704 ops_py_cert_report-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-26 19:30:41.000000 ops_py_cert_report-2.0.0/setup.py
```

### Comparing `ops-py-cert-report-1.0.1/LICENSE` & `ops_py_cert_report-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-cert-report-1.0.1/PKG-INFO` & `ops_py_cert_report-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-cert-report
-Version: 1.0.1
+Version: 2.0.0
 Summary: Output a Cert expire report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-cert-report-1.0.1/ops_py_cert_report.egg-info/PKG-INFO` & `ops_py_cert_report-2.0.0/ops_py_cert_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-cert-report
-Version: 1.0.1
+Version: 2.0.0
 Summary: Output a Cert expire report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

