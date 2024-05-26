# Comparing `tmp/pyuptech-0.1.6.1.tar.gz` & `tmp/pyuptech-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.6.1.tar", last modified: Sat May 25 06:43:56 2024, max compression
+gzip compressed data, was "pyuptech-0.1.6.2.tar", last modified: Sun May 26 10:15:14 2024, max compression
```

## Comparing `pyuptech-0.1.6.1.tar` & `pyuptech-0.1.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     8813 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/README.md
--rw-r--r--   0        0        0      547 2024-05-25 06:43:56.277679 pyuptech-0.1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      190 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1976 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1007 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    12313 2024-05-25 06:43:33.297669 pyuptech-0.1.6.1/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    13599 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     7489 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/__init__.py
--rw-r--r--   0        0        0      737 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/perf_tests.py
--rw-r--r--   0        0        0      208 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/raw_test.py
--rw-r--r--   0        0        0     2480 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/test_sensor.py
--rw-r--r--   0        0        0      424 2024-05-25 06:43:33.301669 pyuptech-0.1.6.1/tests/utils.py
--rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 pyuptech-0.1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     8813 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/README.md
+-rw-r--r--   0        0        0      547 2024-05-26 10:15:14.712349 pyuptech-0.1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1976 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    12344 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13599 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     7489 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-26 10:14:54.700493 pyuptech-0.1.6.2/tests/perf_tests.py
+-rw-r--r--   0        0        0      208 2024-05-26 10:14:54.704493 pyuptech-0.1.6.2/tests/raw_test.py
+-rw-r--r--   0        0        0     2480 2024-05-26 10:14:54.704493 pyuptech-0.1.6.2/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-26 10:14:54.704493 pyuptech-0.1.6.2/tests/utils.py
+-rw-r--r--   0        0        0     9130 1970-01-01 00:00:00.000000 pyuptech-0.1.6.2/PKG-INFO
```

### Comparing `pyuptech-0.1.6.1/README.md` & `pyuptech-0.1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/pyproject.toml` & `pyuptech-0.1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.6.1"
+version = "0.1.6.2"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.6.1/src/pyuptech/__init__.py` & `pyuptech-0.1.6.2/src/pyuptech/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.6.2/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/emulation.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/loader.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/logger.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/pins.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/screen.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/screen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import Enum
+from enum import Enum, IntEnum
 from typing import Literal, Self
 
 from .constant import LIB_FILE_PATH
 from .loader import load_lib
 from .logger import _logger
 
 
@@ -24,15 +24,15 @@
     FONT_12X16 = 10
     FONT_12X20 = 11
     FONT_16X26 = 12
     FONT_22X36 = 13
     FONT_24X40 = 14
 
 
-class Color(Enum):
+class Color(IntEnum):
     """
     All supported color display on the led/lcd
     """
 
     @staticmethod
     def new_color(r: int, g: int, b: int) -> int:
         """
@@ -82,24 +82,25 @@
     BLUEGREEN = new_color(0, 128, 128)
 
     DARKBLUE = new_color(0, 0, 139)
     DARKGREEN = new_color(0, 139, 0)
     DARKRED = new_color(139, 0, 0)
 
 
+__lib__ = load_lib(LIB_FILE_PATH)
+
+
 class Screen:
     """
     Screen module
 
     This class represents an LCD screen and provides methods to manipulate it.
     Each method returns self to enable chainable calls.
     """
 
-    lib = load_lib(LIB_FILE_PATH)
-
     def __init__(self, screen_dir: Literal[1, 2] | int = None):
         """
         Initializes the Screen class.
 
         Parameters:
             screen_dir (Literal[1, 2], optional): The direction to open the screen in. Defaults to None.
 
@@ -118,150 +119,152 @@
           direction (Literal[1, 2]): Display direction; 1 for vertical, 2 for horizontal.
 
         Returns:
           Self for chainable calls.
         """
 
         _logger.info(f"Open LCD with direction: {direction}")
-        self.lib.lcd_open(direction)
+        __lib__.lcd_open(direction)
         return self
 
     def close(self) -> Self:
         """
         Close the LCD.
 
         Returns:
           Self for chainable calls.
         """
         _logger.info("Closing LCD")
-        self.lib.lcd_close()
+        __lib__.lcd_close()
         return self
 
     def refresh(self) -> Self:
         """
         Refresh the screen, printing the display data from the cache onto the screen.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.LCD_Refresh()
+        __lib__.LCD_Refresh()
         return self
 
     def set_font_size(self, font_size: FontSize) -> Self:
         """
         Set the font size.
 
         Args:
           font_size (FontSize): The desired font size.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.LCD_SetFont(font_size.value)
+        __lib__.LCD_SetFont(font_size.value)
         return self
 
-    def set_fore_color(self, color: Color) -> Self:
+    def set_fore_color(self, color: Color | int) -> Self:
         """
         Set the foreground color.
 
         Args:
           color (Color): The desired foreground color.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_SetForecolor(color)
+        __lib__.UG_SetForecolor(color)
         return self
 
-    def set_back_color(self, color: Color) -> Self:
+    def set_back_color(self, color: Color | int) -> Self:
         """
         Set the background color of the LCD.
 
         Args:
           color (Color): The desired background color.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_SetBackcolor(color)
+        __lib__.UG_SetBackcolor(color)
         return self
 
-    def set_led_color(self, index: Literal[0, 1] | int, color: Color) -> Self:
+    def set_led_color(self, index: Literal[0, 1] | int, color: Color | int) -> Self:
         """
         Set the LED color at a specific index.
 
         Parameters:
             index (Literal[0, 1]): The index of the LED to set the color for.
             color (Color): The color to set for the LED.
 
         Returns:
             Self: The instance of the class to allow for method chaining.
         """
-        self.lib.adc_led_set(index, color.value)
+        __lib__.adc_led_set(index, color)
         return self
 
-    def set_led_0(self, color: Color) -> Self:
-        self.lib.adc_led_set(0, color.value)
+    def set_led_0(self, color: Color | int) -> Self:
+        __lib__.adc_led_set(0, color)
         return self
 
-    def set_led_1(self, color: Color) -> Self:
-        self.lib.adc_led_set(1, color.value)
+    def set_led_1(self, color: Color | int) -> Self:
+        __lib__.adc_led_set(1, color)
         return self
 
     def set_led_hex(self, index: int, color: int) -> Self:
-        self.lib.adc_led_set(index, color)
+        __lib__.adc_led_set(index, color)
         return self
 
-    def fill_screen(self, color: Color) -> Self:
+    def fill_screen(self, color: Color | int) -> Self:
         """
         Fill the entire screen with the specified color.
 
         Args:
           color (Color): The color to fill the screen with.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_FillScreen(color.value)
+        __lib__.UG_FillScreen(color)
         return self
 
     def put_string(self, x: int, y: int, display_string: str) -> Self:
         """
         Place a string at specific coordinates on the LCD.
 
         Args:
           x (int): X coordinate (in pixels).
           y (int): Y coordinate (in pixels).
           display_string (str): The string to display on the LCD.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_PutString(x, y, display_string)
+        __lib__.UG_PutString(x, y, display_string)
         return self
 
-    def fill_frame(self, x1: int, y1: int, x2: int, y2: int, color: Color) -> Self:
+    def fill_frame(
+        self, x1: int, y1: int, x2: int, y2: int, color: Color | int
+    ) -> Self:
         """
         Fill a rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
           x2 (int): The X coordinate of the bottom-right corner.
           y2 (int): The Y coordinate of the bottom-right corner.
           color (Color): The color to fill the frame with.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_FillFrame(x1, y1, x2, y2, color.value)
+        __lib__.UG_FillFrame(x1, y1, x2, y2, color)
         return self
 
     def fill_round_frame(
-        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color
+        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
     ) -> Self:
         """
         Fill a rounded rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
@@ -269,69 +272,71 @@
           y2 (int): The Y coordinate of the bottom-right corner.
           r (int): The radius of the corners.
           color (Color): The color to fill the round frame with.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_FillRoundFrame(x1, y1, x2, y2, r, color.value)
+        __lib__.UG_FillRoundFrame(x1, y1, x2, y2, r, color)
         return self
 
-    def fill_circle(self, x0: int, y0: int, r: int, color: Color) -> Self:
+    def fill_circle(self, x0: int, y0: int, r: int, color: Color | int) -> Self:
         """
         Fill a circle with the specified color.
 
         Args:
           x0 (int): The X coordinate of the circle center.
           y0 (int): The Y coordinate of the circle center.
           r (int): The radius of the circle.
           color (Color): The color to fill the circle with.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_FillCircle(x0, y0, r, color.value)
+        __lib__.UG_FillCircle(x0, y0, r, color)
         return self
 
-    def draw_mesh(self, x1: int, y1: int, x2: int, y2: int, color: Color) -> Self:
+    def draw_mesh(self, x1: int, y1: int, x2: int, y2: int, color: Color | int) -> Self:
         """
         Draw a mesh pattern within a rectangle with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
           x2 (int): The X coordinate of the bottom-right corner.
           y2 (int): The Y coordinate of the bottom-right corner.
           color (Color): The color of the mesh lines.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawMesh(x1, y1, x2, y2, color.value)
+        __lib__.UG_DrawMesh(x1, y1, x2, y2, color)
         return self
 
-    def draw_frame(self, x1: int, y1: int, x2: int, y2: int, color: Color) -> Self:
+    def draw_frame(
+        self, x1: int, y1: int, x2: int, y2: int, color: Color | int
+    ) -> Self:
         """
         Draw an empty rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
           x2 (int): The X coordinate of the bottom-right corner.
           y2 (int): The Y coordinate of the bottom-right corner.
           color (Color): The color of the frame lines.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawFrame(x1, y1, x2, y2, color.value)
+        __lib__.UG_DrawFrame(x1, y1, x2, y2, color)
         return self
 
     def draw_round_frame(
-        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color
+        self, x1: int, y1: int, x2: int, y2: int, r: int, color: Color | int
     ) -> Self:
         """
         Draw an empty rounded rectangular frame with the specified color.
 
         Args:
           x1 (int): The X coordinate of the top-left corner.
           y1 (int): The Y coordinate of the top-left corner.
@@ -339,78 +344,78 @@
           y2 (int): The Y coordinate of the bottom-right corner.
           r (int): The radius of the corners.
           color (Color): The color of the frame lines.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawRoundFrame(x1, y1, x2, y2, r, color.value)
+        __lib__.UG_DrawRoundFrame(x1, y1, x2, y2, r, color)
         return self
 
-    def draw_pixel(self, x0: int, y0: int, color: Color) -> Self:
+    def draw_pixel(self, x0: int, y0: int, color: Color | int) -> Self:
         """
         Draw a single pixel at the specified coordinates with the specified color.
 
         Args:
           x0 (int): The X coordinate of the pixel.
           y0 (int): The Y coordinate of the pixel.
           color (Color): The color of the pixel.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawPixel(x0, y0, color.value)
+        __lib__.UG_DrawPixel(x0, y0, color)
         return self
 
-    def draw_circle(self, x0: int, y0: int, r: int, color: Color) -> Self:
+    def draw_circle(self, x0: int, y0: int, r: int, color: Color | int) -> Self:
         """
         Draw an empty circle with the specified color.
 
         Args:
           x0 (int): The X coordinate of the circle center.
           y0 (int): The Y coordinate of the circle center.
           r (int): The radius of the circle.
           color (Color): The color of the circle lines.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawCircle(x0, y0, r, color.value)
+        __lib__.UG_DrawCircle(x0, y0, r, color)
         return self
 
-    def draw_arc(self, x0: int, y0: int, r: int, s: int, color: Color) -> Self:
+    def draw_arc(self, x0: int, y0: int, r: int, s: int, color: Color | int) -> Self:
         """
         Draw an arc with the specified color.
 
         Args:
           x0 (int): The X coordinate of the circle center.
           y0 (int): The Y coordinate of the circle center.
           r (int): The radius of the arc circle.
           s (int): The starting angle of the arc.
           color (Color): The color of the arc lines.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawArc(x0, y0, r, s, color.value)
+        __lib__.UG_DrawArc(x0, y0, r, s, color)
         return self
 
-    def draw_line(self, x1: int, y1: int, x2: int, y2: int, color: Color) -> Self:
+    def draw_line(self, x1: int, y1: int, x2: int, y2: int, color: Color | int) -> Self:
         """
         Draw a line between two points with the specified color.
 
         Args:
           x1 (int): The X coordinate of the first point.
           y1 (int): The Y coordinate of the first point.
           x2 (int): The X coordinate of the second point.
           y2 (int): The Y coordinate of the second point.
           color (Color): The color of the line.
 
         Returns:
           Self for chainable calls.
         """
-        self.lib.UG_DrawLine(x1, y1, x2, y2, color.value)
+        __lib__.UG_DrawLine(x1, y1, x2, y2, color)
         return self
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyuptech-0.1.6.1/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.6.2/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/src/pyuptech/tools/display.py` & `pyuptech-0.1.6.2/src/pyuptech/tools/display.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/tests/display_tests.py` & `pyuptech-0.1.6.2/tests/display_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,10 +19,16 @@
 
     def test_led(self):
         for c in Color:
             self.scr.set_led_color(0, c)
             print(f"\rnow is {c}", end="")
             sleep(1)
 
+    def test_color(self):
+        from pyuptech import Color
+
+        c = Color.new_color(255, 0, 0)
+        print(c)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyuptech-0.1.6.1/tests/perf_tests.py` & `pyuptech-0.1.6.2/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/tests/test_sensor.py` & `pyuptech-0.1.6.2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.6.1/PKG-INFO` & `pyuptech-0.1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
```

