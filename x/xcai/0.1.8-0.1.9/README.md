# Comparing `tmp/xcai-0.1.8.tar.gz` & `tmp/xcai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcai-0.1.8.tar", last modified: Tue May  7 00:38:50 2024, max compression
+gzip compressed data, was "xcai-0.1.9.tar", last modified: Sun May 26 10:59:14 2024, max compression
```

## Comparing `xcai-0.1.8.tar` & `xcai-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-07 00:38:50.831791 xcai-0.1.8/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.8/LICENSE
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      807 2024-05-07 00:38:50.831555 xcai-0.1.8/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.8/README.md
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.8/pyproject.toml
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-05-07 00:38:50.831842 xcai-0.1.8/setup.cfg
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1833 2024-05-07 00:38:28.000000 xcai-0.1.8/setup.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-07 00:38:50.830490 xcai-0.1.8/xcai/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.8/xcai/__init__.py
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5801 2024-05-07 00:36:30.000000 xcai-0.1.8/xcai/xcai.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-07 00:38:50.831320 xcai-0.1.8/xcai.egg-info/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      807 2024-05-07 00:38:50.000000 xcai-0.1.8/xcai.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-05-07 00:38:50.000000 xcai-0.1.8/xcai.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-05-07 00:38:50.000000 xcai-0.1.8/xcai.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-05-07 00:38:50.000000 xcai-0.1.8/xcai.egg-info/requires.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-05-07 00:38:50.000000 xcai-0.1.8/xcai.egg-info/top_level.txt
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-26 10:59:14.504194 xcai-0.1.9/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.9/LICENSE
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      807 2024-05-26 10:59:14.503972 xcai-0.1.9/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.9/README.md
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.9/pyproject.toml
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-05-26 10:59:14.504242 xcai-0.1.9/setup.cfg
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1833 2024-05-26 10:45:51.000000 xcai-0.1.9/setup.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-26 10:59:14.502943 xcai-0.1.9/xcai/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.9/xcai/__init__.py
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5894 2024-05-26 10:58:25.000000 xcai-0.1.9/xcai/xcai.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-05-26 10:59:14.503707 xcai-0.1.9/xcai.egg-info/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      807 2024-05-26 10:59:14.000000 xcai-0.1.9/xcai.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-05-26 10:59:14.000000 xcai-0.1.9/xcai.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-05-26 10:59:14.000000 xcai-0.1.9/xcai.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-05-26 10:59:14.000000 xcai-0.1.9/xcai.egg-info/requires.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-05-26 10:59:14.000000 xcai-0.1.9/xcai.egg-info/top_level.txt
```

### Comparing `xcai-0.1.8/LICENSE` & `xcai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xcai-0.1.8/PKG-INFO` & `xcai-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.8
+Version: 0.1.9
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xcai-0.1.8/setup.py` & `xcai-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcai',  # 包名称，在PyPI中必须唯一
-    version='0.1.8',           # 当前包的版本
+    version='0.1.9',           # 当前包的版本
     author='XiaoChuang.ai',        # 作者名字
     author_email='sup@XiaoChuangai.com',  # 作者邮箱
     #maintainer='Maintainer Name',          # 维护者名字，可选
     #maintainer_email='maintainer.email@example.com',  # 维护者邮箱，可选
     #url='https://github.com/yourusername/your_package',  # 项目的URL，通常是代码仓库的地址
     description='We make AI simple for you',  # 简短的项目描述
     long_description=open('README.md').read(),  # 从README文件中读取的长描述
```

### Comparing `xcai-0.1.8/xcai/xcai.py` & `xcai-0.1.9/xcai/xcai.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             "messages":self.messages,
             "file":kwargs["file"] if "file" in kwargs else "",
             "model":kwargs["model"] if "model" in kwargs else "",
             "with_search_enhance":kwargs["with_search"] if "with_search" in kwargs else False,
             "temperature":kwargs["temperature"] if "temperature" in kwargs else None,
             "top_p":kwargs["top_p"] if "top_p" in kwargs else None,
             "with_rag":kwargs["with_rag"] if "with_rag" in kwargs else False,
+            "model_variant":kwargs["model_variant"] if "model_variant" in kwargs else False,
         }
         return data
     
     def predict(self, **kwargs):
         data = self.data_response(kwargs)
         response = requests.post(self.url, headers=self.headers, data=json.dumps(data), stream=True)
         self.update_model_choice(response.headers.get('model'))
```

### Comparing `xcai-0.1.8/xcai.egg-info/PKG-INFO` & `xcai-0.1.9/xcai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.8
+Version: 0.1.9
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

