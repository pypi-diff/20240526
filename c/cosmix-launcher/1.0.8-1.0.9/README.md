# Comparing `tmp/cosmix_launcher-1.0.8.tar.gz` & `tmp/cosmix_launcher-1.0.9.tar.gz`

## Comparing `cosmix_launcher-1.0.8.tar` & `cosmix_launcher-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/license.txt
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/scripts/test.sh
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/net.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/.gitignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/readme.md
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/license.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/scripts/test.sh
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/.gitignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/readme.md
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.8/license.txt` & `cosmix_launcher-1.0.9/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/requirements.txt` & `cosmix_launcher-1.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/__init__.py` & `cosmix_launcher-1.0.9/src/cosmix/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/config.py` & `cosmix_launcher-1.0.9/src/cosmix/api/config.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.9/src/cosmix/api/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,21 +102,27 @@
             hjson.dump(Instance.get_hjson(self), f)
 
     def get_mods(self) -> list[str]:
         mods = []
         mods_dir = self.path_to("mods")
         if os.path.exists(mods_dir):
             for mod_file in os.listdir(mods_dir):
+                if os.path.isdir(mod_file):
+                    continue
                 manifest = java_manifest.from_jar(os.path.join(mods_dir, mod_file))
                 mods.append(mod.Mod.from_data(manifest, mod_file))
         return mods
 
     # Static Methods
     @staticmethod
     def from_config_file(instance_name: str) -> "Instance":
+        if not Instance.exists(instance_name):
+            logger.error("Instance does not exist.")
+            exit(1)
+
         data = None
         path = os.path.join(paths.INSTANCES, instance_name, "config.hjson")
         with open(path, "r") as f:
             data = hjson.load(f)
         if data is None:
             logger.error(f"Failed to load config at {path}")
             exit(1)
```

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.9/src/cosmix/api/logger.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.9/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.9/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/net.py` & `cosmix_launcher-1.0.9/src/cosmix/api/net.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/paths.py` & `cosmix_launcher-1.0.9/src/cosmix/api/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 from os.path import join
 
 
 __all__ = (
     "LOCAL_PATH",
+    "CR_DIR"
     "WORK_DIR",
     "DEPS",
     "INSTANCES",
     "path_to_cr",
+    "path_to_cq_deps",
+    "update_work_dir",
 )
 
 
 LOCAL_PATH = (
     os.environ.get("APPDATA") or
     os.environ.get("XDG_DATA_HOME") or
     join(os.environ["HOME"], ".local", "share")
```

### Comparing `cosmix_launcher-1.0.8/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.9/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/pyproject.toml` & `cosmix_launcher-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.8/readme.md` & `cosmix_launcher-1.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.8/PKG-INFO` & `cosmix_launcher-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.8
+Version: 1.0.9
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

