# Comparing `tmp/aonet-1.0.3.tar.gz` & `tmp/aonet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aonet-1.0.3.tar", last modified: Tue May 21 06:04:05 2024, max compression
+gzip compressed data, was "aonet-1.0.4.tar", last modified: Sun May 26 14:33:37 2024, max compression
```

## Comparing `aonet-1.0.3.tar` & `aonet-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.597226 aonet-1.0.3/
--rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-21 06:04:05.596940 aonet-1.0.3/PKG-INFO
--rw-rw-r--   0 brent      (501) staff       (20)     1575 2024-05-21 06:02:23.000000 aonet-1.0.3/README.md
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.595221 aonet-1.0.3/aonet/
--rw-r--r--   0 brent      (501) staff       (20)       23 2024-05-21 06:01:07.000000 aonet-1.0.3/aonet/__init__.py
--rw-r--r--   0 brent      (501) staff       (20)     2282 2024-05-21 06:01:49.000000 aonet-1.0.3/aonet/aonet.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.596651 aonet-1.0.3/aonet.egg-info/
--rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      209 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (501) staff       (20)        1 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (501) staff       (20)       12 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/requires.txt
--rw-r--r--   0 brent      (501) staff       (20)        6 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/top_level.txt
--rw-r--r--   0 brent      (501) staff       (20)       38 2024-05-21 06:04:05.597288 aonet-1.0.3/setup.cfg
--rw-r--r--   0 brent      (501) staff       (20)      283 2024-05-21 06:03:56.000000 aonet-1.0.3/setup.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.596243 aonet-1.0.3/tests/
--rw-r--r--   0 brent      (501) staff       (20)      653 2024-05-21 06:02:07.000000 aonet-1.0.3/tests/test.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-26 14:33:37.855062 aonet-1.0.4/
+-rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-26 14:33:37.854784 aonet-1.0.4/PKG-INFO
+-rw-rw-r--   0 brent      (501) staff       (20)     1575 2024-05-21 06:02:23.000000 aonet-1.0.4/README.md
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-26 14:33:37.852145 aonet-1.0.4/aonet/
+-rw-r--r--   0 brent      (501) staff       (20)       23 2024-05-21 06:01:07.000000 aonet-1.0.4/aonet/__init__.py
+-rw-r--r--   0 brent      (501) staff       (20)     2289 2024-05-26 14:24:12.000000 aonet-1.0.4/aonet/aonet.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-26 14:33:37.854476 aonet-1.0.4/aonet.egg-info/
+-rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-26 14:33:37.000000 aonet-1.0.4/aonet.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      209 2024-05-26 14:33:37.000000 aonet-1.0.4/aonet.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (501) staff       (20)        1 2024-05-26 14:33:37.000000 aonet-1.0.4/aonet.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (501) staff       (20)       12 2024-05-26 14:33:37.000000 aonet-1.0.4/aonet.egg-info/requires.txt
+-rw-r--r--   0 brent      (501) staff       (20)        6 2024-05-26 14:33:37.000000 aonet-1.0.4/aonet.egg-info/top_level.txt
+-rw-r--r--   0 brent      (501) staff       (20)       38 2024-05-26 14:33:37.855139 aonet-1.0.4/setup.cfg
+-rw-r--r--   0 brent      (501) staff       (20)      283 2024-05-26 14:25:45.000000 aonet-1.0.4/setup.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-26 14:33:37.854072 aonet-1.0.4/tests/
+-rw-r--r--   0 brent      (501) staff       (20)      607 2024-05-26 14:29:10.000000 aonet-1.0.4/tests/test.py
```

### Comparing `aonet-1.0.3/README.md` & `aonet-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aonet-1.0.3/aonet/aonet.py` & `aonet-1.0.4/aonet/aonet.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,19 @@
         if host is None or host == "":
             host = "api.aonet.ai"
         auth = self.auth
         api_url = self.base_path + api_path
 
         conn = http.client.HTTPSConnection(host)
 
-        data = {
-            "input": input
-        }
+        # data = {
+        #     "input": input
+        # }
 
-        payload = json.dumps(data)
+        payload = json.dumps(input)
 
         headers = (self.headers or {})
         if self.auth_type == AuthType.JWT:
             headers['Authorization'] = 'Bearer ' + auth
         elif self.auth_type == AuthType.API:
             headers['apikey'] = auth
```

### Comparing `aonet-1.0.3/tests/test.py` & `aonet-1.0.4/tests/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import aonet as aonet
+import aonet.aonet as aonet
 
 api_key = "4oipB83LZCpkrVN3i12f38WcBUYH5MR9"
 
 aonet_instance = aonet.AI(api_key)
 
 data = {
-    "input":{
-        "seed": 36446545872,
-        "width": 768,
-        "height": 768,
-        "prompt": "with smoke, half ice and half fire and ultra realistic in detail.wolf, typography, dark fantasy, wildlife photography, vibrant, cinematic and on a black background",
-        "scheduler": "K_EULER",
-        "num_outputs": 1,
-        "guidance_scale": 9,
-        "negative_prompt": "scary, cartoon, painting",
-        "num_inference_steps": 25
+    "input": {
+        "image": "https://replicate.delivery/pbxt/KWDyrcpmbu3DD1MlB85NKy226V6u5uybwi1O9aya1QWw6ozT/famous-photographers-Yousuf-Karsh-1941-churchill-750x954.jpg",
+        "style": "Clay",
+        "prompt": "winston churchill",
+        "negative_prompt": "black and white",
+        "prompt_strength": 4.5,
+        "denoising_strength": 0.66,
+        "instant_id_strength": 0.8
     }
 }
 
-result = aonet_instance.prediction("/predictions/ai/ssd-1b",data)
+result = aonet_instance.prediction("/predictions/ai/face-to-many", data)
 
 print(result)
```

