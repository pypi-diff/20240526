# Comparing `tmp/proxy_inspector-0.0.4-py3-none-any.whl.zip` & `tmp/proxy_inspector-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3861 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     2163 b- defN 23-Mar-03 14:39 proxy_inspector.py
--rw-rw-rw-  2.0 fat     4805 b- defN 23-Mar-03 14:39 useragents.py
--rw-rw-rw-  2.0 fat     1160 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/namespace_packages.txt
--rw-rw-rw-  2.0 fat       27 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/zip-safe
-?rw-rw-r--  2.0 fat      677 b- defN 23-Mar-03 14:39 proxy_inspector-0.0.4.dist-info/RECORD
-8 files, 8927 bytes uncompressed, 2661 bytes compressed:  70.2%
+Zip file size: 3886 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     2161 b- defN 24-May-26 10:05 proxy_inspector.py
+-rw-rw-rw-  2.0 fat     4805 b- defN 24-May-26 10:05 useragents.py
+-rw-rw-rw-  2.0 fat     1182 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/namespace_packages.txt
+-rw-rw-rw-  2.0 fat       27 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/zip-safe
+-rw-rw-r--  2.0 fat      677 b- defN 24-May-26 10:05 proxy_inspector-0.0.5.dist-info/RECORD
+8 files, 8947 bytes uncompressed, 2686 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: proxy_inspector.py
 Comment: 
 
 Filename: useragents.py
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/METADATA
+Filename: proxy_inspector-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/WHEEL
+Filename: proxy_inspector-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/namespace_packages.txt
+Filename: proxy_inspector-0.0.5.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/top_level.txt
+Filename: proxy_inspector-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/zip-safe
+Filename: proxy_inspector-0.0.5.dist-info/zip-safe
 Comment: 
 
-Filename: proxy_inspector-0.0.4.dist-info/RECORD
+Filename: proxy_inspector-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proxy_inspector.py

```diff
@@ -22,15 +22,14 @@
         """
         An Simple Tool for Validate Proxy \n
         :param target_url: Target URL, like "https://www.bing.com/robots.txt"
         :param proxy_urls: Proxy URL list, like ["http://127.0.0.1:7777"]
         :return: Return True if the condition is met
 
         """
-
         proxies = []
 
         # ----------------------------------------
         # Check Schema
         # ----------------------------------------
         proxies_obj_pending = []
         proxies_pending = []
```

## Comparing `proxy_inspector-0.0.4.dist-info/METADATA` & `proxy_inspector-0.0.5.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy-inspector
-Version: 0.0.4
+Version: 0.0.5
 Summary: An Simple Tool for Validate Proxy
 Home-page: https://github.com/HostenWang/proxy-inspector
 Author: HostenWang
 Author-email: hostenwang@foxmail.com
 Maintainer: 
 Maintainer-email: 
 Keywords: python proxy network validate
@@ -14,20 +14,20 @@
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: grequests (~=0.6.0)
-Requires-Dist: requests (~=2.28.1)
+Requires-Dist: grequests ~=0.6.0
+Requires-Dist: requests ~=2.28.1
 
 # proxy-inspector
 
-A Simple Tool for Validate Proxy
+A tool for quickly verifying the availability of proxy IP 
 
 ## Usage
 
 ```python
 >> from proxy_inspector import ProxyInspector
 >> checker = ProxyInspector()
 >> proxies = checker.validate("https://www.google.com", ["https://MY_PROXY_1", "https://MY_PROXY_2", "https://MY-PROXY-3"])
```

## Comparing `proxy_inspector-0.0.4.dist-info/RECORD` & `proxy_inspector-0.0.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-proxy_inspector.py,sha256=eCbB5_ZFtHwKX2Dnk8pbgy_wn_5J7RnCtmbI9VGxLv0,2163
+proxy_inspector.py,sha256=PfJNUl7XGJx6CQxNAYAiqU8bSYL1ewoh9LA7_tLy1H8,2161
 useragents.py,sha256=E218XgDillxvAhQFxJvYS6KRFNQupF4xWe3PaL7m8ww,4805
-proxy_inspector-0.0.4.dist-info/METADATA,sha256=__PZ2zzakLHyUjk0MFWrF9ak6DuLmmqupABPdSm0eKs,1160
-proxy_inspector-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-proxy_inspector-0.0.4.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-proxy_inspector-0.0.4.dist-info/top_level.txt,sha256=RQdKWaa8uQ3XVY-GquvTe2qrP7syYrgASFxVcHurRjk,27
-proxy_inspector-0.0.4.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-proxy_inspector-0.0.4.dist-info/RECORD,,
+proxy_inspector-0.0.5.dist-info/METADATA,sha256=a5wpohx1Ku-Sqz7cCclZ7YBUzsBbkIEZmGXEj871JIw,1182
+proxy_inspector-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+proxy_inspector-0.0.5.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+proxy_inspector-0.0.5.dist-info/top_level.txt,sha256=RQdKWaa8uQ3XVY-GquvTe2qrP7syYrgASFxVcHurRjk,27
+proxy_inspector-0.0.5.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+proxy_inspector-0.0.5.dist-info/RECORD,,
```

