# Comparing `tmp/pi_awning_webthing-0.3.7.tar.gz` & `tmp/pi_awning_webthing-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pi_awning_webthing-0.3.7.tar", last modified: Sun May 26 12:51:43 2024, max compression
+gzip compressed data, was "dist/pi_awning_webthing-0.3.8.tar", last modified: Sun May 26 13:02:56 2024, max compression
```

## Comparing `pi_awning_webthing-0.3.7.tar` & `pi_awning_webthing-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/awning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/awning_webthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/motor_tb6612Fng.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/pi_awning_webthing/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 12:51:43.000000 pi_awning_webthing-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 12:51:32.000000 pi_awning_webthing-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/awning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/awning_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/motor_tb6612Fng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/setup.py
```

### Comparing `pi_awning_webthing-0.3.7/PKG-INFO` & `pi_awning_webthing-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi_awning_webthing
-Version: 0.3.7
+Version: 0.3.8
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.7/README.md` & `pi_awning_webthing-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/__init__.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/app.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/app.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/awning.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/awning.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/awning_webthing.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/awning_webthing.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/motor_tb6612Fng.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/motor_tb6612Fng.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing/switch.py` & `pi_awning_webthing-0.3.8/pi_awning_webthing/switch.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,39 +27,40 @@
 
     def is_forward(self) -> bool:
         return self.state[0]
 
     def is_backward(self) -> bool:
         return self.state[1]
 
+    def is_target_reached(self) -> bool:
+        for anwing in self.awnings:
+            if not anwing.is_target_reached():
+                return False
+        return True
+
     def on_switch_updated(self, pin: int):
         is_forward = GPIO.input(self.pin_forward) >= 1
         is_backward = GPIO.input(self.pin_backward) >= 1
 
         new_state = (is_forward, is_backward)
         try:
             if new_state == self.MOVE_FORWARD:
-                # repeated
-                if self.state == self.MOVE_FORWARD:
-                    for anwing in self.awnings:
-                        current_pos = anwing.get_position()
-                        anwing.set_position(current_pos)
-                # fresh
-                else:
-                    self.last_time_direction_changed = datetime.now()
+                if self.is_target_reached():
                     for anwing in self.awnings:
                         anwing.set_position(100)
-            elif new_state == self.MOVE_BACKWARD:
-                # repeated
-                if self.state == self.MOVE_BACKWARD:
+                else:
                     for anwing in self.awnings:
                         current_pos = anwing.get_position()
                         anwing.set_position(current_pos)
-                # fresh
-                else:
+
+            elif new_state == self.MOVE_BACKWARD:
+                if self.is_target_reached():
                     for anwing in self.awnings:
                         anwing.set_position(0)
-
+                else:
+                    for anwing in self.awnings:
+                        current_pos = anwing.get_position()
+                        anwing.set_position(current_pos)
         except Exception as e:
             logging.error(e)
         finally:
             self.state = new_state
```

### Comparing `pi_awning_webthing-0.3.7/pi_awning_webthing.egg-info/PKG-INFO` & `pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-awning-webthing
-Version: 0.3.7
+Version: 0.3.8
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.7/setup.py` & `pi_awning_webthing-0.3.8/setup.py`

 * *Files identical despite different names*

