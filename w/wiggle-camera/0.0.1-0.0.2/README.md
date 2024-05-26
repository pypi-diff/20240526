# Comparing `tmp/wiggle_camera-0.0.1.tar.gz` & `tmp/wiggle_camera-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggle_camera-0.0.1.tar", last modified: Sat May 25 11:23:49 2024, max compression
+gzip compressed data, was "wiggle_camera-0.0.2.tar", last modified: Sun May 26 16:11:45 2024, max compression
```

## Comparing `wiggle_camera-0.0.1.tar` & `wiggle_camera-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 11:23:49.417382 wiggle_camera-0.0.1/
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1627 2024-05-25 11:23:49.417382 wiggle_camera-0.0.1/PKG-INFO
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1234 2024-05-25 10:37:57.000000 wiggle_camera-0.0.1/README.md
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)      627 2024-04-21 17:55:04.000000 wiggle_camera-0.0.1/pyproject.toml
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)       38 2024-05-25 11:23:49.417382 wiggle_camera-0.0.1/setup.cfg
-drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 11:23:49.409382 wiggle_camera-0.0.1/src/
-drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 11:23:49.413382 wiggle_camera-0.0.1/src/wiggle_camera/
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 10:41:40.000000 wiggle_camera-0.0.1/src/wiggle_camera/__init__.py
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1662 2024-05-18 19:27:27.000000 wiggle_camera-0.0.1/src/wiggle_camera/camera.py
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1111 2024-04-28 13:13:30.000000 wiggle_camera-0.0.1/src/wiggle_camera/install.py
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1011 2024-04-26 19:03:08.000000 wiggle_camera-0.0.1/src/wiggle_camera/main.py
-drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 11:23:49.417382 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1627 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/PKG-INFO
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)      385 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/SOURCES.txt
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)        1 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/dependency_links.txt
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)      112 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/entry_points.txt
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)        7 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/requires.txt
--rw-r--r--   0 wiggle    (1000) wiggle    (1000)       14 2024-05-25 11:23:49.000000 wiggle_camera-0.0.1/src/wiggle_camera.egg-info/top_level.txt
+drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     2174 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/PKG-INFO
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1730 2024-05-25 11:36:50.000000 wiggle_camera-0.0.2/README.md
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)      669 2024-05-26 16:10:10.000000 wiggle_camera-0.0.2/pyproject.toml
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)       38 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/setup.cfg
+drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/src/
+drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/src/wiggle_camera/
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)        0 2024-05-25 10:41:40.000000 wiggle_camera-0.0.2/src/wiggle_camera/__init__.py
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1662 2024-05-18 19:27:27.000000 wiggle_camera-0.0.2/src/wiggle_camera/camera.py
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1111 2024-04-28 13:13:30.000000 wiggle_camera-0.0.2/src/wiggle_camera/install.py
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)      586 2024-05-26 15:50:57.000000 wiggle_camera-0.0.2/src/wiggle_camera/light.py
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     1419 2024-05-26 15:55:46.000000 wiggle_camera-0.0.2/src/wiggle_camera/main.py
+drwxr-xr-x   0 wiggle    (1000) wiggle    (1000)        0 2024-05-26 16:11:45.372011 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)     2174 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/PKG-INFO
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)      412 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/SOURCES.txt
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)        1 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/dependency_links.txt
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)      112 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/entry_points.txt
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)       43 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/requires.txt
+-rw-r--r--   0 wiggle    (1000) wiggle    (1000)       14 2024-05-26 16:11:45.000000 wiggle_camera-0.0.2/src/wiggle_camera.egg-info/top_level.txt
```

### Comparing `wiggle_camera-0.0.1/PKG-INFO` & `wiggle_camera-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: wiggle_camera
-Version: 0.0.1
-Summary: WiggleCamera - Control the camera on your WiggleBin
-Author: Studio Rabota
-Project-URL: Homepage, https://github.com/wiggle-bin/wiggle-camera.git
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: pillow
-
 # WiggleCamera
 
 The [WiggleBIn](https://github.com/wiggle-bin/wiggle-bin) recording service for taking pictures.
 
 ## Prepare Raspberry PI
 
 Install picamera2 - https://github.com/raspberrypi/picamera2.
@@ -83,7 +71,33 @@
 pip3 install -e .
 ```
 
 For installation without dev dependencies
 ```
 pip install --no-dev -r requirements.txt
 ```
+
+## Publishing to PyPi
+
+To build your package, you'll need to install the `build` module. You can do this with pip:
+
+```bash
+pip install --upgrade build
+```
+
+Then, you can build your package with the following command:
+
+```bash
+python -m build
+```
+
+To publish your package to PyPI, you'll need to install the `twine` module:
+
+```bash
+pip install --upgrade twine
+```
+
+Then, you can use `twine` to upload your distributions to PyPI:
+
+```bash
+twine upload -u __token__ -p your_token_here dist/*
+```
```

### Comparing `wiggle_camera-0.0.1/pyproject.toml` & `wiggle_camera-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wiggle_camera"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Studio Rabota" },
 ]
 description = "WiggleCamera - Control the camera on your WiggleBin"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'pillow'
+  'pillow',
+  'adafruit-circuitpython-neopixel-spi',
 ]
 
 [project.scripts]
 wiggle-camera = "wiggle_camera.main:main"
 wiggle-camera-install = "wiggle_camera.install:install"
 
 [project.urls]
```

### Comparing `wiggle_camera-0.0.1/src/wiggle_camera/camera.py` & `wiggle_camera-0.0.2/src/wiggle_camera/camera.py`

 * *Files identical despite different names*

### Comparing `wiggle_camera-0.0.1/src/wiggle_camera/install.py` & `wiggle_camera-0.0.2/src/wiggle_camera/install.py`

 * *Files identical despite different names*

### Comparing `wiggle_camera-0.0.1/src/wiggle_camera/main.py` & `wiggle_camera-0.0.2/src/wiggle_camera/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import os
 import wiggle_camera.camera as camera
-
+from wiggle_camera.light import off, on, default_brightness
 
 def main():
     parser = argparse.ArgumentParser(
         prog="WiggleCamera", description="Control the camera on WiggleBin"
     )
 
     camera_group = parser.add_argument_group("camera")
@@ -19,20 +19,30 @@
         "--service",
         const="status",
         nargs="?",
         choices=["stop", "start"],
         help="control wiggler recording",
     )
 
+    light = parser.add_argument_group("light")
+    light.add_argument(
+        "--light", nargs="?", const=default_brightness, help="light intensity from 0.01 to 1", type=float
+    )
+    light.add_argument("--light-off", action="store_true", help="turn light off")
+
     args = parser.parse_args()
 
     if args.picture:
         camera.picture()
     elif args.recording:
         camera.recording()
     elif args.service:
         os.system(f"systemctl --user {args.service} wiggle-camera-record.service")
         print(f"WiggleCamera recording: {args.service}")
+    elif args.light:
+        on(args.light)
+    elif args.light_off:
+        off()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wiggle_camera-0.0.1/src/wiggle_camera.egg-info/PKG-INFO` & `wiggle_camera-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: wiggle_camera
-Version: 0.0.1
+Version: 0.0.2
 Summary: WiggleCamera - Control the camera on your WiggleBin
 Author: Studio Rabota
 Project-URL: Homepage, https://github.com/wiggle-bin/wiggle-camera.git
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pillow
+Requires-Dist: adafruit-circuitpython-neopixel-spi
 
 # WiggleCamera
 
 The [WiggleBIn](https://github.com/wiggle-bin/wiggle-bin) recording service for taking pictures.
 
 ## Prepare Raspberry PI
 
@@ -83,7 +84,33 @@
 pip3 install -e .
 ```
 
 For installation without dev dependencies
 ```
 pip install --no-dev -r requirements.txt
 ```
+
+## Publishing to PyPi
+
+To build your package, you'll need to install the `build` module. You can do this with pip:
+
+```bash
+pip install --upgrade build
+```
+
+Then, you can build your package with the following command:
+
+```bash
+python -m build
+```
+
+To publish your package to PyPI, you'll need to install the `twine` module:
+
+```bash
+pip install --upgrade twine
+```
+
+Then, you can use `twine` to upload your distributions to PyPI:
+
+```bash
+twine upload -u __token__ -p your_token_here dist/*
+```
```

