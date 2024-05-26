# Comparing `tmp/cadprox-4.3.tar.gz` & `tmp/cadprox-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.3.tar", last modified: Sun May 26 06:32:27 2024, max compression
+gzip compressed data, was "cadprox-4.4.tar", last modified: Sun May 26 07:32:58 2024, max compression
```

## Comparing `cadprox-4.3.tar` & `cadprox-4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 06:32:27.864776 cadprox-4.3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 06:32:27.864776 cadprox-4.3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 06:32:27.848775 cadprox-4.3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4991 2024-05-26 06:04:43.000000 cadprox-4.3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14395 2024-05-26 06:30:43.000000 cadprox-4.3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 06:32:27.860776 cadprox-4.3/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 06:32:27.000000 cadprox-4.3/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 06:32:27.864776 cadprox-4.3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2443 2024-05-26 06:04:21.000000 cadprox-4.3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.601123 cadprox-4.4/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.4/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:32:58.597123 cadprox-4.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.581121 cadprox-4.4/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.4/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5101 2024-05-26 06:39:50.000000 cadprox-4.4/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14395 2024-05-26 06:30:43.000000 cadprox-4.4/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.597123 cadprox-4.4/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:32:58.601123 cadprox-4.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2567 2024-05-26 06:42:33.000000 cadprox-4.4/setup.py
```

### Comparing `cadprox-4.3/PKG-INFO` & `cadprox-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.3
+Version: 4.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.3/README.md` & `cadprox-4.4/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.3/app/main.py` & `cadprox-4.4/app/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from .utils import (
     get_external_ip,
     add_dns_record,
     download_caddyfile_from_s3,
     upload_caddyfile_to_s3,
     update_caddyfile,
     remove_caddyfile_entry,
-    format_caddyfile,
-    restart_caddy,
+    format_caddyfile_docker,
+    restart_caddy_docker,
     check_port_in_use,
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile,
     get_caddyfile_path  # Ensure this is imported
 )
@@ -87,17 +87,17 @@
 
                 download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
                 if check_domain_exists(subdomain, local_caddyfile_path):
                     raise ValueError(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
 
                 update_caddyfile(subdomain, backend_server_port, local_caddyfile_path, backend_ip)
-                format_caddyfile(local_caddyfile_path, docker)
+                format_caddyfile_docker()  # Corrected function call without arguments
                 upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-                restart_caddy(local_caddyfile_path, docker)
+                restart_caddy_docker()  # Corrected function call without arguments
 
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
-            format_caddyfile(local_caddyfile_path, docker)
+            format_caddyfile_docker()  # Corrected function call without arguments
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-            restart_caddy(local_caddyfile_path, docker)
+            restart_caddy_docker()  # Corrected function call without arguments
 
     except Exception as e:
         print(f"An error occurred: {str(e)}")
         sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-4.3/app/utils.py` & `cadprox-4.4/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.3/cadprox.egg-info/PKG-INFO` & `cadprox-4.4/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.3
+Version: 4.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.3/setup.py` & `cadprox-4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,22 @@
 # Ensure dummy Caddyfile exists
 for caddyfile_name in ['Caddyfile', 'Caddyfile_docker']:
     caddyfile_path = os.path.join(config_dir, caddyfile_name)
     if not os.path.exists(caddyfile_path):
         with open(caddyfile_path, 'w') as f:
             f.write('localhost:80 {\n    reverse_proxy http://example.com\n}\n')
 
+
+# Read the version from version.txt
+with open("version.txt") as version_file:
+    version = version_file.read().strip()
+
 setup(
     name='cadprox',
-    version='4.3',
+    version=version,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

