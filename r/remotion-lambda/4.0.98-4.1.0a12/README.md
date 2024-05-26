# Comparing `tmp/remotion_lambda-4.0.98.tar.gz` & `tmp/remotion_lambda-4.1.0a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.98.tar", last modified: Fri Jan 26 08:51:25 2024, max compression
+gzip compressed data, was "remotion_lambda-4.1.0a12.tar", last modified: Sun Aug  6 15:58:27 2023, max compression
```

## Comparing `remotion_lambda-4.0.98.tar` & `remotion_lambda-4.1.0a12.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2024-01-26 08:51:25.173323 remotion_lambda-4.0.98/
--rw-r--r--   0 jonathanburger   (501) staff       (20)     2496 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/LICENSE
--rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2024-01-26 08:51:25.173115 remotion_lambda-4.0.98/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)       29 2024-01-23 08:16:26.000000 remotion_lambda-4.0.98/README.md
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2024-01-26 08:51:25.171486 remotion_lambda-4.0.98/remotion_lambda/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      490 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/remotion_lambda/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)    15406 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/remotion_lambda/models.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     9069 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/remotion_lambda/remotionclient.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2024-01-26 08:38:06.000000 remotion_lambda-4.0.98/remotion_lambda/version.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2024-01-26 08:51:25.172891 remotion_lambda-4.0.98/remotion_lambda.egg-info/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2024-01-26 08:51:25.000000 remotion_lambda-4.0.98/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)      476 2024-01-26 08:51:25.000000 remotion_lambda-4.0.98/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2024-01-26 08:51:25.000000 remotion_lambda-4.0.98/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       23 2024-01-26 08:51:25.000000 remotion_lambda-4.0.98/remotion_lambda.egg-info/requires.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2024-01-26 08:51:25.000000 remotion_lambda-4.0.98/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2024-01-26 08:51:25.173359 remotion_lambda-4.0.98/setup.cfg
--rw-r--r--   0 jonathanburger   (501) staff       (20)      941 2024-01-23 08:16:26.000000 remotion_lambda-4.0.98/setup.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2024-01-26 08:51:25.172673 remotion_lambda-4.0.98/tests/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/tests/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/tests/test_get_render_progress_client.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      831 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/tests/test_render_client_render_media.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      870 2024-01-19 09:26:53.000000 remotion_lambda-4.0.98/tests/test_render_client_render_still.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870838 remotion_lambda-4.1.0a12/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2023-08-06 15:58:27.870663 remotion_lambda-4.1.0a12/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.869636 remotion_lambda-4.1.0a12/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       91 2023-08-06 15:40:13.000000 remotion_lambda-4.1.0a12/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870149 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-06 15:58:27.870887 remotion_lambda-4.1.0a12/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870482 remotion_lambda-4.1.0a12/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.98/LICENSE` & `remotion_lambda-4.1.0a12/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 
 Support is provided on a best-we-can-do basis via GitHub Issues and Discord.
 
 ## Company license
 
 You are required to obtain a company license to use Remotion if you are not within the group of entities eligible for a free license. This license will enable you to use Remotion for the allowed use cases specified in the free license, and give you access to prioritized support (read the [Support Policy](/docs/support)).
 
-Visit [remotion.pro](https://www.remotion.pro) for pricing and to buy a license.
+Visit [companies.remotion.dev](https://companies.remotion.dev) for pricing and to buy a license.
```

### Comparing `remotion_lambda-4.0.98/setup.py` & `remotion_lambda-4.1.0a12/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import os
 import setuptools
 from remotion_lambda.version import VERSION
 
-def load_requirements(path):
-    with open(path) as f:
-        return [line.strip() for line in f]
-
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
-requirements = load_requirements('requirements.txt')
-
 setuptools.setup(
     name="remotion_lambda",
     version=VERSION,
     author="Jonny Burger",
     author_email="jonny@remotion.dev",
     description="Remotion Lambda client",
     long_description_content_type="text/markdown",
@@ -23,9 +17,9 @@
 
     ],
     long_description="Remotion is a framework for creating videos programmatically using React.",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     # Name of the python package
     py_modules=["remotion-lambda"],
-    install_requires=requirements,
+
 )
```

### Comparing `remotion_lambda-4.0.98/tests/test_render_client_render_still.py` & `remotion_lambda-4.1.0a12/tests/test_render_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from unittest import TestCase
 
-from remotion_lambda.models import RenderStillParams
+from remotion_lambda.models import RenderParams
 from remotion_lambda.remotionclient import RemotionClient
 
 
 class TestRemotionClient(TestCase):
     def test_remotion_construct_request(self):
         client = RemotionClient(region="us-east-1",
                                 serve_url="testbed",
                                 function_name="remotion-render")
-        render_still_params = RenderStillParams(
-            composition="still-helloworld",
-            input_props={
-                'message': 'Hello from props!'
+        render_params = RenderParams(
+            composition="react-svg",
+            data={
+                'hi': 'there'
             },
         )
 
         self.assertEqual(client.region, "us-east-1")
-        self.assertIsNotNone(render_still_params)
-        self.assertIsNotNone(render_still_params.input_props)
-        print(client.construct_render_request(
-            render_params=render_still_params, render_type='still'))
+        self.assertIsNotNone(render_params)
+        self.assertIsNotNone(render_params.data)
+        print(client.construct_render_request(render_params=render_params))
```

