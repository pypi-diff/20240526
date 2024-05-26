# Comparing `tmp/cadprox-5.2.tar.gz` & `tmp/cadprox-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-5.2.tar", last modified: Sun May 26 09:17:26 2024, max compression
+gzip compressed data, was "cadprox-5.3.tar", last modified: Sun May 26 09:24:39 2024, max compression
```

## Comparing `cadprox-5.2.tar` & `cadprox-5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.358988 cadprox-5.2/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.2/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:17:26.358988 cadprox-5.2/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.2/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.342987 cadprox-5.2/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.2/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5237 2024-05-26 09:17:15.000000 cadprox-5.2/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    15082 2024-05-26 09:13:14.000000 cadprox-5.2/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.354987 cadprox-5.2/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:17:26.358988 cadprox-5.2/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:17:21.000000 cadprox-5.2/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:24:39.211338 cadprox-5.3/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.3/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:24:39.211338 cadprox-5.3/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.3/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:24:39.191338 cadprox-5.3/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.3/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5237 2024-05-26 09:17:15.000000 cadprox-5.3/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    15473 2024-05-26 09:23:31.000000 cadprox-5.3/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:24:39.207338 cadprox-5.3/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:24:39.000000 cadprox-5.3/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:24:39.215338 cadprox-5.3/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:24:07.000000 cadprox-5.3/setup.py
```

### Comparing `cadprox-5.2/PKG-INFO` & `cadprox-5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.2
+Version: 5.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.2/README.md` & `cadprox-5.3/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-5.2/app/main.py` & `cadprox-5.3/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-5.2/app/utils.py` & `cadprox-5.3/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,14 +272,24 @@
             ['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', docker_path],
             capture_output=True, text=True
         )
         if result.returncode == 0:
             logger.info("Caddy server reloaded successfully within Docker")
         else:
             logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
+        
+        # Restart the Docker container
+        result = subprocess.run(
+            ['docker', 'restart', 'caddy'],
+            capture_output=True, text=True
+        )
+        if result.returncode == 0:
+            logger.info("Docker container 'caddy' restarted successfully")
+        else:
+            logger.error(f"Failed to restart Docker container 'caddy': {result.stderr}")
 
 def restart_caddy_system(caddyfile_path=None):
     caddyfile_path = caddyfile_path or get_caddyfile_path(docker=False)
     result = subprocess.run(['caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully")
     else:
```

### Comparing `cadprox-5.2/cadprox.egg-info/PKG-INFO` & `cadprox-5.3/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.2
+Version: 5.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.2/setup.py` & `cadprox-5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=5.2,
+    version=5.3,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

