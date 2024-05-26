# Comparing `tmp/cadprox-4.7.tar.gz` & `tmp/cadprox-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.7.tar", last modified: Sun May 26 08:04:46 2024, max compression
+gzip compressed data, was "cadprox-4.8.tar", last modified: Sun May 26 08:38:32 2024, max compression
```

## Comparing `cadprox-4.7.tar` & `cadprox-4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.912692 cadprox-4.7/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.7/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:04:46.912692 cadprox-4.7/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.7/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.896692 cadprox-4.7/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.7/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:04:31.000000 cadprox-4.7/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14890 2024-05-26 08:03:55.000000 cadprox-4.7/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:04:46.908692 cadprox-4.7/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:04:46.000000 cadprox-4.7/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:04:46.912692 cadprox-4.7/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:04:41.000000 cadprox-4.7/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.469678 cadprox-4.8/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.8/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:38:32.469678 cadprox-4.8/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.8/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.449677 cadprox-4.8/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.8/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:38:18.000000 cadprox-4.8/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14986 2024-05-26 08:38:07.000000 cadprox-4.8/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:38:32.465677 cadprox-4.8/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:38:32.000000 cadprox-4.8/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:38:32.469678 cadprox-4.8/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:38:27.000000 cadprox-4.8/setup.py
```

### Comparing `cadprox-4.7/PKG-INFO` & `cadprox-4.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.7
+Version: 4.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.7/README.md` & `cadprox-4.8/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.7/app/main.py` & `cadprox-4.8/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.7/app/utils.py` & `cadprox-4.8/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,18 @@
     if docker:
         format_caddyfile_docker(caddyfile_path)
     else:
         format_caddyfile_system(caddyfile_path)
 
 def restart_caddy(caddyfile_path=None, docker=False):
     if docker:
+        format_caddyfile_docker(caddyfile_path)
         restart_caddy_docker(caddyfile_path)
     else:
+        format_caddyfile_system(caddyfile_path)
         restart_caddy_system(caddyfile_path)
 
 def is_caddy_running_in_docker():
     try:
         result = subprocess.run(['docker', 'ps', '--filter', 'name=caddy', '--format', '{{.Names}}'], capture_output=True, text=True)
         return 'caddy' in result.stdout.strip().split('\n')
     except Exception as e:
```

### Comparing `cadprox-4.7/cadprox.egg-info/PKG-INFO` & `cadprox-4.8/cadprox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.7
+Version: 4.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.7/setup.py` & `cadprox-4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=4.7,
+    version=4.8,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

