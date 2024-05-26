# Comparing `tmp/cadprox-4.8.tar.gz` & `tmp/cadprox-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.8.tar", last modified: Sun May 26 08:38:32 2024, max compression
+gzip compressed data, was "cadprox-4.9.tar", last modified: Sun May 26 08:51:52 2024, max compression
```

## Comparing `cadprox-4.8.tar` & `cadprox-4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.469678 cadprox-4.8/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.8/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:38:32.469678 cadprox-4.8/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.8/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.449677 cadprox-4.8/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.8/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:38:18.000000 cadprox-4.8/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14986 2024-05-26 08:38:07.000000 cadprox-4.8/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.465677 cadprox-4.8/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:38:32.469678 cadprox-4.8/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:38:27.000000 cadprox-4.8/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.154297 cadprox-4.9/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.9/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:51:52.150297 cadprox-4.9/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.9/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.134297 cadprox-4.9/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.9/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:51:37.000000 cadprox-4.9/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14990 2024-05-26 08:51:27.000000 cadprox-4.9/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.150297 cadprox-4.9/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:51:52.154297 cadprox-4.9/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:51:44.000000 cadprox-4.9/setup.py
```

### Comparing `cadprox-4.8/PKG-INFO` & `cadprox-4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.8
+Version: 4.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.8/README.md` & `cadprox-4.9/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.8/app/main.py` & `cadprox-4.9/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.8/app/utils.py` & `cadprox-4.9/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
 def format_caddyfile_system(caddyfile_path=None):
     caddyfile_path = caddyfile_path or get_caddyfile_path(docker=False)
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
-        logger.error(f"Failed to format Caddyfile: {result.stderr}")
+            logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
 def restart_caddy_docker(caddyfile_path=None):
     local_path, docker_path = get_caddyfile_paths(docker=True)
     if local_path and verify_caddyfile_existence_and_permissions(local_path):
         result = subprocess.run(
             ['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', docker_path],
             capture_output=True, text=True
```

### Comparing `cadprox-4.8/cadprox.egg-info/PKG-INFO` & `cadprox-4.9/cadprox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.8
+Version: 4.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.8/setup.py` & `cadprox-4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=4.8,
+    version=4.9,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

