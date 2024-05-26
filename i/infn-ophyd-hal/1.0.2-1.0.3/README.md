# Comparing `tmp/infn_ophyd_hal-1.0.2.tar.gz` & `tmp/infn_ophyd_hal-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infn_ophyd_hal-1.0.2.tar", last modified: Sun May 26 17:06:04 2024, max compression
+gzip compressed data, was "infn_ophyd_hal-1.0.3.tar", last modified: Sun May 26 17:17:39 2024, max compression
```

## Comparing `infn_ophyd_hal-1.0.2.tar` & `infn_ophyd_hal-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.627994 infn_ophyd_hal-1.0.2/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:06:04.627385 infn_ophyd_hal-1.0.2/PKG-INFO
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      505 2024-05-25 14:15:27.000000 infn_ophyd_hal-1.0.2/README.md
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.622637 infn_ophyd_hal-1.0.2/infn_ophyd_hal/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       42 2024-05-25 12:40:00.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/__init__.py
--rw-r--r--   0 andreamichelotti   (501) staff       (20)     3908 2024-05-25 09:15:24.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/opyhd_motor.py
--rw-r--r--   0 andreamichelotti   (501) staff       (20)    13142 2024-05-25 22:16:23.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal/tml_ophyd_motor.py
-drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:06:04.626855 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/PKG-INFO
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      298 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/SOURCES.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)        1 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/dependency_links.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       22 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/requires.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       15 2024-05-26 17:06:04.000000 infn_ophyd_hal-1.0.2/infn_ophyd_hal.egg-info/top_level.txt
--rw-r--r--   0 andreamichelotti   (501) staff       (20)       38 2024-05-26 17:06:04.628226 infn_ophyd_hal-1.0.2/setup.cfg
--rw-r--r--   0 andreamichelotti   (501) staff       (20)      659 2024-05-26 17:04:18.000000 infn_ophyd_hal-1.0.2/setup.py
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:17:39.822492 infn_ophyd_hal-1.0.3/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:17:39.822105 infn_ophyd_hal-1.0.3/PKG-INFO
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      505 2024-05-25 14:15:27.000000 infn_ophyd_hal-1.0.3/README.md
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:17:39.818871 infn_ophyd_hal-1.0.3/infn_ophyd_hal/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       42 2024-05-25 12:40:00.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal/__init__.py
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)     3908 2024-05-25 09:15:24.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal/opyhd_motor.py
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)    13142 2024-05-26 17:14:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal/tml_ophyd_motor.py
+drwxr-xr-x   0 andreamichelotti   (501) staff       (20)        0 2024-05-26 17:17:39.821590 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      387 2024-05-26 17:17:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/PKG-INFO
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      298 2024-05-26 17:17:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/SOURCES.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)        1 2024-05-26 17:17:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/dependency_links.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       22 2024-05-26 17:17:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/requires.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       15 2024-05-26 17:17:39.000000 infn_ophyd_hal-1.0.3/infn_ophyd_hal.egg-info/top_level.txt
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)       38 2024-05-26 17:17:39.822619 infn_ophyd_hal-1.0.3/setup.cfg
+-rw-r--r--   0 andreamichelotti   (501) staff       (20)      659 2024-05-26 17:17:20.000000 infn_ophyd_hal-1.0.3/setup.py
```

### Comparing `infn_ophyd_hal-1.0.2/infn_ophyd_hal/opyhd_motor.py` & `infn_ophyd_hal-1.0.3/infn_ophyd_hal/opyhd_motor.py`

 * *Files identical despite different names*

### Comparing `infn_ophyd_hal-1.0.2/infn_ophyd_hal/tml_ophyd_motor.py` & `infn_ophyd_hal-1.0.3/infn_ophyd_hal/tml_ophyd_motor.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,41 +141,41 @@
             status += "- lsp+lsn ERROR\n"
         status += "- dir " + str(self.dir()) + "\n"
         pos = self.user_readback.get()
         status += "- pos " + str(pos) + "\n"
         return status
 
     def iserror(self):
-        return (self.mot_msta_value & (1 << 0x9)) != 0
+        return (self.mot_msta.get() & (1 << 0x9)) != 0
 
     def ishomed(self):
-        return (self.mot_msta_value & (1 << 0xE)) != 0
+        return (self.mot_msta.get() & (1 << 0xE)) != 0
 
     def limit(self):
-        lsn = self.mot_msta_value & (1 << 0xD)
-        lsp = self.mot_msta_value & (1 << 2)
+        lsn = self.mot_msta.get() & (1 << 0xD)
+        lsp = self.mot_msta.get() & (1 << 2)
         if lsn:
             return -1
         if lsp:
             return 1
         if lsn and lsp:
             return -1000
         return 0
     
     def dir(self):
-        return self.mot_msta_value & 0x1
+        return self.mot_msta.get() & 0x1
     
     def moving(self):
         '''Whether or not the motor is moving
 
         Returns
         -------
         moving : bool
         '''
-        return (self.mot_msta_value & (1 << 0xA)) != 0
+        return (self.mot_msta.get() & (1 << 0xA)) != 0
     def home(self, direction, wait=True,timeout=120, **kwargs):
         if self.position() == 0 and self.ishomed():
             return Status()
         if self.homed.get():
             ## if already homed just move
             return self.move(0)
```

### Comparing `infn_ophyd_hal-1.0.2/setup.py` & `infn_ophyd_hal-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="infn_ophyd_hal",
-    version="1.0.2",
+    version="1.0.3",
     description="Ophyd HAL for controlling motors, cameras, magnets... specifically INFN facilities",
     author="Andrea Michelotti", 
     author_email="andrea.michelotti@infn.it", 
     # url="https://baltig.infn.it/infn-epics/infn_ophyd_hal", 
     packages=find_packages(),
     install_requires=[
         "ophyd",
```

