# Comparing `tmp/hyssop_aiodb-0.0.8.tar.gz` & `tmp/hyssop_aiodb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyssop_aiodb-0.0.8.tar", last modified: Sat Dec 17 21:51:34 2022, max compression
+gzip compressed data, was "hyssop_aiodb-0.0.9.tar", last modified: Sun May 26 01:19:26 2024, max compression
```

## Comparing `hyssop_aiodb-0.0.8.tar` & `hyssop_aiodb-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.809640 hyssop_aiodb-0.0.8/
--rw-rw-rw-   0        0        0     1092 2020-09-24 10:33:22.000000 hyssop_aiodb-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      659 2022-12-17 21:51:34.808639 hyssop_aiodb-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2766 2022-05-21 17:08:57.000000 hyssop_aiodb-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.776639 hyssop_aiodb-0.0.8/hyssop_aiodb/
--rw-rw-rw-   0        0        0      319 2022-12-17 21:50:22.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.797640 hyssop_aiodb-0.0.8/hyssop_aiodb/component/
--rw-rw-rw-   0        0        0      507 2022-06-01 19:16:18.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.805639 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/
--rw-rw-rw-   0        0        0      815 2021-01-08 21:25:26.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/__init__.py
--rw-rw-rw-   0        0        0     4855 2021-01-25 00:06:41.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/component.py
--rw-rw-rw-   0        0        0     1220 2021-02-04 04:38:09.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/constants.py
--rw-rw-rw-   0        0        0      486 2021-02-04 04:35:48.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/local.csv
--rw-rw-rw-   0        0        0    36585 2022-12-17 21:46:49.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/utils.py
--rw-rw-rw-   0        0        0     1255 2022-06-01 19:15:49.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb_mixin.py
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.807642 hyssop_aiodb-0.0.8/hyssop_aiodb/unit_test/
--rw-rw-rw-   0        0        0      462 2020-12-27 05:29:11.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/unit_test/__init__.py
--rw-rw-rw-   0        0        0     5556 2022-12-17 21:45:15.000000 hyssop_aiodb-0.0.8/hyssop_aiodb/unit_test/ut.py
-drwxrwxrwx   0        0        0        0 2022-12-17 21:51:34.795646 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/
--rw-rw-rw-   0        0        0      659 2022-12-17 21:51:34.000000 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2022-12-17 21:51:34.000000 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-17 21:51:34.000000 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-12-17 21:51:34.000000 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-17 21:51:34.000000 hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-17 21:51:34.809640 hyssop_aiodb-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1540 2021-10-27 21:42:57.000000 hyssop_aiodb-0.0.8/setup.py
--rw-rw-rw-   0        0        0     1754 2021-03-21 19:00:27.000000 hyssop_aiodb-0.0.8/setup_aiodb.py
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.455092 hyssop_aiodb-0.0.9/
+-rwx------   0 howardlkung   (501) staff       (20)     1092 2020-09-24 10:33:22.000000 hyssop_aiodb-0.0.9/LICENSE
+-rw-r--r--   0 howardlkung   (501) staff       (20)      638 2024-05-26 01:19:26.454919 hyssop_aiodb-0.0.9/PKG-INFO
+-rwx------   0 howardlkung   (501) staff       (20)     2885 2024-05-26 01:19:11.000000 hyssop_aiodb-0.0.9/README.md
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.451050 hyssop_aiodb-0.0.9/hyssop_aiodb/
+-rwx------   0 howardlkung   (501) staff       (20)      314 2024-05-26 01:15:53.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/__init__.py
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.452405 hyssop_aiodb-0.0.9/hyssop_aiodb/component/
+-rwx------   0 howardlkung   (501) staff       (20)      507 2022-06-01 19:16:18.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/__init__.py
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.453830 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/
+-rwx------   0 howardlkung   (501) staff       (20)      815 2021-01-08 21:25:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/__init__.py
+-rwx------   0 howardlkung   (501) staff       (20)     4855 2021-01-25 00:06:41.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/component.py
+-rwx------   0 howardlkung   (501) staff       (20)     1220 2021-02-04 04:38:09.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/constants.py
+-rwx------   0 howardlkung   (501) staff       (20)      486 2021-02-04 04:35:48.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/local.csv
+-rwx------   0 howardlkung   (501) staff       (20)    36585 2022-12-17 21:46:49.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/utils.py
+-rwx------   0 howardlkung   (501) staff       (20)     1255 2022-06-01 19:15:49.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb_mixin.py
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.454549 hyssop_aiodb-0.0.9/hyssop_aiodb/unit_test/
+-rwx------   0 howardlkung   (501) staff       (20)      462 2020-12-27 05:29:11.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/unit_test/__init__.py
+-rwx------   0 howardlkung   (501) staff       (20)     5546 2024-05-25 15:09:44.000000 hyssop_aiodb-0.0.9/hyssop_aiodb/unit_test/ut.py
+drwxr-xr-x   0 howardlkung   (501) staff       (20)        0 2024-05-26 01:19:26.451919 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/
+-rw-r--r--   0 howardlkung   (501) staff       (20)      638 2024-05-26 01:19:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/PKG-INFO
+-rw-r--r--   0 howardlkung   (501) staff       (20)      584 2024-05-26 01:19:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/SOURCES.txt
+-rw-r--r--   0 howardlkung   (501) staff       (20)        1 2024-05-26 01:19:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/dependency_links.txt
+-rw-r--r--   0 howardlkung   (501) staff       (20)       67 2024-05-26 01:19:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/requires.txt
+-rw-r--r--   0 howardlkung   (501) staff       (20)       13 2024-05-26 01:19:26.000000 hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/top_level.txt
+-rw-r--r--   0 howardlkung   (501) staff       (20)       38 2024-05-26 01:19:26.455159 hyssop_aiodb-0.0.9/setup.cfg
+-rwx------   0 howardlkung   (501) staff       (20)     1540 2021-10-27 21:42:57.000000 hyssop_aiodb-0.0.9/setup.py
+-rwx------   0 howardlkung   (501) staff       (20)     1748 2024-05-25 10:32:50.000000 hyssop_aiodb-0.0.9/setup_aiodb.py
```

### Comparing `hyssop_aiodb-0.0.8/LICENSE` & `hyssop_aiodb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/README.md` & `hyssop_aiodb-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,19 @@
 * **0.0.2 - Feb. 15, 2021**:
   * Fix get_argument() of AioHttpRequest with given default value still raise Exception.
 
 * **0.0.1 - Jan. 10, 2021**:
   * Integrate with [aiohttp](https://docs.aiohttp.org/en/stable/) web framework.
 
 ## hyssop-aiodb
+* **0.0.9 - 05. 26, 2024**:
+  * Update dependency aiomysql.
+
+* **0.0.8 - 12. 17, 2022**:
+  * Refactor connection lock.
 
 * **0.0.7 - Apr. 7, 2021**:
   * Fix bug of value convertion in util
   * Fix bug of AsyncEntityUW update().
   * Add timer to reconnect db connections
 
 * **0.0.3 - Feb. 15, 2021**:
```

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/__init__.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/component.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/component.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/constants.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/constants.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb/utils.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb/utils.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/component/aiodb_mixin.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/component/aiodb_mixin.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb/unit_test/ut.py` & `hyssop_aiodb-0.0.9/hyssop_aiodb/unit_test/ut.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This module is part of hyssop and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
 '''
 File created: December 26th 2020
 
 Modified By: hsky77
-Last Updated: December 17th 2022 13:45:15 pm
+Last Updated: May 25th 2024 23:09:44 pm
 '''
 
 import enum
-import asyncio
+# import asyncio
 
-# try:
-#     import asyncio
-#     import uvloop
-#     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-# except:
-#     pass
+try:
+    import asyncio
+    import uvloop
+    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+except:
+    pass
 
 
 from random import randint
 from datetime import datetime
 from typing import Dict, Any
 
 from sqlalchemy import Column, String, Integer, Text, Enum, DateTime, ForeignKey
@@ -97,18 +97,18 @@
             SW_MODULES, file_name=__path__[0] + "/testdb.db"
             # , reconnect_seconds=0
         )
 
         db = AioMySQLDatabase(SW_MODULES,      host="192.168.1.20",  port=3306,
                               db_name="test",
                               user="root",
-                              password="Hk..8564",
+                              password="test_mariadb",
                               connections=1,
-                              connect_timeout=1
-                              #   reconnect_seconds=0
+                            #   connect_timeout=10
+                                reconnect_seconds=0
                               )
 
         async def testAsync(index: str):
             async with db.get_connection_proxy() as conn:
                 async with conn.get_cursor_proxy() as cur:
                     account_data = {
                         'account': index,
```

### Comparing `hyssop_aiodb-0.0.8/hyssop_aiodb.egg-info/SOURCES.txt` & `hyssop_aiodb-0.0.9/hyssop_aiodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/setup.py` & `hyssop_aiodb-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `hyssop_aiodb-0.0.8/setup_aiodb.py` & `hyssop_aiodb-0.0.9/setup_aiodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This module is part of hyssop and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
 '''
 File created: August 21st 2020
 
 Modified By: hsky77
-Last Updated: December 29th 2020 19:41:42 pm
+Last Updated: May 25th 2024 18:32:50 pm
 '''
 
 import os
 import shutil
 import setuptools
 
 from hyssop import Version as hy_ver
@@ -47,12 +47,12 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=['hyssop>=' + hy_ver,
                       'sqlalchemy==1.3.20',
-                      'aiomysql==0.0.21',
-                      'aiosqlite==0.16.0'],
+                      'aiomysql==0.2.0',
+                      'aiosqlite==0.20.0'],
     python_requires='>=3.6',
     package_data={'': ['*.yaml', '*.csv']}
 )
```

