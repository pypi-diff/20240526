# Comparing `tmp/extrautilities-1.2.tar.gz` & `tmp/extrautilities-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.2.tar", last modified: Fri May 24 15:45:09 2024, max compression
+gzip compressed data, was "extrautilities-1.3.tar", last modified: Sun May 26 08:26:45 2024, max compression
```

## Comparing `extrautilities-1.2.tar` & `extrautilities-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:45:09.713157 extrautilities-1.2/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:45:09.700949 extrautilities-1.2/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.2/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.2/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.2/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.2/ExtraUtils/callbackVoid.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.2/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.2/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     1274 2024-05-24 15:44:21.000000 extrautilities-1.2/ExtraUtils/validate_dict.py
--rw-rw-rw-   0        0        0     3349 2024-05-24 15:45:09.713157 extrautilities-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:45:09.711650 extrautilities-1.2/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-05-24 15:45:09.000000 extrautilities-1.2/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-24 15:45:09.000000 extrautilities-1.2/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:45:09.000000 extrautilities-1.2/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:45:09.000000 extrautilities-1.2/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-24 15:45:09.000000 extrautilities-1.2/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:45:09.713700 extrautilities-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-24 15:45:06.000000 extrautilities-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.507007 extrautilities-1.3/
+drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.492727 extrautilities-1.3/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.3/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.3/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.3/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.3/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.3/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.3/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.3/ExtraUtils/validate_dict.py
+-rw-rw-rw-   0        0        0     3349 2024-05-26 08:26:45.506004 extrautilities-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 08:26:45.505505 extrautilities-1.3/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3349 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 08:26:45.000000 extrautilities-1.3/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:26:45.507007 extrautilities-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-05-26 08:26:40.000000 extrautilities-1.3/setup.py
```

### Comparing `extrautilities-1.2/ExtraUtils/RateLimit.py` & `extrautilities-1.3/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.2/ExtraUtils/asyncTokens.py` & `extrautilities-1.3/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.2/ExtraUtils/getFileContent.py` & `extrautilities-1.3/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.2/ExtraUtils/timeBasedToken.py` & `extrautilities-1.3/ExtraUtils/timeBasedToken.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.2/ExtraUtils/validate_dict.py` & `extrautilities-1.3/ExtraUtils/validate_dict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 def validate_dict(format:dict, data:dict)->bool:
     for key, rule in format.items():
         if rule.get["__required"] and key not in data:
             print(f"❌  Missing required field {key}. @channel_points.py(validate_dict)")
             return False
+        
         if rule.get("__type"):
             tpe = rule.get("__type")
             if not isinstance(data[key], tpe):
-                print(f"❌  Invalid type for {key}. @channel_points.py(validate_dict)")
+                print(f"❌  Invalid type for {key} expecting {tpe}. @channel_points.py(validate_dict)")
                 return False
+            if isinstance(data[key], dict):
+                if not validate_dict(tpe, data[key]):
+                    return False
+            
+        if isinstance(rule.get("__value"), list) and data[key] not in rule.get("__value"):
+            print(f"❌  Invalid value for {key} expected to be a value contained in {rule.get("__value")}. @channel_points.py(validate_dict)")
+            return False
+        
+        if rule.get("__range") and (isinstance(data[key], int) or isinstance(data[key], float)):
+            min, max = rule.get("__range").split("..")
+            min = int(min) if min else -999_999_999.0
+            max = int(max) if max else 999_999_999.0
+            dig = data[key]
+            if isinstance(data[key], int):
+                dig = float(data[key])
+            if not min <= dig <= max:
+                    print(f"❌  Invalid length for {key}. @channel_points.py(validate_dict)\n->length must be between {min} and {max}")
+                    return False
+            
         if rule.get("__length"):
             min, max = rule.get("__length").split("..")
             min = int(min) if min else -999_999_999
             max = int(max) if max else 999_999_999
-            if not isinstance(data[key], int) and not isinstance(data[key], dict):
+            if not isinstance(data[key], dict):
                 if not min <= len(data[key]) <= max:
-                    print(f"❌  Invalid length for {key}. @channel_points.py(validate_dict)\n->length must be between {min} and {max}")
-                    return False
-            elif not isinstance(data[key], dict):
-                if not min <= data[key] <= max:
                     print(f"❌  Invalid value for {key}. @channel_points.py(validate_dict)\n->value must be between {min} and {max}")
-                    return False
+                    return False
+    return True
```

### Comparing `extrautilities-1.2/PKG-INFO` & `extrautilities-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.2
+Version: 1.3
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.2/README.md` & `extrautilities-1.3/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.2/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.3/extrautilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.2
+Version: 1.3
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.2/setup.py` & `extrautilities-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

