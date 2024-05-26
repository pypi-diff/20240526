# Comparing `tmp/cadprox-5.tar.gz` & `tmp/cadprox-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-5.tar", last modified: Sun May 26 08:59:12 2024, max compression
+gzip compressed data, was "cadprox-5.1.tar", last modified: Sun May 26 09:13:47 2024, max compression
```

## Comparing `cadprox-5.tar` & `cadprox-5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.332359 cadprox-5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5349 2024-05-26 08:59:12.332359 cadprox-5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.316359 cadprox-5/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:58:56.000000 cadprox-5/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14990 2024-05-26 08:58:40.000000 cadprox-5/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.332359 cadprox-5/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5349 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:59:12.336359 cadprox-5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2561 2024-05-26 08:59:02.000000 cadprox-5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.367058 cadprox-5.1/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.1/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:13:47.367058 cadprox-5.1/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.1/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.351058 cadprox-5.1/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.1/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5072 2024-05-26 09:13:27.000000 cadprox-5.1/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    15082 2024-05-26 09:13:14.000000 cadprox-5.1/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.363058 cadprox-5.1/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:13:47.367058 cadprox-5.1/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:13:42.000000 cadprox-5.1/setup.py
```

### Comparing `cadprox-5/PKG-INFO` & `cadprox-5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5
+Version: 5.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5/README.md` & `cadprox-5.1/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-5/app/main.py` & `cadprox-5.1/app/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     format_caddyfile,
     restart_caddy,
     check_port_in_use,
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile,
-    get_caddyfile_path
+    get_caddyfile_path,
+    get_caddyfile_paths
 )
 
 def main():
     """
     The main function of the CADProxy Command Line Tool.
     Parses command line arguments and executes the corresponding commands.
     """
@@ -80,14 +81,15 @@
                 print(f"Warning: Port {backend_server_port} is already in use.")
                 # Continue without exiting
 
             if add_dns_record(subdomain, external_ip, api_token, zone_id):
                 wait_until_resolvable(subdomain)
 
                 local_caddyfile_path = get_caddyfile_path(docker)
+                logger.info(f"Using local Caddyfile path: {local_caddyfile_path}")
 
                 download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
                 if check_domain_exists(subdomain, local_caddyfile_path):
                     raise ValueError(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
 
                 update_caddyfile(subdomain, backend_server_port, local_caddyfile_path, backend_ip)
```

### Comparing `cadprox-5/app/utils.py` & `cadprox-5.1/app/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,15 +148,19 @@
         logger.error(f"Error uploading Caddyfile to S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def get_caddyfile_path(docker=False):
     config_dir = os.path.expanduser('~/cadprox_config')
     if docker:
-        return os.path.join(config_dir, 'Caddyfile_docker')
+        local_path, docker_path = get_caddyfile_paths(docker=True)
+        if local_path:
+            return local_path
+        else:
+            return os.path.join(config_dir, 'Caddyfile_docker')
     return os.path.join(config_dir, 'Caddyfile')
 
 def update_caddyfile(subdomain, port, caddyfile_path=None, backend_ip='localhost'):
     new_entry = f"{subdomain} {{\n    reverse_proxy {backend_ip}:{port}\n}}\n"
     logger.info(f"Adding new entry to Caddyfile at path: {caddyfile_path}")
     logger.info(f"New entry: {new_entry}")
     try:
@@ -225,19 +229,18 @@
 def get_caddyfile_paths(docker):
     if docker:
         try:
             result = subprocess.run(['docker', 'inspect', 'caddy'], capture_output=True, text=True, check=True)
             containers = json.loads(result.stdout)
             if containers:
                 container = containers[0]
-                binds = container['HostConfig']['Binds']
-                for bind in binds:
-                    if '/etc/caddy/Caddyfile' in bind:
-                        local_path, docker_path = bind.split(':')
-                        return local_path, docker_path
+                mounts = container['Mounts']
+                for mount in mounts:
+                    if mount['Destination'] == '/etc/caddy/Caddyfile':
+                        return mount['Source'], mount['Destination']
             return None, None
         except subprocess.CalledProcessError as e:
             logger.error(f"Error inspecting Docker container: {e}")
             return None, None
     else:
         local_path = get_caddyfile_path(docker=False)
         return local_path, None
```

### Comparing `cadprox-5/cadprox.egg-info/PKG-INFO` & `cadprox-5.1/cadprox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5
+Version: 5.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5/setup.py` & `cadprox-5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=5,
+    version=5.1,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

