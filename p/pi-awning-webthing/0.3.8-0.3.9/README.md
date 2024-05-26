# Comparing `tmp/pi_awning_webthing-0.3.8.tar.gz` & `tmp/pi_awning_webthing-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pi_awning_webthing-0.3.8.tar", last modified: Sun May 26 13:02:56 2024, max compression
+gzip compressed data, was "dist/pi_awning_webthing-0.3.9.tar", last modified: Sun May 26 13:09:02 2024, max compression
```

## Comparing `pi_awning_webthing-0.3.8.tar` & `pi_awning_webthing-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/awning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/awning_webthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/motor_tb6612Fng.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/pi_awning_webthing/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:02:56.000000 pi_awning_webthing-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 13:02:42.000000 pi_awning_webthing-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/awning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/awning_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/motor_tb6612Fng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/pi_awning_webthing/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 13:09:01.000000 pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:09:02.000000 pi_awning_webthing-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 13:08:51.000000 pi_awning_webthing-0.3.9/setup.py
```

### Comparing `pi_awning_webthing-0.3.8/PKG-INFO` & `pi_awning_webthing-0.3.9/pi_awning_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pi_awning_webthing
-Version: 0.3.8
+Name: pi-awning-webthing
+Version: 0.3.9
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.8/README.md` & `pi_awning_webthing-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/__init__.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/app.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/app.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/awning.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/awning.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             logging.info("move to previous target position " + str(saved_target_pos))
             self.set_position(saved_target_pos)
 
     def __get_current_position(self) -> int:
         return self.movement.get_current_pos()
 
     def is_target_reached(self) -> bool:
-        return self.movement.is_target_reached()
+        return self.__get_current_position() == self.get_position()
 
     def get_position(self) -> int:
         return self.movement.get_target_pos()
 
     def set_position(self, new_position: int):
         with self.__lock:
             logging.info(self.name + " set position: " + str(new_position))
```

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/awning_webthing.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/awning_webthing.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/motor_tb6612Fng.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/motor_tb6612Fng.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing/switch.py` & `pi_awning_webthing-0.3.9/pi_awning_webthing/switch.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.8/pi_awning_webthing.egg-info/PKG-INFO` & `pi_awning_webthing-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pi-awning-webthing
-Version: 0.3.8
+Name: pi_awning_webthing
+Version: 0.3.9
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.8/setup.py` & `pi_awning_webthing-0.3.9/setup.py`

 * *Files identical despite different names*

