# Comparing `tmp/cadprox-4.4.tar.gz` & `tmp/cadprox-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.4.tar", last modified: Sun May 26 07:32:58 2024, max compression
+gzip compressed data, was "cadprox-4.5.tar", last modified: Sun May 26 07:44:06 2024, max compression
```

## Comparing `cadprox-4.4.tar` & `cadprox-4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.601123 cadprox-4.4/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.4/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:32:58.597123 cadprox-4.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.581121 cadprox-4.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5101 2024-05-26 06:39:50.000000 cadprox-4.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14395 2024-05-26 06:30:43.000000 cadprox-4.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:32:58.597123 cadprox-4.4/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:32:58.000000 cadprox-4.4/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:32:58.601123 cadprox-4.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2567 2024-05-26 06:42:33.000000 cadprox-4.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.815834 cadprox-4.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:44:06.815834 cadprox-4.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.795833 cadprox-4.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5074 2024-05-26 07:43:04.000000 cadprox-4.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14395 2024-05-26 07:42:30.000000 cadprox-4.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 07:44:06.815834 cadprox-4.5/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 07:44:06.000000 cadprox-4.5/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 07:44:06.819834 cadprox-4.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 07:44:02.000000 cadprox-4.5/setup.py
```

### Comparing `cadprox-4.4/PKG-INFO` & `cadprox-4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.4
+Version: 4.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.4/README.md` & `cadprox-4.5/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.4/app/main.py` & `cadprox-4.5/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     format_caddyfile_docker,
     restart_caddy_docker,
     check_port_in_use,
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile,
-    get_caddyfile_path  # Ensure this is imported
+    get_caddyfile_path
 )
 
 def main():
     """
     The main function of the CADProxy Command Line Tool.
     Parses command line arguments and executes the corresponding commands.
     """
```

### Comparing `cadprox-4.4/app/utils.py` & `cadprox-4.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.4/cadprox.egg-info/PKG-INFO` & `cadprox-4.5/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.4
+Version: 4.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.4/setup.py` & `cadprox-4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=version,
+    version=4.5,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

