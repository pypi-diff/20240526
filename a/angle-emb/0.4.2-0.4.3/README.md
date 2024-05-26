# Comparing `tmp/angle_emb-0.4.2.tar.gz` & `tmp/angle_emb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angle_emb-0.4.2.tar", last modified: Sat May 25 02:29:00 2024, max compression
+gzip compressed data, was "angle_emb-0.4.3.tar", last modified: Sun May 26 05:30:34 2024, max compression
```

## Comparing `angle_emb-0.4.2.tar` & `angle_emb-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.570639 angle_emb-0.4.2/
--rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.2/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-25 02:29:00.570918 angle_emb-0.4.2/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)    16565 2024-05-25 02:28:23.000000 angle_emb-0.4.2/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.561690 angle_emb-0.4.2/angle_emb/
--rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-25 02:28:33.000000 angle_emb-0.4.2/angle_emb/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)    70668 2024-05-25 02:28:23.000000 angle_emb-0.4.2/angle_emb/angle.py
--rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-22 08:19:50.000000 angle_emb-0.4.2/angle_emb/angle_trainer.py
--rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.2/angle_emb/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-25 02:29:00.570097 angle_emb-0.4.2/angle_emb.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/entry_points.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.2/angle_emb.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-25 02:29:00.000000 angle_emb-0.4.2/angle_emb.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-25 02:29:00.572219 angle_emb-0.4.2/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-25 02:28:33.000000 angle_emb-0.4.2/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.302784 angle_emb-0.4.3/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1061 2024-01-15 11:58:12.000000 angle_emb-0.4.3/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-26 05:30:34.303133 angle_emb-0.4.3/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)    16565 2024-05-25 02:28:23.000000 angle_emb-0.4.3/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.284288 angle_emb-0.4.3/angle_emb/
+-rw-r--r--   0 seanlee    (501) staff       (20)       70 2024-05-26 05:29:29.000000 angle_emb-0.4.3/angle_emb/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    70613 2024-05-26 05:29:24.000000 angle_emb-0.4.3/angle_emb/angle.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    13833 2024-05-22 08:19:50.000000 angle_emb-0.4.3/angle_emb/angle_trainer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)      512 2024-05-21 09:01:40.000000 angle_emb-0.4.3/angle_emb/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2024-05-26 05:30:34.302147 angle_emb-0.4.3/angle_emb.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)    17282 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      355 2024-05-26 05:30:34.000000 angle_emb-0.4.3/angle_emb.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       63 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/entry_points.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2024-01-15 12:03:51.000000 angle_emb-0.4.3/angle_emb.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       87 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)       10 2024-05-26 05:30:33.000000 angle_emb-0.4.3/angle_emb.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      202 2024-05-26 05:30:34.306904 angle_emb-0.4.3/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1529 2024-05-26 05:29:29.000000 angle_emb-0.4.3/setup.py
```

### Comparing `angle_emb-0.4.2/LICENSE` & `angle_emb-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.2/PKG-INFO` & `angle_emb-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle_emb
-Version: 0.4.2
+Version: 0.4.3
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle_emb Version: 0.4.2 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle_emb Version: 0.4.3 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `angle_emb-0.4.2/README.md` & `angle_emb-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.2/angle_emb/angle.py` & `angle_emb-0.4.3/angle_emb/angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1309,16 +1309,15 @@
                     model = get_peft_model(model, peft_config)
                 self.backbone = model
             else:
                 if pretrained_model_path is not None:
                     logger.info(f'Load pretrained model from {pretrained_model_path}')
                 self.backbone = AutoModel.from_pretrained(
                     pretrained_model_path or model_name_or_path,
-                    trust_remote_code=True,
-                    torch_dtype=torch_dtype or "auto")
+                    trust_remote_code=True)
 
         if train_mode and self.apply_lora:
             self.backbone.print_trainable_parameters()
 
         self.backbone.config.use_cache = False
         self.pooler = Pooler(
             self.backbone,
```

### Comparing `angle_emb-0.4.2/angle_emb/angle_trainer.py` & `angle_emb-0.4.3/angle_emb/angle_trainer.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.2/angle_emb/utils.py` & `angle_emb-0.4.3/angle_emb/utils.py`

 * *Files identical despite different names*

### Comparing `angle_emb-0.4.2/angle_emb.egg-info/PKG-INFO` & `angle_emb-0.4.3/angle_emb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angle-emb
-Version: 0.4.2
+Version: 0.4.3
 Summary: AnglE-optimize Text Embeddings
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: angle_emb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: angle-emb Version: 0.4.2 Summary: AnglE-optimize
+Metadata-Version: 2.1 Name: angle-emb Version: 0.4.3 Summary: AnglE-optimize
 Text Embeddings Author: sean lee Author-email: xmlee97@gmail.com Keywords:
 angle_emb Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `angle_emb-0.4.2/setup.py` & `angle_emb-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='angle_emb',
-    version='0.4.2',
+    version='0.4.3',
     description='AnglE-optimize Text Embeddings',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

