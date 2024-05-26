# Comparing `tmp/chatchat-0.1.1.tar.gz` & `tmp/chatchat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.1.1.tar", last modified: Thu May 23 13:31:23 2024, max compression
+gzip compressed data, was "chatchat-0.1.2.tar", last modified: Sun May 26 00:51:38 2024, max compression
```

## Comparing `chatchat-0.1.1.tar` & `chatchat-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:23.231751 chatchat-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-23 13:31:17.000000 chatchat-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-23 13:31:23.231751 chatchat-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-23 13:31:17.000000 chatchat-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:23.231751 chatchat-0.1.1/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/tencent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-23 13:31:17.000000 chatchat-0.1.1/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:23.231751 chatchat-0.1.1/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-23 13:31:23.000000 chatchat-0.1.1/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 13:31:23.000000 chatchat-0.1.1/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:31:23.000000 chatchat-0.1.1/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 13:31:23.000000 chatchat-0.1.1/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 13:31:23.000000 chatchat-0.1.1/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:31:23.231751 chatchat-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 13:31:17.000000 chatchat-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-26 00:51:26.000000 chatchat-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-26 00:51:38.736480 chatchat-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-26 00:51:26.000000 chatchat-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:51:38.736480 chatchat-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-26 00:51:26.000000 chatchat-0.1.2/setup.py
```

### Comparing `chatchat-0.1.1/LICENSE` & `chatchat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.1/chatchat/alibaba.py` & `chatchat-0.1.2/chatchat/alibaba.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from chatchat.base import Base
-import httpx, time
+import httpx
 
 class Completion(Base):
-    def __init__(self, jfile, model='qwen-turbo'):
+    def __init__(self, model='qwen-turbo'):
+        super().__init__()
+
+        plat = 'alibaba'
+        self.verify_secret_data(plat, ('api_key',))
+        self.jdata = self.secret_data[plat]
+
         # https://dashscope.console.aliyun.com/dashboard?apiKey=all&model=qwen-turbo
         self.model_type = set([
             'qwen-turbo',
             'qwen-plus',
             'qwen-max',
         ])
 
         if model not in self.model_type:
             raise RuntimeError(f'supported chat type: {list(self.model_type)}')
         self.model = model
 
-        self.jfile = jfile
-        self.jdata = self.load_json(jfile)['alibaba']
         self.api = 'https://dashscope.aliyuncs.com/api/v1/services/aigc/text-generation/generation'
         self.client = httpx.Client()
         self.headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.jdata["api_key"]}',
         }
 
@@ -40,16 +44,16 @@
         jmsg = [{
             "role": "user",
             "content": message,
         }]
         return self.send_message(jmsg)
 
 class Chat(Completion):
-    def __init__(self, jfile, model='qwen-turbo', history=[]):
-        super().__init__(jfile, model=model)
+    def __init__(self, model='qwen-turbo', history=[]):
+        super().__init__(model=model)
         self.history = history
 
     def chat(self, message):
         self.history.append({
             'role': 'user',
             'content': message,
         })
```

### Comparing `chatchat-0.1.1/chatchat/baidu.py` & `chatchat-0.1.2/chatchat/baidu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 from chatchat.base import Base
 import httpx, time
 
 class Completion(Base):
-    def __init__(self, jfile, model='ERNIE-Speed-8K'):
+    def __init__(self, model='ERNIE-Speed-8K'):
+        super().__init__()
+
+        # https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application
+        #     {
+        #         "baidu": {
+        #             "api_key": "x",
+        #             "secret_key": "y",
+        #             "expires_in": "z",
+        #             "access_token": "k"
+        #         }
+        #     }
+        plat = 'baidu'
+        self.verify_secret_data(plat, ('api_key', 'secret_key'))
+        self.jdata = self.secret_data[plat]
+        self.update_interval = 3600
+
         # https://console.bce.baidu.com/qianfan/ais/console/onlineService
         self.api_list = {
             'ERNIE-Speed-8K': 'ernie_speed',
             'ERNIE-Speed-128K': 'ernie-speed-128k',
             'ERNIE-Speed-AppBuilder': 'ai_apaas',
             'ERNIE-Lite-8K': 'ernie-lite-8k',
             'ERNIE-Lite-8K-0922': 'eb-instant',
@@ -15,34 +31,19 @@
             'Yi-34B-Chat': 'yi_34b_chat',
         }
 
         if model not in self.api_list:
             raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
         self.api = 'https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/' + self.api_list[model]
         self.client = httpx.Client()
-
-        # jfile: https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application
-        #     {
-        #         "baidu": {
-        #             "api_key": "x",
-        #             "secret_key": "y",
-        #             "expires_in": "z",
-        #             "access_token": "k"
-        #         }
-        #     }
-        self.jfile = jfile
-        self.jdata = self.load_json(jfile)['baidu']
-        self.update_interval = 3600
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
-        if "api_key" not in self.jdata or "secret_key" not in self.jdata:
-            raise RuntimeError(f'please check <baidu> api_key and secret_key in {jfile}')
         self.update_access_token()
 
     def update_access_token(self):
         if 'expires_in' not in self.jdata or not self.jdata['expires_in'] \
             or self.jdata['expires_in'] < time.time() + self.update_interval:
             # https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Ilkkrb0i5
             url = "https://aip.baidubce.com/oauth/2.0/token"
@@ -83,16 +84,16 @@
                 "role": "user",
                 "content": message,
             }
         ]
         return self.send_messages(messages)
 
 class Chat(Completion):
-    def __init__(self, jfile, model='ERNIE-Speed-8K', history=[]):
-        super().__init__(jfile, model=model)
+    def __init__(self, model='ERNIE-Speed-8K', history=[]):
+        super().__init__(model=model)
         self.history = history
 
     def chat(self, message):
         self.history.append({
             "role": "user",
             "content": message,
         })
```

### Comparing `chatchat-0.1.1/chatchat/tencent.py` & `chatchat-0.1.2/chatchat/tencent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from chatchat.base import Base
-import hashlib, hmac, json, os, sys, time
+import hashlib, hmac, json, time
 from datetime import datetime
 import httpx
 
 class Completion(Base):
-    def __init__(self, jfile, model='hunyuan-lite'):
+    def __init__(self, model='hunyuan-lite'):
+        super().__init__()
+
+        plat = 'tencent'
+        self.verify_secret_data(plat, ('secret_id', 'secret_key'))
+        self.jdata = self.secret_data[plat]
+        self.secret_id = self.jdata['secret_id']
+        self.secret_key = self.jdata['secret_key']
+
         self.model_type = set([
             'hunyuan-lite',
             'hunyuan-standard',
             'hunyuan-standard-256K',
             'hunyuan-pro',
         ])
-
         if model not in self.model_type:
             raise RuntimeError(f'supported chat type: {list(self.model_type)}')
         self.model = model
 
-        self.jfile = jfile
-        self.jdata = self.load_json(jfile)['tencent']
-        self.secret_id = self.jdata['secret_id']
-        self.secret_key = self.jdata['secret_key']
         self.host = 'hunyuan.tencentcloudapi.com'
         self.endpoint = f'https://{self.host}'
         self.client = httpx.Client()
 
     def encode_message(self, jmsg):
         # step 1
         http_request_method = "POST"
@@ -98,16 +101,16 @@
         jmsg = [{
             "Role": "user",
             "Content": message,
         }]
         return self.send_message(jmsg)
 
 class Chat(Completion):
-    def __init__(self, jfile, model='hunyuan-lite', history=[]):
-        super().__init__(jfile, model=model)
+    def __init__(self, model='hunyuan-lite', history=[]):
+        super().__init__(model=model)
         self.history = history
 
     def chat(self, message):
         self.history.append({
             'Role': 'user',
             'Content': message,
         })
```

### Comparing `chatchat-0.1.1/chatchat/xunfei.py` & `chatchat-0.1.2/chatchat/xunfei.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from wsgiref.handlers import format_date_time
 from urllib.parse import urlencode
 from chatchat.base import Base
 import base64, hashlib, hmac
 from datetime import datetime
 from time import mktime
-import time, websocket, json, ssl
+import websocket, json, ssl
 
 class Completion(Base):
-    def __init__(self, jfile, model='Spark Lite'):
+    def __init__(self, model='Spark Lite'):
+        super().__init__()
+
+        # https://console.xfyun.cn/services/bm2
+        # "xunfei": {
+        #     "app_id": "x",
+        #     "api_secret": "y",
+        #     "api_key": "z"
+        # }
+        plat = 'xunfei'
+        self.verify_secret_data(plat, ('api_key', 'api_secret', 'app_id'))
+        self.jdata = self.secret_data[plat]
+
         # https://www.xfyun.cn/doc/spark/Web.html#_1-接口说明
         self.api_list = {
             'Spark3.5 Max': {
                 'path': '/v3.5/chat',
                 'domain': 'generalv3.5',
             },
             'Spark Pro': {
@@ -31,32 +43,20 @@
         if model not in self.api_list:
             raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
         self.host = 'spark-api.xf-yun.com'
         self.api = self.api_list[model]
         self.path = self.api['path']
         self.domain = self.api['domain']
 
-        # jfile: https://console.xfyun.cn/services/bm2
-        # "xunfei": {
-        #     "app_id": "x",
-        #     "api_secret": "y",
-        #     "api_key": "z"
-        # }
-        self.jfile = jfile
-        self.jdata = self.load_json(jfile)['xunfei']
         self.update_interval = 150
         self.headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
-        if "api_key" not in self.jdata or "api_secret" not in self.jdata:
-            raise RuntimeError(f'please check <xunfei> api_key and api_secret in {jfile}')
-
-        self.update_url()
         websocket.enableTrace(False)
         self.answer = ''
 
     def create_url(self):
         # https://www.xfyun.cn/doc/spark/general_url_authentication.html
         now = datetime.now()
         date = format_date_time(mktime(now.timetuple()))
@@ -80,29 +80,14 @@
             "date": date,
             "host": self.host
         }
         url = f'wss://{self.host}{self.path}?{urlencode(query)}'
 
         return url
 
-    def update_url(self):
-        if 'expires_in' not in self.jdata or not self.jdata['expires_in'] \
-            or self.jdata['expires_in'] < time.time() + self.update_interval:
-            cur_time = time.time()
-            url = self.create_url()
-            self.jdata['url'] = url
-            self.jdata['expires_in'] = cur_time + 300
-            jdata = self.load_json(self.jfile)
-            jdata.update({'xunfei': self.jdata})
-            self.write_json(self.jfile, jdata)
-
-    def get_url(self):
-        self.update_url()
-        return self.jdata['url']
-
     def on_error(self, wsapp, error):
         print(f'Error: {error}')
 
     def on_close(self, wsapp, close_status_code, close_msg):
         ...
 
     def on_open(self, wsapp):
@@ -144,37 +129,37 @@
 
     def create(self, message, stream=False):
         jmsg = self.make_message([{
             "role": "user", "content": message
         }])
 
         self.answer = ''
-        url = self.get_url()
+        url = self.create_url()
         ws = websocket.WebSocketApp(
             url, on_message=self.on_message, on_error=self.on_error,
             on_close=self.on_close, on_open=self.on_open,
         )
         ws.json = jmsg
         ws.stream = stream
         ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
         return self.answer
 
 class Chat(Completion):
-    def __init__(self, jfile, model='Spark Lite', history=[]):
-        super().__init__(jfile, model=model)
+    def __init__(self, model='Spark Lite', history=[]):
+        super().__init__(model=model)
         self.history = history
 
     def chat(self, message, stream=False):
         self.history.append({
             "role": "user", "content": message
         })
         jmsg = self.make_message(self.history)
 
         self.answer = ''
-        url = self.get_url()
+        url = self.create_url()
         ws = websocket.WebSocketApp(
             url, on_message=self.on_message, on_error=self.on_error,
             on_close=self.on_close, on_open=self.on_open,
         )
         ws.json = jmsg
         ws.stream = stream
         ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
```

### Comparing `chatchat-0.1.1/setup.py` & `chatchat-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.1.1',
+    version = '0.1.2',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
@@ -20,8 +20,11 @@
         'httpx', 'websocket-client',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3.8',
     ],
+    entry_points = {
+        'console_scripts': ['chatchat=chatchat.__main__:main'],
+    },
 )
```

