# Comparing `tmp/AZMusicAPI-1.4.3.tar.gz` & `tmp/AZMusicAPI-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AZMusicAPI-1.4.3.tar", last modified: Thu Jan  4 05:42:24 2024, max compression
+gzip compressed data, was "AZMusicAPI-1.4.5.tar", last modified: Sun May 26 08:20:01 2024, max compression
```

## Comparing `AZMusicAPI-1.4.3.tar` & `AZMusicAPI-1.4.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 05:42:24.428607 AZMusicAPI-1.4.3/
-drwxrwxrwx   0        0        0        0 2024-01-04 05:42:24.314449 AZMusicAPI-1.4.3/AZMusicAPI/
--rw-rw-rw-   0        0        0     2229 2024-01-04 05:41:47.000000 AZMusicAPI-1.4.3/AZMusicAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 05:42:24.361323 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/
--rw-rw-rw-   0        0        0     1292 2024-01-04 05:42:23.000000 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-01-04 05:42:24.000000 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 05:42:23.000000 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-04 05:42:23.000000 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-04 05:42:23.000000 AZMusicAPI-1.4.3/AZMusicAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1292 2024-01-04 05:42:24.371857 AZMusicAPI-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-01-04 05:42:24.448651 AZMusicAPI-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-01-04 05:41:47.000000 AZMusicAPI-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:20:01.635536 AZMusicAPI-1.4.5/
+drwxrwxrwx   0        0        0        0 2024-05-26 08:20:01.612126 AZMusicAPI-1.4.5/AZMusicAPI/
+-rw-rw-rw-   0        0        0     3835 2024-05-26 08:19:16.000000 AZMusicAPI-1.4.5/AZMusicAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:20:01.629666 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/
+-rw-rw-rw-   0        0        0     1321 2024-05-26 08:20:01.000000 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-05-26 08:20:01.000000 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:20:01.000000 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 08:20:01.000000 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 08:20:01.000000 AZMusicAPI-1.4.5/AZMusicAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1321 2024-05-26 08:20:01.633536 AZMusicAPI-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:20:01.635536 AZMusicAPI-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      517 2024-05-26 08:19:56.000000 AZMusicAPI-1.4.5/setup.py
```

### Comparing `AZMusicAPI-1.4.3/AZMusicAPI/__init__.py` & `AZMusicAPI-1.4.5/AZMusicAPI/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,94 @@
 import requests
 
 
 # AZ Studio版权所有
 # 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
 
-def getmusic(keyword, api, number=20):
+def getmusic(keyword, api, number=20, server="ncma"):
     number = int(number)
     # 获得指定关键词的歌曲 关键词可为 歌手/歌曲名/专辑名
     # keyword：关键词 number:返回歌曲数量,可选,默认20 api:自行部署neteasecloudmusicapi的地址
     # 返回值说明：正常返回列表  "Error 0"：没有结果 "Error 1":用户未输入
     search_url = api + "search"
-    search_data = {"keywords":keyword}
-    if len(keyword) > 0:
+    if server == "ncma":
+        search_data = {"keywords": keyword}
+        if len(keyword) > 0:
+            try:
+                response_data = requests.get(search_url, params=search_data, timeout=20).json()
+            except:
+                return "NetworkError"
+            songs_data = response_data['result']['songs']
+            if len(response_data['result']['songs']) <= 0:
+                return "Error 0"
+            else:
+                data = []
+                try:
+                    for i in range(len(songs_data)):
+                        artists = ""
+                        for y in range(len(songs_data[i]["artists"])):
+                            if y != 0:
+                                artists = artists + ","
+                            artists = artists + songs_data[i]["artists"][y]["name"]
+                        data.append({"id": songs_data[i]['id'], "name": songs_data[i]['name'], "artists": artists,
+                                     "album": songs_data[i]['album']["name"]})
+                except:
+                    data.append({"id": '-1', "name": 'error', "artists": 'error',
+                                 "album": 'error'})
+                if len(data) > number:
+                    data = data[:number]
+                return data
+        else:
+            return "Error 1"
+    else:
+        if len(keyword) == 0:
+            return "Error 1"
+        search_data = {"key": keyword, "pageSize": number}
         try:
-            response_data = requests.get(search_url, params=search_data,  timeout=20).json()
+            data = requests.get(search_url, params=search_data, timeout=20).json()
         except:
             return "NetworkError"
-        songs_data = response_data['result']['songs']
-        if len(response_data['result']['songs']) <= 0:
-            return "Error 0"
+        if data["result"] != 100:
+            return "Error 1"
         else:
-            data = []
-            try:
-                for i in range(len(songs_data)):
-                    artists = ""
-                    for y in range(len(songs_data[i]["artists"])):
-                        if y != 0:
-                            artists = artists + ","
-                        artists = artists + songs_data[i]["artists"][y]["name"]
-                    data.append({"id": songs_data[i]['id'], "name": songs_data[i]['name'],"artists": artists, "album": songs_data[i]['album']["name"]})
-            except:
-                data.append({"id": '-1', "name": 'error', "artists": 'error',
-                             "album": 'error'})
-            if len(data) > number:
-                data = data[:number]
-            return data
-    else:
-        return "Error 1"
+            data_r = []
+            for i in data["data"]["list"]:
+                artists = ''
+                for j in range(len(i["singer"])):
+                    if j == 0:
+                        artists = i["singer"][j]["name"]
+                    else:
+                        artists = artists + i["singer"][j]["name"]
 
+                data_r.append({"id": i["songmid"], "name": i["name"], "album": i["albumname"], "artists": artists})
+        return data_r
 
-def geturl(id,api):
+def geturl(id, api, server="ncma"):
     # 获取音乐的音频地址
     # id:歌曲的id值  api:自行部署neteasecloudmusicapi的地址
-    # 返回值：正常:返回音频链接  "Error 3":id不正确或无版权
-    search_url = api + "song/url"
-    search_data = {"id": id}
-    try:
-        response_data = requests.get(search_url, params=search_data).json()
-    except:
-        return "NetworkError"
-    try:
-        song_url = response_data['data'][0]["url"]
-    except:
-        return "Error 3"
-    return song_url
-
+    # 返回值：正常:返回音频链接  "Error 3":id不正确或无版权  "Error 4":获取链接失败，建议检查是否登录
+    if server == "nama":
+        search_url = api + "song/url"
+        search_data = {"id": id}
+        try:
+            response_data = requests.get(search_url, params=search_data).json()
+        except:
+            return "NetworkError"
+        try:
+            song_url = response_data['data'][0]["url"]
+        except:
+            return "Error 3"
+        return song_url
+    else:
+        search_url = api + "song/urls"
+        search_data = {"id": id}
+        try:
+            response_data = requests.get(search_url, params=search_data).json()
+        except:
+            return "NetworkError"
+        if response_data["result"] != 100:
+            return "Error 4"
+        try:
+            song_url = response_data['data'][id]
+        except:
+            return "Error 3"
+        return song_url
```

### Comparing `AZMusicAPI-1.4.3/AZMusicAPI.egg-info/PKG-INFO` & `AZMusicAPI-1.4.5/AZMusicAPI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 1.4.3
+Version: 1.4.5
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 
 ### AZ Studio版权所有
 ### 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
-
+> 这是过时的说明文档
 # AZMusicAPI模块使用指南
 
 ## 安装
 
 ```pip install AZMusicAPI```
 
 ## 导入
```

### Comparing `AZMusicAPI-1.4.3/PKG-INFO` & `AZMusicAPI-1.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: AZMusicAPI
-Version: 1.4.3
+Version: 1.4.5
 Summary: 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 Author: AZ Studio
 Project-URL: GitHub, https://github.com/AZ-Studio-2023/AZMusicAPI/
 Description-Content-Type: text/markdown
 
 # AZMusicAPI
 轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links
 
 ### AZ Studio版权所有
 ### 该项目仅供娱乐 请勿用于违法事业 违者与AZ Studio无关
-
+> 这是过时的说明文档
 # AZMusicAPI模块使用指南
 
 ## 安装
 
 ```pip install AZMusicAPI```
 
 ## 导入
```

### Comparing `AZMusicAPI-1.4.3/setup.py` & `AZMusicAPI-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='AZMusicAPI',
-    version='1.4.3',
+    version='1.4.5',
     author='AZ Studio',
     description='轻松访问音乐信息和歌曲音频链接 | Easy access to music information and song audio links',
     long_description = open('readme.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=['AZMusicAPI'],
     install_requires=['requests'],
     project_urls={
```

