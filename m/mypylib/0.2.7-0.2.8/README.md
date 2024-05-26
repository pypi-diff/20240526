# Comparing `tmp/mypylib-0.2.7.tar.gz` & `tmp/mypylib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.7.tar", last modified: Sun May 26 06:37:31 2024, max compression
+gzip compressed data, was "mypylib-0.2.8.tar", last modified: Sun May 26 06:46:22 2024, max compression
```

## Comparing `mypylib-0.2.7.tar` & `mypylib-0.2.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.381225 mypylib-0.2.7/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:37:31.380941 mypylib-0.2.7/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.7/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.376190 mypylib-0.2.7/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    51345 2024-05-26 06:35:10.000000 mypylib-0.2.7/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3661 2024-04-26 09:26:57.000000 mypylib-0.2.7/mypylib/binance.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.7/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.7/mypylib/my_random_proxy.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/rayin.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    11120 2024-05-12 07:09:19.000000 mypylib-0.2.7/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.380422 mypylib-0.2.7/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.7/mypylib/tmpDevelopment/arping.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.7/mypylib/tmpDevelopment/tmp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.7/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2024-04-28 14:14:53.000000 mypylib-0.2.7/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.7/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    12075 2024-05-26 06:32:42.000000 mypylib-0.2.7/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:37:31.378127 mypylib-0.2.7/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-05-26 06:37:31.000000 mypylib-0.2.7/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-05-26 06:37:31.381311 mypylib-0.2.7/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.7/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:46:22.967612 mypylib-0.2.8/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:46:22.967351 mypylib-0.2.8/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.8/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:46:22.962940 mypylib-0.2.8/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    51416 2024-05-26 06:45:40.000000 mypylib-0.2.8/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3661 2024-04-26 09:26:57.000000 mypylib-0.2.8/mypylib/binance.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.8/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.8/mypylib/my_random_proxy.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/rayin.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    11120 2024-05-12 07:09:19.000000 mypylib-0.2.8/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:46:22.966723 mypylib-0.2.8/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.8/mypylib/tmpDevelopment/arping.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.8/mypylib/tmpDevelopment/tmp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.8/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2024-04-28 14:14:53.000000 mypylib-0.2.8/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.8/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    12084 2024-05-26 06:45:21.000000 mypylib-0.2.8/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-05-26 06:46:22.964704 mypylib-0.2.8/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-05-26 06:46:22.000000 mypylib-0.2.8/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-05-26 06:46:22.000000 mypylib-0.2.8/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-05-26 06:46:22.000000 mypylib-0.2.8/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-05-26 06:46:22.000000 mypylib-0.2.8/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-05-26 06:46:22.967698 mypylib-0.2.8/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.8/setup.py
```

### Comparing `mypylib-0.2.7/README.md` & `mypylib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.8/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/__init__.py` & `mypylib-0.2.8/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,17 +95,18 @@
     '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
     '2024/04/15: 0.2.02 add warrant_bible_do_all()',
     '2024/04/16: 0.2.03 change request to http.client',
     '2024/04/16: 0.2.04 add proxy',
     '2024/04/16: 0.2.05 add proxy to request.get()',
     '2024/04/28: 0.2.06 add order_callback() in sjtools',
     '2024/05/02: 0.2.07 增加權證在外流通、到期日',
+    '2024/05/02: 0.2.08 增加權證在外流通、到期日 fix bug',
 }
 
-__version__ = '0.2.07'
+__version__ = '0.2.08'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.7/mypylib/binance.py` & `mypylib-0.2.8/mypylib/binance.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/binance_copy_bot.py` & `mypylib-0.2.8/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/chdbif.py` & `mypylib-0.2.8/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/crawler.py` & `mypylib-0.2.8/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/crypto.py` & `mypylib-0.2.8/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/finmind.py` & `mypylib-0.2.8/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/libexcel.py` & `mypylib-0.2.8/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/mvp.py` & `mypylib-0.2.8/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/option_test.py` & `mypylib-0.2.8/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/rayin.py` & `mypylib-0.2.8/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.8/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/shioaji_kline.py` & `mypylib-0.2.8/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/shioaji_ticks.py` & `mypylib-0.2.8/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/sjtools.py` & `mypylib-0.2.8/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tLineNotify.py` & `mypylib-0.2.8/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/ti.py` & `mypylib-0.2.8/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tmpDevelopment/arping.py` & `mypylib-0.2.8/mypylib/tmpDevelopment/arping.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tmpDevelopment/tmp.py` & `mypylib-0.2.8/mypylib/tmpDevelopment/tmp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.8/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tplaysound.py` & `mypylib-0.2.8/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/tredis.py` & `mypylib-0.2.8/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/mypylib/warrant.py` & `mypylib-0.2.8/mypylib/warrant.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     today = datetime.datetime.today()
     with open(target_file, "w+") as fp:
         for warrant in dict_warrant_to_info:
             day_end = datetime.datetime.strptime(dict_warrant_to_info[warrant]['到期日期'], '%Y/%m/%d')
             fp.write(f'{warrant}\t'
                      f'{dict_warrant_to_info[warrant]["標的代碼"]}\t'
                      f'{dict_warrant_to_info[warrant]["認購/售類別"]}\t'
-                     f'{dict_warrant_to_info["流通在外估計張數"]}\t'
+                     f'{dict_warrant_to_info[warrant]["流通在外估計張數"]}\t'
                      f'{(day_end - today).days}\n')
 
 
 def download_latest_warrant_bible():
     day_now = datetime.datetime.now()
 
     while True:
```

### Comparing `mypylib-0.2.7/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.8/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.7/setup.py` & `mypylib-0.2.8/setup.py`

 * *Files identical despite different names*

