# Comparing `tmp/altstore_proxy-1.3.2.tar.gz` & `tmp/altstore_proxy-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.3.2.tar", last modified: Fri May 24 20:02:49 2024, max compression
+gzip compressed data, was "altstore_proxy-1.3.3.tar", last modified: Sat May 25 16:07:43 2024, max compression
```

## Comparing `altstore_proxy-1.3.2.tar` & `altstore_proxy-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 20:02:49.000000 altstore_proxy-1.3.2/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:02:49.340021 altstore_proxy-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 20:02:44.000000 altstore_proxy-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:43.506872 altstore_proxy-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-25 16:07:43.506872 altstore_proxy-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:43.502872 altstore_proxy-1.3.3/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:43.506872 altstore_proxy-1.3.3/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:07:43.506872 altstore_proxy-1.3.3/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 16:07:43.000000 altstore_proxy-1.3.3/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:07:43.506872 altstore_proxy-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-25 16:07:39.000000 altstore_proxy-1.3.3/setup.py
```

### Comparing `altstore_proxy-1.3.2/LICENSE.md` & `altstore_proxy-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.3.2/PKG-INFO` & `altstore_proxy-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.3.2
+Version: 1.3.3
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.3.2/README.md` & `altstore_proxy-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.3.2/altstore_proxy/providers/notifications.py` & `altstore_proxy-1.3.3/altstore_proxy/providers/notifications.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # AltStore-Proxy
 # Project by https://github.com/rix1337
 
 import json
-import os
 
 import requests
 
 
 def readable_size(size):
     if size:  # integer byte value
         power = 2 ** 10
@@ -47,15 +46,15 @@
             },
             'fields': [
                 {
                     'name': "Size",
                     'value': readable_size(app['size']),
                 }, {
                     'name': "Download",
-                    'value': f'[{os.path.basename(app["filename"])}]({app["downloadURL"]})'
+                    'value': f'[{app["filename"]}]({app["downloadURL"]})'
                 }
 
             ]
         }]
     }
 
     try:
```

### Comparing `altstore_proxy-1.3.2/altstore_proxy/providers/version.py` & `altstore_proxy-1.3.3/altstore_proxy/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # AltStore-Proxy
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.3.2"
+    return "1.3.3"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `altstore_proxy-1.3.2/altstore_proxy/run.py` & `altstore_proxy-1.3.3/altstore_proxy/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,36 +42,38 @@
     response = requests.get(url, stream=True, allow_redirects=True)
     total_size_in_bytes = int(response.headers.get('content-length', 0))
 
     # Resolve the actual URL if the provided URL is a shortened URL
     if "tinyurl.com" in url:
         url = response.url
 
-    filename = os.path.join(shared_state.values["cache"], os.path.basename(url))
+    file_path = os.path.join(shared_state.values["cache"], os.path.basename(url))
+    file_name = os.path.basename(file_path)
 
-    os.makedirs(os.path.dirname(filename), exist_ok=True)
+
+    os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
     # Check if file already exists and compare sizes
-    if os.path.exists(filename):
-        existing_file_size = os.path.getsize(filename)
+    if os.path.exists(file_path):
+        existing_file_size = os.path.getsize(file_path)
         if existing_file_size == total_size_in_bytes:
-            print(f"File {filename} already exists with the same size. Skipping download.")
-            return filename, True
+            print(f"File {file_path} already exists with the same size. Skipping download.")
+            return file_name, True
 
-    print(f"Downloading {url} to {filename}")
+    print(f"Downloading {url} to {file_path}")
     progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
-    with open(filename, 'wb') as f:
+    with open(file_path, 'wb') as f:
         for data in response.iter_content(chunk_size=1024):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
 
-    return filename, False
+    return file_name, False
 
 
 def update_json_proxy(shared_state_dict, shared_state_lock):
     shared_state.set_state(shared_state_dict, shared_state_lock)
 
     try:
         while True:
@@ -88,15 +90,15 @@
 
             for repo in shared_state.values["repos_to_cache"]:
                 response = requests.get(repo)
                 data = response.json()
                 for app in data['apps']:
                     print("Found " + app['name'] + ", v." + app['version'])
                     app['filename'], skipped = download_and_cache_ipa(app['downloadURL'])
-                    app['downloadURL'] = shared_state.values["baseurl"] + '/' + app['filename']
+                    app['downloadURL'] = shared_state.values["baseurl"] + '/cache/' + app['filename']
 
                     if not skipped:
                         if shared_state.values['discord_webhook']:
                             notifications.discord_webhook(shared_state, app)
 
                 merged_json['apps'].extend(data['apps'])
```

### Comparing `altstore_proxy-1.3.2/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.3.3/altstore_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.3.2
+Version: 1.3.3
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.3.2/setup.py` & `altstore_proxy-1.3.3/setup.py`

 * *Files identical despite different names*

