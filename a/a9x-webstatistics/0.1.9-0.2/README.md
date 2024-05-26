# Comparing `tmp/a9x_webstatistics-0.1.9.tar.gz` & `tmp/a9x_webstatistics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.1.9.tar", last modified: Sun May 12 12:56:45 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.2.tar", last modified: Sun May 26 13:59:46 2024, max compression
```

## Comparing `a9x_webstatistics-0.1.9.tar` & `a9x_webstatistics-0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:59:46.894225 a9x_webstatistics-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/gencockpit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/summarizemonth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-05-26 13:59:46.000000 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-26 13:59:46.000000 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:59:46.000000 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 13:59:46.000000 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 13:59:46.000000 a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:59:46.898225 a9x_webstatistics-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-26 13:59:35.000000 a9x_webstatistics-0.2/tests/test_z090_gencockpit010.py
```

### Comparing `a9x_webstatistics-0.1.9/LICENSE` & `a9x_webstatistics-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.9/PKG-INFO` & `a9x_webstatistics-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.9
+Version: 0.2
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.9/README.md` & `a9x_webstatistics-0.2/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.9/setup.py` & `a9x_webstatistics-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.9/src/a9x_webstatistics/main.py` & `a9x_webstatistics-0.2/src/a9x_webstatistics/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import io
 import json
 import re
 import sys
 from datetime import datetime
 from .updatestatistics import upd
+from .summarizemonth import summonth
 from importlib.metadata import version
 import geoip2.database
 
 def parseRec(rec, log_pattern, j, georeader):
     print(str(rec))
     j['records_read_total'] += 1
 
@@ -112,15 +113,15 @@
         (25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])           # 2001:db8:3:4::192.0.2.33  64:ff9b::192.0.2.33 (IPv4-Embedded IPv6 Address)
         )
         )[ ]-[ ]-[ ]\[(?P<dateandtime>\d{2}\/[a-zA-Z]{3}\/\d{4}:\d{2}:\d{2}:\d{2}[ ](\+|\-)\d{4})\][ ]
         ((?P<method>)(\"(GET|POST|HEAD|PUT|DELETE|OPTIONS|PROPFIND))[ ]
         (?P<url>.+)[ ](HTTP\/(1\.1|2\.0)"))[ ]
         (?P<statuscode>\d{3})[ ]
         (?P<bytessent>\d+)[ ]
-        (?P<referer>-|"([^"]+)")[ ]
+        (["](?P<referer>[^"]+)["])[ ]
         (["](?P<useragent>[^"]+)["])
         """,
         flags=re.VERBOSE
     )
     
     # process infile:
     with open(infile,'r') as infile:
@@ -129,15 +130,18 @@
             # skip unrecognized records:
             if not recparsed or recparsed['timestamp'] is None or recparsed['ip'] is None:
                 continue
             # skip already processed data:
             if recparsed['timestamp']  <=  d['timelastrec']:
                 continue
             d, visitIP = upd(d, recparsed, visitIP)
-            
+
+    # summarize previous months
+    d = summonth(d)
+    
     # write updated statistic file:
     with open(statfile, "w") as sf:
        json.dump(d,sf)  
     return 0
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False,
```

### Comparing `a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.2/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.9
+Version: 0.2
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.9/tests/test_main001.py` & `a9x_webstatistics-0.2/tests/test_main001.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.9/tests/test_main010.py` & `a9x_webstatistics-0.2/tests/test_main010.py`

 * *Files identical despite different names*

