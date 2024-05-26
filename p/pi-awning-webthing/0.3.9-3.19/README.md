# Comparing `tmp/pi_awning_webthing-0.3.9.tar.gz` & `tmp/pi_awning_webthing-3.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pi_awning_webthing-0.3.9.tar", last modified: Sun May 26 13:09:02 2024, max compression
+gzip compressed data, was "dist/pi_awning_webthing-3.19.tar", last modified: Sun May 26 14:15:47 2024, max compression
```

## Comparing `pi_awning_webthing-0.3.9.tar` & `pi_awning_webthing-3.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/awning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/awning_webthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/motor_tb6612Fng.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/awning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/awning_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/motor_tb6612Fng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/pi_awning_webthing/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/pi_awning_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:15:47.000000 pi_awning_webthing-3.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 14:15:37.000000 pi_awning_webthing-3.19/setup.py
```

### Comparing `pi_awning_webthing-0.3.9/PKG-INFO` & `pi_awning_webthing-3.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi_awning_webthing
-Version: 0.3.9
+Version: 3.19
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.9/README.md` & `pi_awning_webthing-3.19/README.md`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/__init__.py` & `pi_awning_webthing-3.19/pi_awning_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/app.py` & `pi_awning_webthing-3.19/pi_awning_webthing/app.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/awning.py` & `pi_awning_webthing-3.19/pi_awning_webthing/awning.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,22 @@
     def get_position(self) -> int:
         pass
 
     @abstractmethod
     def set_position(self, new_position: int):
         pass
 
+    @abstractmethod
+    def is_moving(self) -> bool:
+        pass
+
+    @abstractmethod
+    def stop(self):
+        pass
+
     def add_listener(self, listener):
         self.__listeners.add(listener)
 
     def _notify_listeners(self):
         for listener in self.__listeners:
             listener()
 
@@ -74,14 +82,17 @@
             self.direction = 1
         else:
             self.direction = -1
 
     def get_pause_sec(self):
         return 0.5
 
+    def is_moving(self) -> bool:
+        return False
+
     def get_current_pos(self) -> int:
         if self.is_target_reached():
             return self.get_target_pos()
         else:
             return self.start_pos + (self.__get_num_processed_slots() * self.direction)
 
     def get_target_pos(self) -> int:
@@ -124,14 +135,17 @@
 class Idling(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, 0, sec_per_slot, True, awning)
         self.motor.stop()
         self.awning.on_updated()
 
+    def is_moving(self) -> bool:
+        return False
+
     def get_pause_sec(self):
         pause_sec = int(self.SLOT_TOLERANCE * self.sec_per_slot * 1.4)
         if pause_sec < 3:
             pause_sec = 3
         return pause_sec
 
     def process(self):
@@ -141,22 +155,29 @@
 class Forward(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, new_position: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, new_position - start_pos, sec_per_slot, True, awning)
         self.motor.forward()
         self.awning.on_updated()
 
+    def is_moving(self) -> bool:
+        return True
+
 
 class Backward(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, new_position: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, start_pos - new_position, sec_per_slot, False, awning)
         self.motor.backward()
         self.awning.on_updated()
 
+    def is_moving(self) -> bool:
+        return True
+
+
 
 class PiAwning(Awning):
     PERIODIC_CALIBRATE_ON_HOUR = 3
     PERIODIC_CALIBRATE_ON_MINUTE = 10
 
     def __init__(self, motor: Motor):
         self.motor = motor
@@ -195,23 +216,29 @@
         self.set_position(0)   # and backward to position 0. This ensures that the awning is calibrated with position 0
         # wait until completed
         for i in range (0, 60):
             if self.is_target_reached():
                 break
             else:
                 time.sleep(5)
-        if self.__get_current_position() != saved_target_pos:
+        if self.get_current_position() != saved_target_pos:
             logging.info("move to previous target position " + str(saved_target_pos))
             self.set_position(saved_target_pos)
 
-    def __get_current_position(self) -> int:
+    def stop(self):
+        self.set_position(self.get_current_position())
+
+    def get_current_position(self) -> int:
         return self.movement.get_current_pos()
 
     def is_target_reached(self) -> bool:
-        return self.__get_current_position() == self.get_position()
+        return self.get_current_position() == self.get_position()
+
+    def is_moving(self) -> bool:
+        return self.movement.is_moving()
 
     def get_position(self) -> int:
         return self.movement.get_target_pos()
 
     def set_position(self, new_position: int):
         with self.__lock:
             logging.info(self.name + " set position: " + str(new_position))
@@ -240,14 +267,24 @@
 
     def is_target_reached(self) -> bool:
         for awning in self.__awnings:
             if not awning.is_target_reached():
                 return False
         return True
 
+    def is_moving(self) -> bool:
+        for anwing in self.__awnings:
+            if anwing.is_moving():
+                return True
+        return False
+
+    def stop(self):
+        for anwing in self.__awnings:
+            anwing.stop()
+
     def get_position(self) -> int:
         positions = [awning.get_position() for awning in self.__awnings]
         total = sum(positions)
         if total == 0:
             return 0
         else:
             return int(total/len(positions))
```

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/awning_webthing.py` & `pi_awning_webthing-3.19/pi_awning_webthing/awning_webthing.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,21 +74,21 @@
 
 
 
 def run_server(port: int, filename: str, switch_pin_forward: int, switch_pin_backward: int, description: str):
 
     while True:
         awnings = [PiAwning(motor) for motor in load_tb6612fng(filename)]
-        if len(awnings) > 2:
-            awnings = [Awnings("all", awnings)] + awnings
+        anwing_all= Awnings("all", awnings)
+        awnings = [anwing_all] + awnings
         awning_webthings = [AwningWebThing(description, anwing) for anwing in awnings]
         server = WebThingServer(MultipleThings(awning_webthings, 'Awnings'), port=port, disable_host_validation=True)
 
         if switch_pin_forward > 0 and switch_pin_backward > 0:
-            Switch(switch_pin_forward, switch_pin_backward, awnings= awnings)
+            Switch(switch_pin_forward, switch_pin_backward, awnings=anwing_all)
 
         try:
             logging.info('starting the server')
             server.start()
         except KeyboardInterrupt:
             logging.info('stopping the server')
             server.stop()
```

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/motor_tb6612Fng.py` & `pi_awning_webthing-3.19/pi_awning_webthing/motor_tb6612Fng.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing/switch.py` & `pi_awning_webthing-3.19/pi_awning_webthing/switch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 import logging
 import RPi.GPIO as GPIO
 from datetime import datetime, timedelta
 from typing import List
-from pi_awning_webthing.awning import Awning
+from pi_awning_webthing.awning import Awnings
 
 
 class Switch:
     STOP = (False, False)
     MOVE_FORWARD = (True, False)
     MOVE_BACKWARD = (False, True)
     IDLE = (True, True)
 
-    def __init__(self, pin_forward: int, pin_backward: int, awnings: List[Awning]):
+    def __init__(self, pin_forward: int, pin_backward: int, awnings: Awnings):
         self.awnings = awnings
         self.pin_forward = pin_forward
         self.pin_backward = pin_backward
-        self.state = self.STOP
+        self.last_time_pressed = datetime.now()
         GPIO.setmode(GPIO.BCM)
         GPIO.setup(self.pin_forward, GPIO.IN, GPIO.PUD_DOWN)
         GPIO.add_event_detect(self.pin_forward, GPIO.BOTH)
         GPIO.add_event_callback(self.pin_forward, self.on_switch_updated)
         GPIO.setup(self.pin_backward, GPIO.IN, GPIO.PUD_DOWN)
         GPIO.add_event_detect(self.pin_backward, GPIO.BOTH)
         GPIO.add_event_callback(self.pin_backward, self.on_switch_updated)
         logging.info("Switch bound to pin_forward=" + str(self.pin_forward) + " and pin_backward=" + str(self.pin_backward))
 
-    def is_forward(self) -> bool:
-        return self.state[0]
-
-    def is_backward(self) -> bool:
-        return self.state[1]
-
-    def is_target_reached(self) -> bool:
-        for anwing in self.awnings:
-            if not anwing.is_target_reached():
-                return False
-        return True
-
     def on_switch_updated(self, pin: int):
         is_forward = GPIO.input(self.pin_forward) >= 1
         is_backward = GPIO.input(self.pin_backward) >= 1
-
         new_state = (is_forward, is_backward)
-        try:
-            if new_state == self.MOVE_FORWARD:
-                if self.is_target_reached():
-                    for anwing in self.awnings:
-                        anwing.set_position(100)
-                else:
-                    for anwing in self.awnings:
-                        current_pos = anwing.get_position()
-                        anwing.set_position(current_pos)
+        logging.info("\n\n\nnew state Forward=" + str(new_state[0]) + "; Backward=" + str(new_state[1]) + " is_moving=" + str(self.awnings.is_moving()))
 
-            elif new_state == self.MOVE_BACKWARD:
-                if self.is_target_reached():
-                    for anwing in self.awnings:
-                        anwing.set_position(0)
-                else:
-                    for anwing in self.awnings:
-                        current_pos = anwing.get_position()
-                        anwing.set_position(current_pos)
-        except Exception as e:
-            logging.error(e)
-        finally:
-            self.state = new_state
+        if datetime.now() > (self.last_time_pressed + timedelta(seconds=0.5)):
+            self.last_time_pressed = datetime.now()
+            try:
+                if new_state == self.MOVE_FORWARD:
+                    if self.awnings.is_moving():
+                        logging.info("Forward and motion. stop")
+                        self.awnings.stop()
+                    else:
+                        logging.info("Forward set pos 0")
+                        self.awnings.set_position(100)
+                elif new_state == self.MOVE_BACKWARD:
+                    if self.awnings.is_moving():
+                        logging.info("Bckward and motion. stop")
+                        self.awnings.stop()
+                    else:
+                        logging.info("Bckward set pos 0")
+                        self.awnings.set_position(0)
+            except Exception as e:
+                logging.error(e)
+        else:
+            logging.info("double click")
```

### Comparing `pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/PKG-INFO` & `pi_awning_webthing-3.19/pi_awning_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-awning-webthing
-Version: 0.3.9
+Version: 3.19
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.9/setup.py` & `pi_awning_webthing-3.19/setup.py`

 * *Files identical despite different names*

