# Comparing `tmp/python-fasthtml-0.0.1.tar.gz` & `tmp/python-fasthtml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fasthtml-0.0.1.tar", last modified: Sun May 26 01:39:09 2024, max compression
+gzip compressed data, was "python-fasthtml-0.0.2.tar", last modified: Fri May 17 08:05:44 2024, max compression
```

## Comparing `python-fasthtml-0.0.1.tar` & `python-fasthtml-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:39:09.200302 python-fasthtml-0.0.1/
--rw-rw-r--   0 jhoward    (501) staff       (20)    11337 2023-04-27 10:12:58.000000 python-fasthtml-0.0.1/LICENSE
--rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 python-fasthtml-0.0.1/MANIFEST.in
--rw-r--r--   0 jhoward    (501) staff       (20)     2771 2024-05-26 01:39:09.200111 python-fasthtml-0.0.1/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)     1917 2024-05-26 01:36:26.000000 python-fasthtml-0.0.1/README.md
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:39:09.198824 python-fasthtml-0.0.1/fastsql/
--rw-r--r--   0 jhoward    (501) staff       (20)       43 2024-05-26 01:21:51.000000 python-fasthtml-0.0.1/fastsql/__init__.py
--rw-r--r--   0 jhoward    (501) staff       (20)     1355 2024-05-26 01:21:51.000000 python-fasthtml-0.0.1/fastsql/_modidx.py
--rw-r--r--   0 jhoward    (501) staff       (20)     2293 2024-05-26 01:21:51.000000 python-fasthtml-0.0.1/fastsql/core.py
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:39:09.199874 python-fasthtml-0.0.1/python_fasthtml.egg-info/
--rw-r--r--   0 jhoward    (501) staff       (20)     2771 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)      380 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/SOURCES.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/dependency_links.txt
--rw-r--r--   0 jhoward    (501) staff       (20)       36 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/entry_points.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-26 01:11:06.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/not-zip-safe
--rw-r--r--   0 jhoward    (501) staff       (20)       30 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/requires.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        8 2024-05-26 01:39:09.000000 python-fasthtml-0.0.1/python_fasthtml.egg-info/top_level.txt
--rw-r--r--   0 jhoward    (501) staff       (20)      879 2024-05-26 01:08:00.000000 python-fasthtml-0.0.1/settings.ini
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-26 01:39:09.200346 python-fasthtml-0.0.1/setup.cfg
--rw-r--r--   0 jhoward    (501) staff       (20)     2608 2024-05-26 01:11:25.000000 python-fasthtml-0.0.1/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.979245 python-fasthtml-0.0.2/
+-rw-r--r--   0 jhoward    (501) staff       (20)    11357 2024-05-17 05:17:01.000000 python-fasthtml-0.0.2/LICENSE
+-rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 python-fasthtml-0.0.2/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)     3563 2024-05-17 08:05:44.979055 python-fasthtml-0.0.2/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     2762 2024-05-17 08:05:22.000000 python-fasthtml-0.0.2/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.977881 python-fasthtml-0.0.2/fasthtml/
+-rw-r--r--   0 jhoward    (501) staff       (20)       43 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1990 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4228 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/core.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.978735 python-fasthtml-0.0.2/python_fasthtml.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)     3563 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)      383 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/entry_points.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-17 05:43:33.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)       56 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        9 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      893 2024-05-17 08:05:08.000000 python-fasthtml-0.0.2/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-17 08:05:44.979294 python-fasthtml-0.0.2/setup.cfg
+-rw-rw-r--   0 jhoward    (501) staff       (20)     2598 2024-05-17 05:43:20.000000 python-fasthtml-0.0.2/setup.py
```

### Comparing `python-fasthtml-0.0.1/LICENSE` & `python-fasthtml-0.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022, fastai
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `python-fasthtml-0.0.1/setup.py` & `python-fasthtml-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
     'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10 3.11 3.12'.split()
+py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
 
 requirements = shlex.split(cfg.get('requirements', ''))
 if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
```

