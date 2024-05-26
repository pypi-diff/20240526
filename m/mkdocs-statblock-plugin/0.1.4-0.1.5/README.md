# Comparing `tmp/mkdocs_statblock_plugin-0.1.4.tar.gz` & `tmp/mkdocs_statblock_plugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_statblock_plugin-0.1.4.tar", last modified: Wed May 22 16:33:08 2024, max compression
+gzip compressed data, was "mkdocs_statblock_plugin-0.1.5.tar", last modified: Sun May 26 08:57:44 2024, max compression
```

## Comparing `mkdocs_statblock_plugin-0.1.4.tar` & `mkdocs_statblock_plugin-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-22 16:33:08.896268 mkdocs_statblock_plugin-0.1.4/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1115 2024-05-20 13:33:14.000000 mkdocs_statblock_plugin-0.1.4/LICENSE
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5829 2024-05-22 16:33:08.896268 mkdocs_statblock_plugin-0.1.4/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5378 2024-05-22 16:17:02.000000 mkdocs_statblock_plugin-0.1.4/README.md
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-22 16:33:08.896268 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2024-05-20 09:39:13.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2136 2024-05-21 13:13:56.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2496 2024-05-22 16:31:23.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/statblock_handler.py
-drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-22 16:33:08.896268 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5829 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)      442 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/entry_points.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       37 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/requires.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       24 2024-05-22 16:33:08.000000 mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/top_level.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2024-05-22 16:33:08.896268 mkdocs_statblock_plugin-0.1.4/setup.cfg
--rw-r--r--   0 johannes  (1000) johannes  (1000)      915 2024-05-22 16:32:32.000000 mkdocs_statblock_plugin-0.1.4/setup.py
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-26 08:57:44.021954 mkdocs_statblock_plugin-0.1.5/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1115 2024-05-20 13:33:14.000000 mkdocs_statblock_plugin-0.1.5/LICENSE
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5829 2024-05-26 08:57:44.021954 mkdocs_statblock_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5378 2024-05-22 16:17:02.000000 mkdocs_statblock_plugin-0.1.5/README.md
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-26 08:57:44.021954 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2024-05-20 09:39:13.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2136 2024-05-21 13:13:56.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2693 2024-05-23 21:25:40.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/statblock_handler.py
+drwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-26 08:57:44.021954 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5829 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      442 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       37 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/requires.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       24 2024-05-26 08:57:43.000000 mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/top_level.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2024-05-26 08:57:44.021954 mkdocs_statblock_plugin-0.1.5/setup.cfg
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      915 2024-05-26 08:57:34.000000 mkdocs_statblock_plugin-0.1.5/setup.py
```

### Comparing `mkdocs_statblock_plugin-0.1.4/LICENSE` & `mkdocs_statblock_plugin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_statblock_plugin-0.1.4/PKG-INFO` & `mkdocs_statblock_plugin-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_statblock_plugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: MkDocs plugin to format YAML within statblock superfences as HTML
 Home-page: https://github.com/johannes-z/mkdocs-statblock-plugin.git
 Author: Johannes Zwirchmayr
 Author-email: johannes.zwirchmayr@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs_statblock_plugin Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: mkdocs_statblock_plugin Version: 0.1.5 Summary:
 MkDocs plugin to format YAML within statblock superfences as HTML Home-page:
 https://github.com/johannes-z/mkdocs-statblock-plugin.git Author: Johannes
 Zwirchmayr Author-email: johannes.zwirchmayr@gmail.com Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 mkdocs>=1.6.0 Requires-Dist: pyyaml Requires-Dist: htmlmin>=0.1.12 # mkdocs
 statblock plugin This mkdocs plugin scans your files for `statblock` code
 blocks and renders them as statblocks. The statblock templates are defined with
```

### Comparing `mkdocs_statblock_plugin-0.1.4/README.md` & `mkdocs_statblock_plugin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py` & `mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/mkdocs_statblock_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin/statblock_handler.py` & `mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin/statblock_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 import re
 import htmlmin
 from jinja2 import Environment, FileSystemLoader
 
 
 def kebabize(string):
+    """Converts a string to kebab-case."""
     if string:
         parts = re.findall(
-            r"[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+", string
+            r"[A-Z]{2,}(?=[A-Z][a-z]+|\b)|[A-Z]?[a-z]+|[A-Z]",
+            string,
         )
         return "-".join(map(str.lower, parts))
     else:
         return ""
 
 
 def modifierFilter(input):
@@ -66,12 +68,17 @@
     def extendMonster(self, data):
         """Extends the monster statblock with the base monster data if it exists in the bestiary."""
         if "monster" not in data:
             return data
         monster_name = data["monster"]
         kebab_name = kebabize(monster_name)
         baseMonsterFilePath = self.bestiary[kebab_name + ".yaml"]
-        if os.path.exists(baseMonsterFilePath):
-            with open(baseMonsterFilePath, "r") as f:
-                monster_data = yaml.safe_load(f)
-            data = {**monster_data, **data}
+
+        if not baseMonsterFilePath or not os.path.exists(baseMonsterFilePath):
+            return {
+                **data,
+                **{"error": f"Monster '{monster_name}' not found in bestiary."},
+            }
+        with open(baseMonsterFilePath, "r") as f:
+            monster_data = yaml.safe_load(f)
+        data = {**monster_data, **data}
         return data
```

### Comparing `mkdocs_statblock_plugin-0.1.4/mkdocs_statblock_plugin.egg-info/PKG-INFO` & `mkdocs_statblock_plugin-0.1.5/mkdocs_statblock_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_statblock_plugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: MkDocs plugin to format YAML within statblock superfences as HTML
 Home-page: https://github.com/johannes-z/mkdocs-statblock-plugin.git
 Author: Johannes Zwirchmayr
 Author-email: johannes.zwirchmayr@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs_statblock_plugin Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: mkdocs_statblock_plugin Version: 0.1.5 Summary:
 MkDocs plugin to format YAML within statblock superfences as HTML Home-page:
 https://github.com/johannes-z/mkdocs-statblock-plugin.git Author: Johannes
 Zwirchmayr Author-email: johannes.zwirchmayr@gmail.com Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 mkdocs>=1.6.0 Requires-Dist: pyyaml Requires-Dist: htmlmin>=0.1.12 # mkdocs
 statblock plugin This mkdocs plugin scans your files for `statblock` code
 blocks and renders them as statblocks. The statblock templates are defined with
```

### Comparing `mkdocs_statblock_plugin-0.1.4/setup.py` & `mkdocs_statblock_plugin-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="mkdocs_statblock_plugin",
-    version="0.1.4",
+    version="0.1.5",
     description="MkDocs plugin to format YAML within statblock superfences as HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/johannes-z/mkdocs-statblock-plugin.git",
     author="Johannes Zwirchmayr",
     author_email="johannes.zwirchmayr@gmail.com",
     packages=find_packages(),
```

