# Comparing `tmp/cadprox-4.6.tar.gz` & `tmp/cadprox-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.6.tar", last modified: Sun May 26 07:51:08 2024, max compression
+gzip compressed data, was "cadprox-4.7.tar", last modified: Sun May 26 08:04:46 2024, max compression
```

## Comparing `cadprox-4.6.tar` & `cadprox-4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.089044 cadprox-4.6/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.6/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:51:08.089044 cadprox-4.6/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.6/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.073043 cadprox-4.6/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.6/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5198 2024-05-26 07:49:48.000000 cadprox-4.6/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14552 2024-05-26 07:49:25.000000 cadprox-4.6/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.089044 cadprox-4.6/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:51:08.093044 cadprox-4.6/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 07:50:18.000000 cadprox-4.6/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.912692 cadprox-4.7/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.7/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:04:46.912692 cadprox-4.7/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.7/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.896692 cadprox-4.7/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.7/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:04:31.000000 cadprox-4.7/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14890 2024-05-26 08:03:55.000000 cadprox-4.7/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.908692 cadprox-4.7/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:04:46.912692 cadprox-4.7/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:04:41.000000 cadprox-4.7/setup.py
```

### Comparing `cadprox-4.6/PKG-INFO` & `cadprox-4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.6
+Version: 4.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.6/README.md` & `cadprox-4.7/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.6/app/main.py` & `cadprox-4.7/app/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from .utils import (
     get_external_ip,
     add_dns_record,
     download_caddyfile_from_s3,
     upload_caddyfile_to_s3,
     update_caddyfile,
     remove_caddyfile_entry,
-    format_caddyfile_docker,
-    restart_caddy_docker,
+    format_caddyfile,
+    restart_caddy,
     check_port_in_use,
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile,
     get_caddyfile_path
 )
@@ -87,17 +87,17 @@
 
                 download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
                 if check_domain_exists(subdomain, local_caddyfile_path):
                     raise ValueError(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
 
                 update_caddyfile(subdomain, backend_server_port, local_caddyfile_path, backend_ip)
-                format_caddyfile_docker(local_caddyfile_path)  # Corrected function call with the local path argument
+                format_caddyfile(local_caddyfile_path, docker)
                 upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-                restart_caddy_docker(local_caddyfile_path)  # Corrected function call with the local path argument
+                restart_caddy(local_caddyfile_path, docker)
 
         if args.command in ['remove', 'docker_remove']:
             subdomain = args.subdomain
             docker = args.command == 'docker_remove'
             if not subdomain:
                 raise ValueError("Error: Subdomain must be provided.")
 
@@ -109,17 +109,17 @@
             )
 
             s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
             local_caddyfile_path = get_caddyfile_path(docker)
 
             download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
             remove_caddyfile_entry(subdomain, local_caddyfile_path)
-            format_caddyfile_docker(local_caddyfile_path)  # Corrected function call with the local path argument
+            format_caddyfile(local_caddyfile_path, docker)
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-            restart_caddy_docker(local_caddyfile_path)  # Corrected function call with the local path argument
+            restart_caddy(local_caddyfile_path, docker)
 
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-4.6/app/utils.py` & `cadprox-4.7/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,16 @@
     config_dir = os.path.expanduser('~/cadprox_config')
     if docker:
         return os.path.join(config_dir, 'Caddyfile_docker')
     return os.path.join(config_dir, 'Caddyfile')
 
 def update_caddyfile(subdomain, port, caddyfile_path=None, backend_ip='localhost'):
     new_entry = f"{subdomain} {{\n    reverse_proxy {backend_ip}:{port}\n}}\n"
+    logger.info(f"Adding new entry to Caddyfile at path: {caddyfile_path}")
+    logger.info(f"New entry: {new_entry}")
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
@@ -214,64 +216,68 @@
             logger.error(f"Caddyfile at {caddyfile_path} is not readable. Check permissions.")
             return False
     else:
         logger.error(f"Caddyfile at {caddyfile_path} does not exist")
         return False
     return True
 
-def get_caddyfile_paths():
-    try:
-        result = subprocess.run(['docker', 'inspect', 'caddy'], capture_output=True, text=True, check=True)
-        containers = json.loads(result.stdout)
-        if containers:
-            container = containers[0]
-            binds = container['HostConfig']['Binds']
-            for bind in binds:
-                if '/etc/caddy/Caddyfile' in bind:
-                    local_path, docker_path = bind.split(':')
-                    return local_path, docker_path
-        return None, None
-    except subprocess.CalledProcessError as e:
-        logger.error(f"Error inspecting Docker container: {e}")
-        return None, None
+def get_caddyfile_paths(docker):
+    if docker:
+        try:
+            result = subprocess.run(['docker', 'inspect', 'caddy'], capture_output=True, text=True, check=True)
+            containers = json.loads(result.stdout)
+            if containers:
+                container = containers[0]
+                binds = container['HostConfig']['Binds']
+                for bind in binds:
+                    if '/etc/caddy/Caddyfile' in bind:
+                        local_path, docker_path = bind.split(':')
+                        return local_path, docker_path
+            return None, None
+        except subprocess.CalledProcessError as e:
+            logger.error(f"Error inspecting Docker container: {e}")
+            return None, None
+    else:
+        local_path = get_caddyfile_path(docker=False)
+        return local_path, None
 
 def format_caddyfile_docker(caddyfile_path=None):
-    local_path, docker_path = get_caddyfile_paths()
+    local_path, docker_path = get_caddyfile_paths(docker=True)
     if local_path and verify_caddyfile_existence_and_permissions(local_path):
         result = subprocess.run(
             ['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', docker_path],
             capture_output=True, text=True
         )
         if result.returncode == 0:
             logger.info("Caddyfile formatted successfully within Docker")
         else:
             logger.error(f"Failed to format Caddyfile within Docker: {result.stderr}")
 
 def format_caddyfile_system(caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
+    caddyfile_path = caddyfile_path or get_caddyfile_path(docker=False)
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
 def restart_caddy_docker(caddyfile_path=None):
-    local_path, docker_path = get_caddyfile_paths()
+    local_path, docker_path = get_caddyfile_paths(docker=True)
     if local_path and verify_caddyfile_existence_and_permissions(local_path):
         result = subprocess.run(
             ['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', docker_path],
             capture_output=True, text=True
         )
         if result.returncode == 0:
             logger.info("Caddy server reloaded successfully within Docker")
         else:
             logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
 def restart_caddy_system(caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
+    caddyfile_path = caddyfile_path or get_caddyfile_path(docker=False)
     result = subprocess.run(['caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully")
     else:
         logger.error(f"Failed to reload Caddy server: {result.stderr}")
 
 def check_port_in_use(port):
```

### Comparing `cadprox-4.6/cadprox.egg-info/PKG-INFO` & `cadprox-4.7/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.6
+Version: 4.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.6/setup.py` & `cadprox-4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=4.6,
+    version=4.7,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

