# Comparing `tmp/sh1106_framework-0.0.8.tar.gz` & `tmp/sh1106_framework-0.0.9.tar.gz`

## Comparing `sh1106_framework-0.0.8.tar` & `sh1106_framework-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/setup.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_font_generator.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_framework.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/sh1106_image_generator.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/constants.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state_manager.py
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/drawing.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/fonts.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/src/sh1106_framework/graphics/images.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/ping-pong.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/ping.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/tests/ping-pong/pong.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/default-font.json
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/default-font.png
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/example-images.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/useful-assets/example-images.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/LICENSE
--rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9542 2020-02-02 00:00:00.000000 sh1106_framework-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/setup.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/sh1106_font_generator.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/sh1106_framework.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/sh1106_image_generator.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/framework/constants.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/framework/states/state.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/framework/states/state_manager.py
+-rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/graphics/drawing.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/graphics/fonts.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/src/sh1106_framework/graphics/images.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/tests/ping-pong/ping-pong.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/tests/ping-pong/ping.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/tests/ping-pong/pong.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/useful-assets/default-font.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/useful-assets/default-font.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/useful-assets/example-images.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/useful-assets/example-images.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 sh1106_framework-0.0.9/PKG-INFO
```

### Comparing `sh1106_framework-0.0.8/setup.py` & `sh1106_framework-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sh1106_framework',
-    version='0.0.8',
+    version='0.0.9',
     author='Dan Convey',
     description='A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_font_generator.py` & `sh1106_framework-0.0.9/src/sh1106_framework/sh1106_font_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_framework.py` & `sh1106_framework-0.0.9/src/sh1106_framework/sh1106_framework.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/sh1106_image_generator.py` & `sh1106_framework-0.0.9/src/sh1106_framework/sh1106_image_generator.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state.py` & `sh1106_framework-0.0.9/src/sh1106_framework/framework/states/state.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/framework/states/state_manager.py` & `sh1106_framework-0.0.9/src/sh1106_framework/framework/states/state_manager.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/src/sh1106_framework/graphics/drawing.py` & `sh1106_framework-0.0.9/src/sh1106_framework/graphics/drawing.py`

 * *Files 3% similar despite different names*

```diff
@@ -313,15 +313,33 @@
             The scale of the image.
         centered_horizontal: bool
             Whether or not the image should be centered horizontally.
         centered_vertical: bool
             Whether or not the image should be centered vertically.
         """
         
-        Images._draw_image(image, x, y, color, scale, centered_horizontal, centered_vertical)
+        image_pixels = Images._images[image]
+        
+        if centered_horizontal:
+            offset_x = int((-image_pixels[0][0]*scale) / 2)
+        else:
+            offset_x = 0
+            
+        if centered_vertical:
+            offset_y = int((-image_pixels[0][1]*scale) / 2)
+        else:
+            offset_y = 0
+        
+        for y1 in range(image_pixels[0][1]):
+            for x1 in range(image_pixels[0][0]):
+                if image_pixels[y1+1][x1] == 1:
+                    if scale == 1:
+                        Drawing.set_pixel(x+x1+offset_x, y+y1+offset_y, color)
+                    else:
+                        Drawing.draw_rect(int(x+x1*scale+offset_x), int(y+y1*scale+offset_y), scale, scale, color)
     
     @staticmethod
     def _render() -> None:
         width = len(Drawing.__lcdpixels[0])
         height = len(Drawing.__lcdpixels)
         
         # Convert the 2D list into a bytes object with bit packing
```

### Comparing `sh1106_framework-0.0.8/tests/ping-pong/ping-pong.py` & `sh1106_framework-0.0.9/tests/ping-pong/ping-pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/tests/ping-pong/ping.py` & `sh1106_framework-0.0.9/tests/ping-pong/ping.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/tests/ping-pong/pong.py` & `sh1106_framework-0.0.9/tests/ping-pong/pong.py`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/useful-assets/default-font.json` & `sh1106_framework-0.0.9/useful-assets/default-font.json`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/useful-assets/default-font.png` & `sh1106_framework-0.0.9/useful-assets/default-font.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/useful-assets/example-images.png` & `sh1106_framework-0.0.9/useful-assets/example-images.png`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/LICENSE` & `sh1106_framework-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/README.md` & `sh1106_framework-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.8/pyproject.toml` & `sh1106_framework-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,37 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src/sh1106_framework"]
 include = [
   "README.md",
   "LICENSE",
   "src/sh1106_framework/**/*.py",
   "tests/**/*.py",
-  "useful-assets/*"
+  "useful-assets/*",
 ]
 
 [project]
 name = "sh1106_framework"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
-  { name="Dan Convey", email="author@example.com" },
+  { name="Dan Convey" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
 requires-python = ">=3.10"  
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
-    "Operating System :: Other OS"
+    "Operating System :: Other OS",
+]
+dependencies = [
+  "luma.oled",
+  "pillow",
 ]
 
 [project.urls]
 Homepage = "https://github.com/danspage/sh1106-framework"
 Issues = "https://github.com/danspage/sh1106-framework/issues"
 
 [project.scripts]
```

### Comparing `sh1106_framework-0.0.8/PKG-INFO` & `sh1106_framework-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.3
 Name: sh1106_framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
-Author-email: Dan Convey <author@example.com>
+Author: Dan Convey
 License: Apache License 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Other OS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: luma-oled
+Requires-Dist: pillow
 Description-Content-Type: text/markdown
 
 
 # SH1106 OLED Screen Framework Package
 
 A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
```

