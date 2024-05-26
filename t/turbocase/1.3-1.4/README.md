# Comparing `tmp/turbocase-1.3.tar.gz` & `tmp/turbocase-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbocase-1.3.tar", last modified: Fri May 17 13:45:46 2024, max compression
+gzip compressed data, was "turbocase-1.4.tar", last modified: Sun May 26 18:44:54 2024, max compression
```

## Comparing `turbocase-1.3.tar` & `turbocase-1.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.936815 turbocase-1.3/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-17 13:45:46.936815 turbocase-1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2443 2024-05-15 14:44:48.000000 turbocase-1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 13:45:46.936815 turbocase-1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-17 13:45:29.000000 turbocase-1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.933482 turbocase-1.3/turbocase/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.3/turbocase/__init__.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 14:42:59.000000 turbocase-1.3/turbocase/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-17 12:51:54.000000 turbocase-1.3/turbocase/cases.py
--rw-r--r--   0 root         (0) root         (0)     8225 2024-05-17 13:31:10.000000 turbocase-1.3/turbocase/kicad.py
--rw-r--r--   0 root         (0) root         (0)      845 2024-05-17 13:19:26.000000 turbocase-1.3/turbocase/parts.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-17 12:58:48.000000 turbocase-1.3/turbocase/scad.py
--rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.3/turbocase/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.936815 turbocase-1.3/turbocase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.718432 turbocase-1.4/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-26 18:44:54.718432 turbocase-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-17 13:48:51.000000 turbocase-1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 18:44:54.718432 turbocase-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-26 18:42:45.000000 turbocase-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.715099 turbocase-1.4/turbocase/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.4/turbocase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-17 16:22:48.000000 turbocase-1.4/turbocase/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-26 14:19:02.000000 turbocase-1.4/turbocase/cases.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2024-05-26 14:19:02.000000 turbocase-1.4/turbocase/kicad.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-26 14:26:10.000000 turbocase-1.4/turbocase/scad.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.4/turbocase/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 18:44:54.718432 turbocase-1.4/turbocase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-26 18:44:54.000000 turbocase-1.4/turbocase.egg-info/top_level.txt
```

### Comparing `turbocase-1.3/LICENSE.txt` & `turbocase-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turbocase-1.3/README.md` & `turbocase-1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,31 +20,38 @@
 
 An example of a KiCAD PCB with a case outline on `User.6`:
 ![KiCAD PCB with case outline](images/kicad.png)
 
 The generated case from this file:
 ![OpenSCAD model of the generated case](images/scad.png)
 
-
 ## Installation
 
 ```shell-session
 $ pip install turbocase
 ```
 
 ## Usage
 
 1. Create a case outline in the `User.6` layer using the line drawing tools.
 2. Add the `Height` property to the connector footprints that need to be in the case export
 3. Ensure the screw holes for the PCB are MountingHole footprints
 4. Run the turbocase tool to make an OpenSCAD file:
+
 ```shell-session
 $ turbocase project/project.kicad_pcb case.scad
 ```
 
+## Footprints
+
+TurboCase can automatically add prefab structures to the generated case by using the included KiCad library.
+The TurboCase.pretty folder in this repository is the footprint library that defines custom objects to add to the
+design of your case. The tool will detect any footprints that start with `TurboCase:` and append the correct module
+from `parts.py` into the final OpenSCAD file.
+
 ## Command line options
 
 ```
 usage: turbocase [-h] [--layer LAYER] [--bottom BOTTOM] [--wall WALL] pcb output
 
 positional arguments:
   pcb              Input kicad PCB file
```

### Comparing `turbocase-1.3/turbocase/__main__.py` & `turbocase-1.4/turbocase/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('pcb', help='Input kicad PCB file')
     parser.add_argument('output', help='Generated openSCAD case template')
     parser.add_argument('--layer', help='Layer with the case inner-outline [defaults to User.6]', default='User.6')
     parser.add_argument('--bottom', help='Bottom thickness in mm [default 1.2]', default=1.2, type=float)
     parser.add_argument('--wall', help='Wall thickness in mm [default 1.2]', default=1.2, type=float)
+    parser.add_argument('--standoff', help='Height generated for the PCB mounts in mm[default 5]', default=5, type=float)
     args = parser.parse_args()
 
     case = load_pcb(args.pcb, args.layer)
 
     case.floor_thickness = args.bottom
     case.wall_thickness = args.wall
+    case.standoff_height = args.standoff
 
     code = scad.generate(case)
     with open(args.output, 'w') as handle:
         handle.write(code)
 
 
 if __name__ == '__main__':
```

### Comparing `turbocase-1.3/turbocase/cases.py` & `turbocase-1.4/turbocase/cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,42 @@
 
     def depth(self):
         return self.prop_height
 
 
 class Part:
     def __init__(self):
-        self.script = None
         self.position = None
-        self.rotation = None
+        self.description = None
+
+        self.add = None
+        self.substract = None
+
+        self.offset_pcb = False
 
 
 class Case:
     connectors: list[Connector]
 
     def __init__(self):
         self.inner_path = []
         self.pcb_mount = []
         self.pcb_thickness = 1.6
         self.floor_thickness = 1.2
         self.wall_thickness = 1.2
+        self.standoff_height = 5
+
+        self.cutouts = []
 
         self.max_connector_height = 0
         self.connectors = []
 
         self.modules = []
         self.parts = []
+        self.max_part_height = 0
 
     def get_inner_bounds(self):
         min_x = self.inner_path[0][0]
         max_x = 0
         min_y = self.inner_path[0][1]
         max_y = 0
         for point in self.inner_path:
```

### Comparing `turbocase-1.3/turbocase/vector.py` & `turbocase-1.4/turbocase/vector.py`

 * *Files identical despite different names*

