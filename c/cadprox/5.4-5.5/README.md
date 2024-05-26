# Comparing `tmp/cadprox-5.4.tar.gz` & `tmp/cadprox-5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-5.4.tar", last modified: Sun May 26 09:55:45 2024, max compression
+gzip compressed data, was "cadprox-5.5.tar", last modified: Sun May 26 10:38:48 2024, max compression
```

## Comparing `cadprox-5.4.tar` & `cadprox-5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:55:45.479924 cadprox-5.4/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.4/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:55:45.479924 cadprox-5.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:55:45.459924 cadprox-5.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5237 2024-05-26 09:17:15.000000 cadprox-5.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    15912 2024-05-26 09:48:44.000000 cadprox-5.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:55:45.475924 cadprox-5.4/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:55:45.000000 cadprox-5.4/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:55:45.479924 cadprox-5.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:55:38.000000 cadprox-5.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 10:38:48.519311 cadprox-5.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 10:38:48.519311 cadprox-5.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 10:38:48.499310 cadprox-5.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5302 2024-05-26 10:32:43.000000 cadprox-5.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    15912 2024-05-26 09:48:44.000000 cadprox-5.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 10:38:48.515311 cadprox-5.5/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 10:38:48.000000 cadprox-5.5/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 10:38:48.519311 cadprox-5.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 10:38:42.000000 cadprox-5.5/setup.py
```

### Comparing `cadprox-5.4/PKG-INFO` & `cadprox-5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.4
+Version: 5.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.4/README.md` & `cadprox-5.5/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-5.4/app/main.py` & `cadprox-5.5/app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
             if not s3_caddy_filename:
                 s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
 
             external_ip = get_external_ip()
             if not external_ip:
                 raise ValueError("Failed to retrieve external IP address.")
 
-            backend_ip = '172.17.0.1' if docker else 'localhost'
+            #backend_ip = '172.17.0.1' if docker else 'localhost'
+            backend_ip = 'localhost' if docker else 'localhost'
 
             if check_port_in_use(backend_server_port):
                 print(f"Warning: Port {backend_server_port} is already in use.")
                 # Continue without exiting
 
             if add_dns_record(subdomain, external_ip, api_token, zone_id):
                 wait_until_resolvable(subdomain)
```

### Comparing `cadprox-5.4/app/utils.py` & `cadprox-5.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-5.4/cadprox.egg-info/PKG-INFO` & `cadprox-5.5/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.4
+Version: 5.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.4/setup.py` & `cadprox-5.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=5.4,
+    version=5.5,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

