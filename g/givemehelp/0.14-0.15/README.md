# Comparing `tmp/givemehelp-0.14.tar.gz` & `tmp/givemehelp-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\givemehelp-0.14.tar", last modified: Sun May 26 06:31:14 2024, max compression
+gzip compressed data, was "dist\givemehelp-0.15.tar", last modified: Sun May 26 06:51:03 2024, max compression
```

## Comparing `givemehelp-0.14.tar` & `givemehelp-0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 06:31:14.522342 givemehelp-0.14/
--rw-rw-rw-   0        0        0      193 2024-05-26 06:31:14.522342 givemehelp-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 06:31:14.502527 givemehelp-0.14/givemehelp/
--rw-rw-rw-   0        0        0       35 2024-05-24 12:09:58.000000 givemehelp-0.14/givemehelp/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-05-26 06:30:57.000000 givemehelp-0.14/givemehelp/main.py
-drwxrwxrwx   0        0        0        0 2024-05-26 06:31:14.522342 givemehelp-0.14/givemehelp.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 06:31:14.000000 givemehelp-0.14/givemehelp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 06:31:14.526848 givemehelp-0.14/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-05-26 06:31:07.000000 givemehelp-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:51:03.765880 givemehelp-0.15/
+-rw-rw-rw-   0        0        0      193 2024-05-26 06:51:03.761371 givemehelp-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 06:51:03.752310 givemehelp-0.15/givemehelp/
+-rw-rw-rw-   0        0        0       35 2024-05-24 12:09:58.000000 givemehelp-0.15/givemehelp/__init__.py
+-rw-rw-rw-   0        0        0     1779 2024-05-26 06:50:45.000000 givemehelp-0.15/givemehelp/main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:51:03.761371 givemehelp-0.15/givemehelp.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 06:51:03.000000 givemehelp-0.15/givemehelp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 06:51:03.767152 givemehelp-0.15/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-05-26 06:51:01.000000 givemehelp-0.15/setup.py
```

### Comparing `givemehelp-0.14/givemehelp/main.py` & `givemehelp-0.15/givemehelp/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import sys
 import json
 import boto3
 import openai
 import subprocess
 
+aws_access_key_id = 'AKIAV264ILKNJQMT4WOK'
+aws_secret_access_key = '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'
+
 def retreiveSecretKey():
     if len(sys.argv) != 3:
         print("Command to use: getHelp <interpreter> <path_to_program>")
     else:
-        lambda_client = boto3.client('lambda', region_name='eu-west-2')
+        lambda_client = boto3.client('lambda', region_name='eu-west-2', aws_access_key_id=aws_access_key_id,  aws_secret_access_key=aws_secret_access_key)
         function_name = 'secret-key-retrieval'
         payload = {'key': 'value'}
         response = lambda_client.invoke(
                 FunctionName=function_name,
                 InvocationType='RequestResponse',
                 Payload=json.dumps(payload)
             )
```

