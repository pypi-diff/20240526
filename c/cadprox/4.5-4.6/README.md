# Comparing `tmp/cadprox-4.5.tar.gz` & `tmp/cadprox-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.5.tar", last modified: Sun May 26 07:44:06 2024, max compression
+gzip compressed data, was "cadprox-4.6.tar", last modified: Sun May 26 07:51:08 2024, max compression
```

## Comparing `cadprox-4.5.tar` & `cadprox-4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.815834 cadprox-4.5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:44:06.815834 cadprox-4.5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.795833 cadprox-4.5/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.5/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5074 2024-05-26 07:43:04.000000 cadprox-4.5/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14395 2024-05-26 07:42:30.000000 cadprox-4.5/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.815834 cadprox-4.5/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:44:06.819834 cadprox-4.5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 07:44:02.000000 cadprox-4.5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.089044 cadprox-4.6/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.6/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:51:08.089044 cadprox-4.6/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.6/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.073043 cadprox-4.6/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.6/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5198 2024-05-26 07:49:48.000000 cadprox-4.6/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14552 2024-05-26 07:49:25.000000 cadprox-4.6/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:51:08.089044 cadprox-4.6/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:51:08.000000 cadprox-4.6/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:51:08.093044 cadprox-4.6/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 07:50:18.000000 cadprox-4.6/setup.py
```

### Comparing `cadprox-4.5/PKG-INFO` & `cadprox-4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.5
+Version: 4.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.5/README.md` & `cadprox-4.6/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.5/app/main.py` & `cadprox-4.6/app/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,17 +87,17 @@
 
                 download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
                 if check_domain_exists(subdomain, local_caddyfile_path):
                     raise ValueError(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
 
                 update_caddyfile(subdomain, backend_server_port, local_caddyfile_path, backend_ip)
-                format_caddyfile_docker()  # Corrected function call without arguments
+                format_caddyfile_docker(local_caddyfile_path)  # Corrected function call with the local path argument
                 upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-                restart_caddy_docker()  # Corrected function call without arguments
+                restart_caddy_docker(local_caddyfile_path)  # Corrected function call with the local path argument
 
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
-            format_caddyfile_docker()  # Corrected function call without arguments
+            format_caddyfile_docker(local_caddyfile_path)  # Corrected function call with the local path argument
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-            restart_caddy_docker()  # Corrected function call without arguments
+            restart_caddy_docker(local_caddyfile_path)  # Corrected function call with the local path argument
 
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-4.5/app/utils.py` & `cadprox-4.6/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
+    except Exception as e:
+        logger.error(f"Error updating Caddyfile: {e}")
+        logger.error(traceback.format_exc())
 
 def remove_caddyfile_entry(subdomain, caddyfile_path=None):
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
         new_content = re.sub(rf"{subdomain} \{{.*?\}}\n", '', content, flags=re.DOTALL)
         with open(caddyfile_path, 'w') as caddy_file:
@@ -227,15 +230,15 @@
                     local_path, docker_path = bind.split(':')
                     return local_path, docker_path
         return None, None
     except subprocess.CalledProcessError as e:
         logger.error(f"Error inspecting Docker container: {e}")
         return None, None
 
-def format_caddyfile_docker():
+def format_caddyfile_docker(caddyfile_path=None):
     local_path, docker_path = get_caddyfile_paths()
     if local_path and verify_caddyfile_existence_and_permissions(local_path):
         result = subprocess.run(
             ['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', docker_path],
             capture_output=True, text=True
         )
         if result.returncode == 0:
@@ -247,26 +250,26 @@
     caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
-def restart_caddy_docker():
+def restart_caddy_docker(caddyfile_path=None):
     local_path, docker_path = get_caddyfile_paths()
     if local_path and verify_caddyfile_existence_and_permissions(local_path):
         result = subprocess.run(
             ['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', docker_path],
             capture_output=True, text=True
         )
         if result.returncode == 0:
             logger.info("Caddy server reloaded successfully within Docker")
         else:
             logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
-        
+
 def restart_caddy_system(caddyfile_path=None):
     caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully")
     else:
         logger.error(f"Failed to reload Caddy server: {result.stderr}")
```

### Comparing `cadprox-4.5/cadprox.egg-info/PKG-INFO` & `cadprox-4.6/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.5
+Version: 4.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.5/setup.py` & `cadprox-4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=4.5,
+    version=4.6,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

