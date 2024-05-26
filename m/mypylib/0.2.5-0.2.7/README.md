# Comparing `tmp/mypylib-0.2.5.tar.gz` & `tmp/mypylib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.5.tar", last modified: Tue Apr 16 12:43:42 2024, max compression
+gzip compressed data, was "mypylib-0.2.7.tar", last modified: Sun May 26 06:37:31 2024, max compression
```

## Comparing `mypylib-0.2.5.tar` & `mypylib-0.2.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:43:42.561606 mypylib-0.2.5/
--rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 12:43:42.561606 mypylib-0.2.5/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     3740 2023-11-06 13:42:12.000000 mypylib-0.2.5/README.md
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:43:42.557606 mypylib-0.2.5/mypylib/
--rw-rw-r--   0 william   (1000) william   (1000)     3184 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/MP_shioaji_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)    51224 2024-04-16 12:42:35.000000 mypylib-0.2.5/mypylib/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)     3364 2024-03-13 13:37:39.000000 mypylib-0.2.5/mypylib/binance.py
--rw-rw-r--   0 william   (1000) william   (1000)     7105 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/binance_copy_bot.py
--rw-rw-r--   0 william   (1000) william   (1000)     3421 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/chdbif.py
--rw-rw-r--   0 william   (1000) william   (1000)     5984 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/crawler.py
--rw-rw-r--   0 william   (1000) william   (1000)     1083 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/crypto.py
--rw-rw-r--   0 william   (1000) william   (1000)     5093 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/finmind.py
--rw-rw-r--   0 william   (1000) william   (1000)    87196 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/libexcel.py
--rw-rw-r--   0 william   (1000) william   (1000)    24435 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/mvp.py
--rw-rw-r--   0 william   (1000) william   (1000)      157 2024-03-13 13:37:39.000000 mypylib-0.2.5/mypylib/my_random_proxy.py
--rw-rw-r--   0 william   (1000) william   (1000)     3588 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/option_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     1109 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/rayin.py
--rw-rw-r--   0 william   (1000) william   (1000)      778 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/shioaji_history_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)     2490 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/shioaji_kline.py
--rw-rw-r--   0 william   (1000) william   (1000)     1312 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/shioaji_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)    10696 2024-03-13 13:37:39.000000 mypylib-0.2.5/mypylib/sjtools.py
--rw-rw-r--   0 william   (1000) william   (1000)     1464 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/tLineNotify.py
--rw-rw-r--   0 william   (1000) william   (1000)     7735 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/ti.py
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:43:42.561606 mypylib-0.2.5/mypylib/tmpDevelopment/
--rw-rw-r--   0 william   (1000) william   (1000)        0 2023-11-06 13:42:12.000000 mypylib-0.2.5/mypylib/tmpDevelopment/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)       37 2024-03-14 04:27:41.000000 mypylib-0.2.5/mypylib/tmpDevelopment/aa.py
--rw-rw-r--   0 william   (1000) william   (1000)     1958 2024-03-14 04:49:02.000000 mypylib-0.2.5/mypylib/tmpDevelopment/socket_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     1074 2023-11-06 13:42:12.000000 mypylib-0.2.5/mypylib/tmpDevelopment/warrant_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     2543 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/tplaysound.py
--rw-rw-r--   0 william   (1000) william   (1000)     8609 2023-11-06 13:43:07.000000 mypylib-0.2.5/mypylib/tredis.py
--rw-rw-r--   0 william   (1000) william   (1000)    11751 2024-04-16 12:40:32.000000 mypylib-0.2.5/mypylib/warrant.py
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:43:42.557606 mypylib-0.2.5/mypylib.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 12:43:42.000000 mypylib-0.2.5/mypylib.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)      752 2024-04-16 12:43:42.000000 mypylib-0.2.5/mypylib.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        1 2024-04-16 12:43:42.000000 mypylib-0.2.5/mypylib.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)        8 2024-04-16 12:43:42.000000 mypylib-0.2.5/mypylib.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)       38 2024-04-16 12:43:42.561606 mypylib-0.2.5/setup.cfg
--rw-rw-r--   0 william   (1000) william   (1000)      846 2023-11-06 13:42:12.000000 mypylib-0.2.5/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.381225 mypylib-0.2.7/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:37:31.380941 mypylib-0.2.7/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.7/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.376190 mypylib-0.2.7/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    51345 2024-05-26 06:35:10.000000 mypylib-0.2.7/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3661 2024-04-26 09:26:57.000000 mypylib-0.2.7/mypylib/binance.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.7/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.7/mypylib/my_random_proxy.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/rayin.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    11120 2024-05-12 07:09:19.000000 mypylib-0.2.7/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.380422 mypylib-0.2.7/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.7/mypylib/tmpDevelopment/arping.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.7/mypylib/tmpDevelopment/tmp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2024-04-28 14:14:53.000000 mypylib-0.2.7/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.7/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    12075 2024-05-26 06:32:42.000000 mypylib-0.2.7/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.378127 mypylib-0.2.7/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-05-26 06:37:31.381311 mypylib-0.2.7/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.7/setup.py
```

### Comparing `mypylib-0.2.5/README.md` & `mypylib-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.7/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/__init__.py` & `mypylib-0.2.7/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,17 +93,19 @@
     '2024/03/24: 0.1.99 modify warrant_bible_convert_to_c_need() and save warrant_bible.txt',
     '2024/03/27: 0.2.00 fix get_punishment_list() date bug ',
     '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
     '2024/04/15: 0.2.02 add warrant_bible_do_all()',
     '2024/04/16: 0.2.03 change request to http.client',
     '2024/04/16: 0.2.04 add proxy',
     '2024/04/16: 0.2.05 add proxy to request.get()',
+    '2024/04/28: 0.2.06 add order_callback() in sjtools',
+    '2024/05/02: 0.2.07 增加權證在外流通、到期日',
 }
 
-__version__ = '0.2.05'
+__version__ = '0.2.07'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.5/mypylib/binance.py` & `mypylib-0.2.7/mypylib/binance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Org binance data path: https://data.binance.vision/
+#
+# 這個是用來下載幣安 Binance 的歷史資料做回測
+#
+
+
+
 import requests
 import xmltodict
 import json
 import wget
 from enum import Enum
 import os
 
@@ -44,27 +51,29 @@
     _3m = '3m'
     _4h = '4h'
     _5m = '5m'
     _6h = '6h'
     _8h = '8h'
 
 
+# 列出幣安歷史資料上的所有標地
 def binance_get_history_list_targets(future_option_spot, cm_um, daily_monthly, klines_others):
     # https://s3-ap-northeast-1.amazonaws.com/data.binance.vision?delimiter=/&prefix=data/futures/um/monthly/klines/
     url = f'https://s3-ap-northeast-1.amazonaws.com/data.binance.vision?delimiter=/&prefix=data/{future_option_spot}/{cm_um}/{daily_monthly}/{klines_others}/'
     # print(url)
     r = requests.get(url, headers=headers)
     xpars = xmltodict.parse(r.text)
     ret = []
     # print(xpars)
     for x in xpars['ListBucketResult']['CommonPrefixes']:
         ret.append(x['Prefix'].split('/')[-2])
     return ret
 
 
+# 列出幣安歷史資料上的所有檔案
 def binance_get_history_list_files_by_target(future_option_spot, cm_um, daily_monthly, klines_others, str_target, period):
     url = f'https://s3-ap-northeast-1.amazonaws.com/data.binance.vision?delimiter=/&prefix=data/{future_option_spot}/{cm_um}/{daily_monthly}/{klines_others}/{str_target}/{period}/'
     print(url)
     r = requests.get(url, headers=headers)
     print(r.text)
     xpars = xmltodict.parse(r.text)
     ret = []
@@ -80,37 +89,33 @@
     except:
         print(f"download {url} failed")
         return False
     return True
 
 
 if __name__ == '__main__':
+    # 列出幣安所有標地
     list_targets = binance_get_history_list_targets(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines)
     print(list_targets)
 
-    list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, list_targets[0], Period._15m)
+
+    list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, list_targets[0], Period._5m)
     print(list_files)
 
+
     binance_get_history_download_file(list_files[0], list_files[0].split('/')[-1])
 
     for target in list_targets:
-        list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, target, Period._15m)
+        if not target.endswith('USDT'):
+            continue
+        list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, target, Period._1m)
         for file_url in list_files:
             if not file_url.endswith('.zip'):
                 continue
             file_name = file_url.split('/')[-1]
 
             if os.path.isfile(file_name):
                 continue
 
             print(f'Donwload {file_url} {file_name}')
             binance_get_history_download_file(file_url, file_name)
 
-
-
-
-
-
-
-
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mypylib-0.2.5/mypylib/binance_copy_bot.py` & `mypylib-0.2.7/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/chdbif.py` & `mypylib-0.2.7/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/crawler.py` & `mypylib-0.2.7/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/crypto.py` & `mypylib-0.2.7/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/finmind.py` & `mypylib-0.2.7/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/libexcel.py` & `mypylib-0.2.7/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/mvp.py` & `mypylib-0.2.7/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/option_test.py` & `mypylib-0.2.7/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/rayin.py` & `mypylib-0.2.7/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.7/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/shioaji_kline.py` & `mypylib-0.2.7/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/shioaji_ticks.py` & `mypylib-0.2.7/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/sjtools.py` & `mypylib-0.2.7/mypylib/sjtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+
 import datetime
 import pandas as pd
 import shioaji as sj
 from shioaji import contracts
-from shioaji.constant import SecurityType
+from shioaji.constant import SecurityType, OrderState
 from shioaji.contracts import Contract
 import os
 from time import sleep
 import json
 from mypylib import get_trade_days
 from typing import Union
 from collections import defaultdict
@@ -198,14 +199,25 @@
         self.api.login(self.api_key, self.secret_key, contracts_cb=self.contract_cb)
 
         while True:
             sleep(1)
             if self.bool_OPT_fetched and self.bool_STK_fetched and self.bool_FUT_fetched and self.bool_IND_fetched:
                 break
 
+        self.api.set_order_callback(self.order_callback)
+
+    def order_callback(self, stat: OrderState, msg_dict: dict):
+        logger.info(f'{stat} {msg_dict}')
+
+    def activate_ca(self, ca_path, ca_passwd, person_id):
+        self.api.activate_ca(ca_path=ca_path,
+                             ca_passwd=ca_passwd,
+                             person_id=person_id,
+                             store=1000)
+
     def contract_cb(self, security_type: SecurityType):
         logger.info(f"{repr(security_type)} fetch done.")
         if security_type == SecurityType.Index:
             self.bool_IND_fetched = True
         elif security_type == SecurityType.Future:
             self.bool_FUT_fetched = True
         elif security_type == SecurityType.Stock:
```

### Comparing `mypylib-0.2.5/mypylib/tLineNotify.py` & `mypylib-0.2.7/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/ti.py` & `mypylib-0.2.7/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.7/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/tplaysound.py` & `mypylib-0.2.7/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/tredis.py` & `mypylib-0.2.7/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.5/mypylib/warrant.py` & `mypylib-0.2.7/mypylib/warrant.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,17 +231,23 @@
 
             dict_stock_to_warrant[x[4]].append(x[1])
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
 def warrant_bible_convert_to_c_need(dict_warrant_to_info):
     target_file = f'/home/william/warrant/warrant_bible.txt'
+    today = datetime.datetime.today()
     with open(target_file, "w+") as fp:
         for warrant in dict_warrant_to_info:
-            fp.write(f'{warrant}\t{dict_warrant_to_info[warrant]["標的代碼"]}\t{dict_warrant_to_info[warrant]["認購/售類別"]}\n')
+            day_end = datetime.datetime.strptime(dict_warrant_to_info[warrant]['到期日期'], '%Y/%m/%d')
+            fp.write(f'{warrant}\t'
+                     f'{dict_warrant_to_info[warrant]["標的代碼"]}\t'
+                     f'{dict_warrant_to_info[warrant]["認購/售類別"]}\t'
+                     f'{dict_warrant_to_info["流通在外估計張數"]}\t'
+                     f'{(day_end - today).days}\n')
 
 
 def download_latest_warrant_bible():
     day_now = datetime.datetime.now()
 
     while True:
         str_date = day_now.strftime('%Y-%m-%d')
```

### Comparing `mypylib-0.2.5/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.7/mypylib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 mypylib/tredis.py
 mypylib/warrant.py
 mypylib.egg-info/PKG-INFO
 mypylib.egg-info/SOURCES.txt
 mypylib.egg-info/dependency_links.txt
 mypylib.egg-info/top_level.txt
 mypylib/tmpDevelopment/__init__.py
-mypylib/tmpDevelopment/aa.py
-mypylib/tmpDevelopment/socket_test.py
+mypylib/tmpDevelopment/arping.py
+mypylib/tmpDevelopment/tmp.py
 mypylib/tmpDevelopment/warrant_test.py
```

### Comparing `mypylib-0.2.5/setup.py` & `mypylib-0.2.7/setup.py`

 * *Files identical despite different names*

