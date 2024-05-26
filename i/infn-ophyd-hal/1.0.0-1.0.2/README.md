# Comparing `tmp/infn_ophyd_hal-1.0.0.tar.gz` & `tmp/infn_ophyd_hal-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infn_ophyd_hal-1.0.0.tar", last modified: Sat May 25 14:15:12 2024, max compression
+gzip compressed data, was "infn_ophyd_hal-1.0.2.tar", last modified: Sun May 26 17:06:04 2024, max compression
```

## Comparing `infn_ophyd_hal-1.0.0.tar` & `infn_ophyd_hal-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-25 14:15:12.381243 infn_ophyd_hal-1.0.0/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-25 14:15:12.380673 infn_ophyd_hal-1.0.0/PKG-INFO
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      505 2024-05-25 14:14:47.000000 infn_ophyd_hal-1.0.0/README.md
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-25 14:15:12.375594 infn_ophyd_hal-1.0.0/infn_ophyd_hal/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       42 2024-05-25 12:40:00.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal/__init__.py
--rw-r--r--   0 andreamichelotti   (501) staff       (20)     3908 2024-05-25 09:15:24.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal/opyhd_motor.py
--rw-r--r--   0 andreamichelotti   (501) staff       (20)    13136 2024-05-25 14:05:10.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal/tml_ophyd_motor.py
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-25 14:15:12.379846 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-25 14:15:12.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/PKG-INFO
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      298 2024-05-25 14:15:12.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/SOURCES.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)        1 2024-05-25 14:15:12.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/dependency_links.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       22 2024-05-25 14:15:12.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/requires.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       15 2024-05-25 14:15:12.000000 infn_ophyd_hal-1.0.0/infn_ophyd_hal.egg-info/top_level.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       38 2024-05-25 14:15:12.381457 infn_ophyd_hal-1.0.0/setup.cfg
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      659 2024-05-25 13:43:41.000000 infn_ophyd_hal-1.0.0/setup.py
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.627994 infn_ophyd_hal-1.0.2/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:06:04.627385 infn_ophyd_hal-1.0.2/PKG-INFO
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      505 2024-05-25 14:15:27.000000 infn_ophyd_hal-1.0.2/README.md
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.622637 infn_ophyd_hal-1.0.2/infn_ophyd_hal/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       42 2024-05-25 12:40:00.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/__init__.py
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)     3908 2024-05-25 09:15:24.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/opyhd_motor.py
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)    13142 2024-05-25 22:16:23.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/tml_ophyd_motor.py
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.626855 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/PKG-INFO
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      298 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/SOURCES.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)        1 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/dependency_links.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       22 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/requires.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       15 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/top_level.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       38 2024-05-26 17:06:04.628226 infn_ophyd_hal-1.0.2/setup.cfg
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      659 2024-05-26 17:04:18.000000 infn_ophyd_hal-1.0.2/setup.py
```

### Comparing `infn_ophyd_hal-1.0.0/infn_ophyd_hal/opyhd_motor.py` & `infn_ophyd_hal-1.0.2/infn_ophyd_hal/opyhd_motor.py`

 * *Files identical despite different names*

### Comparing `infn_ophyd_hal-1.0.0/infn_ophyd_hal/tml_ophyd_motor.py` & `infn_ophyd_hal-1.0.2/infn_ophyd_hal/tml_ophyd_motor.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 RUN = 1
 STOP = 2
 POS_TOLERANCE = 10
 
 class OphydTmlMotor(Device, PositionerBase):
     
     mot_msta = Cpt(EpicsSignalRO, ":MSTA")
-    mot_stat = Cpt(EpicsSignal, ":STAT")
+    mot_stat = Cpt(EpicsSignalRO, ":STAT")
     user_readback = Cpt(EpicsSignalRO, ":RBV")
     mot_msgs = Cpt(EpicsSignal, ":MSGS")
     mot_act_sp = Cpt(EpicsSignal, ":ACT")
     mot_act_rb = Cpt(EpicsSignal, ":ACT_RB")
     mot_actx_sp = Cpt(EpicsSignal, ":ACTX_SP")
     user_setpoint = Cpt(EpicsSignal, ":VAL_SP")
     mot_val_rb = Cpt(EpicsSignal, ":VAL_RB")
@@ -56,15 +56,15 @@
             read_attrs = ['user_readback', 'user_setpoint']
             
         super().__init__(prefix, read_attrs=read_attrs,
                          configuration_attrs=configuration_attrs,
                          name=name, parent=parent, **kwargs)
         self.poi = poi
         self.user_readback.name = self.name
-        self.mot_stat.subscribe(self._on_mot_stat_change)
+        # self.mot_stat.subscribe(self._on_mot_stat_change)
         self.user_readback.subscribe(self._on_user_readback_change)
         self.mot_msta.subscribe(self._on_mot_msta_change)
 
         # Initial connection check
         self.mot_stat_value = self.mot_stat.get()
         self.mot_msta_value = self.mot_msta.get()
         #logging.debug(f"{name} State:\n{self.decode()}")
@@ -80,15 +80,15 @@
 
         
         super().unstage()
         
     def __del__(self):
         '''Destructor to handle any necessary cleanup.'''
         logger.debug(f"Cleaning up {self.name}")
-        self.mot_stat.unsubscribe(self._on_mot_stat_change)
+        # self.mot_stat.unsubscribe(self._on_mot_stat_change)
         self.user_readback.unsubscribe(self._on_user_readback_change)
         self.mot_msta.unsubscribe(self._on_mot_msta_change)
         
         self.unstage()
         # Add any other necessary cleanup here
               
     def enable(self,restart=False):
```

### Comparing `infn_ophyd_hal-1.0.0/setup.py` & `infn_ophyd_hal-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="infn_ophyd_hal",
-    version="1.0.0",
+    version="1.0.2",
     description="Ophyd HAL for controlling motors, cameras, magnets... specifically INFN facilities",
     author="Andrea Michelotti", 
     author_email="andrea.michelotti@infn.it", 
     # url="https://baltig.infn.it/infn-epics/infn_ophyd_hal", 
     packages=find_packages(),
     install_requires=[
         "ophyd",
```

