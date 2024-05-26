# Comparing `tmp/cbpi4-BM_PID_SmartBoilWithPump-0.1.6.tar.gz` & `tmp/cbpi4-BM_PID_SmartBoilWithPump-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-BM_PID_SmartBoilWithPump-0.1.6.tar", last modified: Sat Aug 20 16:18:31 2022, max compression
+gzip compressed data, was "cbpi4-BM_PID_SmartBoilWithPump-0.1.7.tar", last modified: Sun May 26 06:15:56 2024, max compression
```

## Comparing `cbpi4-BM_PID_SmartBoilWithPump-0.1.6.tar` & `cbpi4-BM_PID_SmartBoilWithPump-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-20 16:18:31.307985 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/
--rw-r--r--   0 root         (0) root         (0)      108 2021-11-29 14:39:00.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3677 2022-08-20 16:18:31.307985 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2910 2022-08-20 16:18:10.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-20 16:18:31.307985 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4-BM_PID_SmartBoilWithPump/
--rw-r--r--   0 root         (0) root         (0)    11717 2022-08-20 16:18:10.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4-BM_PID_SmartBoilWithPump/__init__.py
--rw-r--r--   0 root         (0) root         (0)       47 2021-11-29 14:39:00.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4-BM_PID_SmartBoilWithPump/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-20 16:18:31.307985 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3677 2022-08-20 16:18:30.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2022-08-20 16:18:30.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-20 16:18:30.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-08-20 16:18:30.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-20 16:18:31.307985 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      950 2022-08-20 16:18:10.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:15:56.021628 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/
+-rw-rw-rw-   0        0        0    35129 2021-11-29 14:39:00.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      108 2021-11-29 14:39:00.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3569 2024-05-26 06:15:56.019629 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3193 2024-05-26 06:14:20.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 06:15:55.949627 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4-BM_PID_SmartBoilWithPump/
+-rw-rw-rw-   0        0        0    12781 2024-05-24 15:04:23.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4-BM_PID_SmartBoilWithPump/__init__.py
+-rw-rw-rw-   0        0        0       47 2021-11-29 14:39:00.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4-BM_PID_SmartBoilWithPump/config.yaml
+drwxrwxrwx   0        0        0        0 2024-05-26 06:15:56.016624 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/
+-rw-rw-rw-   0        0        0     3569 2024-05-26 06:15:55.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-26 06:15:55.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 06:15:55.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-26 06:15:55.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 06:15:56.022624 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      974 2024-05-26 06:15:28.000000 cbpi4-BM_PID_SmartBoilWithPump-0.1.7/setup.py
```

### Comparing `cbpi4-BM_PID_SmartBoilWithPump-0.1.6/PKG-INFO` & `cbpi4-BM_PID_SmartBoilWithPump-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-Metadata-Version: 2.1
-Name: cbpi4-BM_PID_SmartBoilWithPump
-Version: 0.1.6
-Summary: CraftBeerPi4 PID Kettle Logic Plugin
-Home-page: https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump
-Author: ['Alexander Vollkopf', 'Guy Lev']
-Author-email: avollkopf@web.de
-License: GPLv3
-Description: # CBPi4 Braumeister Smart Boil with Pump KettleLogic
-        
-        ### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
-        
-        ## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
-        - The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
-        - It runs on PID control until it reaches a specified temperature. Above that temperature it heates w/o PID logic until a specified boil temp is reached.
-        - Power to run boil can be specified in the plugin
-        - Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
-        
-        
-        ### Installation:
-        
-        You can install it directly via pypi.org:	
-        - sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
-        
-        Alternativeley you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
-        - sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
-        
-        
-        ## Parameters:
-        
-        ![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
-        
-        - Configurable:
-        	- P: Proportional - Takes current value into account
-        	- I: Integral - Takes past values into account
-        	- D: Derivative - Takes future values into account
-        	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
-        	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
-        	- Max Boil Output: Maximum Power during when Boil Temp is reached
-        	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
-        	- Max PID Temp: PID is switched off above this temperature
-        	- Rest Interval: Time interval in seconds after which Pump is switched off
-        	- Rest Time: Pump is switched off for specified time in seconds
-        	
-        - Fixed in Code:
-        	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
-        
-        
-        Changelog:
-        
-        - 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
-        - 11.05.22: (0.1.5) Updated README (removed cbpi add)
-        - 10.05.22: (0.1.4) removed cbpi dependency
-        - 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be sitched on at start and off if temp is above controll limit. But no pump pause is triggered
-        - 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
-        - 21.11.21: Updated setup and Readme 
-        - 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
-        - 01.11.21: Merged Pull request from madhatguy ansd fixed some bugs
-        - 15.03.21: Support for cbpi >= 4.0.0.32
-        - 31.10.21: Changed logic to coroutines
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: cbpi4-BM_PID_SmartBoilWithPump
+Version: 0.1.7
+Summary: CraftBeerPi4 PID Kettle Logic Plugin
+Home-page: https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump
+Author: ['Alexander Vollkopf', 'Guy Lev']
+Author-email: avollkopf@web.de
+License: GPLv3
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CBPi4 Braumeister Smart Boil with Pump KettleLogic
+
+### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
+
+## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
+- The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
+- It runs on PID control until it reaches a specified temperature. Above that temperature it heats w/o PID logic until a specified boil temp is reached.
+- Power to run boil can be specified in the plugin
+- Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
+
+
+### Installation:
+
+You can install it directly via pypi.org:	
+- sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
+
+Alternatively you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
+- sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
+
+
+## Parameters:
+
+![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
+
+- Configurable:
+	- P: Proportional - Takes current value into account
+	- I: Integral - Takes past values into account
+	- D: Derivative - Takes future values into account
+	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
+	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
+	- Max Boil Output: Maximum Power during when Boil Temp is reached
+	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
+	- Max PID Temp: PID is switched off above this temperature
+	- RestOnActiveTimer: Yes: Pump will rest only on active step timer. No: Pump rest is not dependent on mash steps
+	- Rest Interval: Time interval in seconds after which Pump is switched off
+	- Rest Time: Pump is switched off for specified time in seconds
+	
+- Fixed in Code:
+	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
+
+
+Changelog:
+
+- 26.05.24: (0.1.7) De(activation) of pump pause during active timer as Option. Automode will now also work w/o steps
+- 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
+- 11.05.22: (0.1.5) Updated README (removed cbpi add)
+- 10.05.22: (0.1.4) removed cbpi dependency
+- 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be switched on at start and off if temp is above control limit. But no pump pause is triggered
+- 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
+- 21.11.21: Updated setup and Readme 
+- 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
+- 01.11.21: Merged Pull request from madhatguy and fixed some bugs
+- 15.03.21: Support for cbpi >= 4.0.0.32
+- 31.10.21: Changed logic to coroutines
+
+
```

### Comparing `cbpi4-BM_PID_SmartBoilWithPump-0.1.6/README.md` & `cbpi4-BM_PID_SmartBoilWithPump-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-# CBPi4 Braumeister Smart Boil with Pump KettleLogic
-
-### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
-
-## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
-- The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
-- It runs on PID control until it reaches a specified temperature. Above that temperature it heates w/o PID logic until a specified boil temp is reached.
-- Power to run boil can be specified in the plugin
-- Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
-
-
-### Installation:
-
-You can install it directly via pypi.org:	
-- sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
-
-Alternativeley you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
-- sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
-
-
-## Parameters:
-
-![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
-
-- Configurable:
-	- P: Proportional - Takes current value into account
-	- I: Integral - Takes past values into account
-	- D: Derivative - Takes future values into account
-	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
-	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
-	- Max Boil Output: Maximum Power during when Boil Temp is reached
-	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
-	- Max PID Temp: PID is switched off above this temperature
-	- Rest Interval: Time interval in seconds after which Pump is switched off
-	- Rest Time: Pump is switched off for specified time in seconds
-	
-- Fixed in Code:
-	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
-
-
-Changelog:
-
-- 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
-- 11.05.22: (0.1.5) Updated README (removed cbpi add)
-- 10.05.22: (0.1.4) removed cbpi dependency
-- 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be sitched on at start and off if temp is above controll limit. But no pump pause is triggered
-- 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
-- 21.11.21: Updated setup and Readme 
-- 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
-- 01.11.21: Merged Pull request from madhatguy ansd fixed some bugs
-- 15.03.21: Support for cbpi >= 4.0.0.32
-- 31.10.21: Changed logic to coroutines
+# CBPi4 Braumeister Smart Boil with Pump KettleLogic
+
+### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
+
+## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
+- The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
+- It runs on PID control until it reaches a specified temperature. Above that temperature it heats w/o PID logic until a specified boil temp is reached.
+- Power to run boil can be specified in the plugin
+- Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
+
+
+### Installation:
+
+You can install it directly via pypi.org:	
+- sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
+
+Alternatively you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
+- sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
+
+
+## Parameters:
+
+![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
+
+- Configurable:
+	- P: Proportional - Takes current value into account
+	- I: Integral - Takes past values into account
+	- D: Derivative - Takes future values into account
+	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
+	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
+	- Max Boil Output: Maximum Power during when Boil Temp is reached
+	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
+	- Max PID Temp: PID is switched off above this temperature
+	- RestOnActiveTimer: Yes: Pump will rest only on active step timer. No: Pump rest is not dependent on mash steps
+	- Rest Interval: Time interval in seconds after which Pump is switched off
+	- Rest Time: Pump is switched off for specified time in seconds
+	
+- Fixed in Code:
+	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
+
+
+Changelog:
+
+- 26.05.24: (0.1.7) De(activation) of pump pause during active timer as Option. Automode will now also work w/o steps
+- 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
+- 11.05.22: (0.1.5) Updated README (removed cbpi add)
+- 10.05.22: (0.1.4) removed cbpi dependency
+- 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be switched on at start and off if temp is above control limit. But no pump pause is triggered
+- 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
+- 21.11.21: Updated setup and Readme 
+- 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
+- 01.11.21: Merged Pull request from madhatguy and fixed some bugs
+- 15.03.21: Support for cbpi >= 4.0.0.32
+- 31.10.21: Changed logic to coroutines
```

### Comparing `cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4-BM_PID_SmartBoilWithPump/__init__.py` & `cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4-BM_PID_SmartBoilWithPump/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,269 @@
-import asyncio
-import logging
-from cbpi.api import *
-import time
-from cbpi.controller.step_controller import StepController
-import re
-
-
-@parameters([Property.Number(label="P", configurable=True, default_value=117.0795, description="P Value of PID"),
-             Property.Number(label="I", configurable=True, default_value=0.2747, description="I Value of PID"),
-             Property.Number(label="D", configurable=True, default_value=41.58, description="D Value of PID"),
-             Property.Select(label="SampleTime", options=[2,5], description="PID Sample time in seconds. Default: 5 (How often is the output calculation done)"),
-             Property.Number(label="Max_Pump_Temp", configurable=True, default_value=88,
-                             description="Max temp the pump can work in."),
-             Property.Number(label="Max_Boil_Output", configurable=True, default_value=85,
-                             description="Power when Max Boil Temperature is reached."),
-             Property.Number(label="Max_Boil_Temp", configurable=True, default_value=98,
-                             description="When Temperature reaches this, power will be reduced to Max Boil Output."),
-             Property.Number(label="Max_PID_Temp", configurable=True,
-                             description="When this temperature is reached, PID will be turned off"),
-             Property.Number(label="Rest_Interval", configurable=True, default_value=600,
-                             description="Rest the pump after this many seconds during the mash."),
-             Property.Number(label="Rest_Time", configurable=True, default_value=60,
-                             description="Rest the pump for this many seconds every rest interval.")])
-class BM_PID_SmartBoilWithPump(CBPiKettleLogic):
-
-    def __init__(self, cbpi, id, props):
-        super().__init__(cbpi, id, props)
-        self._logger = logging.getLogger(type(self).__name__)
-        self.sample_time, self.max_output, self.pid = None, None, None
-        self.work_time, self.rest_time, self.max_output_boil = None, None, None
-        self.max_boil_temp, self.max_pid_temp, self.max_pump_temp = None, None, None
-        self.kettle, self.heater, self.agitator = None, None, None
-
-        self.controller : StepController = cbpi.step
-
-    async def on_stop(self):
-        # ensure to switch also pump off when logic stops
-        await self.actor_off(self.agitator)
-
-    async def get_activity(self):
-        active_step = None
-        data=self.controller.get_state()
-        try:
-            steps=data['steps']
-            for step in steps:
-                if step['status'] == "A":
-                    active_step=step 
-        except:
-           pass 
-
-        return active_step
-
-    # subroutine that controlls pump aue and ump stop if max pump temp is reached
-    async def pump_control(self):
-        #get pump based on agitator id
-        self.pump = self.cbpi.actor.find_by_id(self.agitator)
-
-        await self.actor_on(self.agitator)
-
-        pump_rest = True
-        if (self.rest_time == 0) or (self.work_time == 0):
-            pump_rest = False
-
-        while self.running:
-            # get current pump status
-            pump_on = self.pump.instance.state
-            # if the current temp is below the max pump temp, check if pause time is reached to pause pump
-            if (self.get_sensor_value(self.kettle.sensor).get("value") < self.max_pump_temp):
-                if pump_rest == True:
-                    self._logger.debug("starting pump")
-                    #switch the pump on
-                    await self.actor_on(self.agitator)
-                    # calculate time, when pump should do the next pause
-                    off_time = time.time() + self.work_time
-                    # run pump until next pause time is reached
-                    while time.time() < off_time:
-                        await asyncio.sleep(1)
-                        # stop cycle, if current temp is higher than max pump temp
-                        if self.get_sensor_value(self.kettle.sensor).get("value") >= self.max_pump_temp:
-                            break
-                    # pause pump when active pump Interval is completed
-                    # check if timer is running or if step is ramping -> pump will be only paused if timer is running and not during ramp
-                    active_step = await self.get_activity()
-                    state_text=active_step.get('state_text')
-                    check_running_timer = re.compile('[0-9]{2}:[0-9]{2}:[0-9]{2}')
-                    if check_running_timer.match(state_text) is not None:
-                        self._logger.debug("resting pump")
-                        logging.info("Timer is running")
-                        logging.info("Step {}".format(state_text))
-                        await self.actor_off(self.agitator)
-                        await asyncio.sleep(self.rest_time)
-                else:
-                    await asyncio.sleep(1)
-            # If temeprature is above max pump temp, and pump is on, switch it off
-            # Staops also the pump if user switches it on and temp is abouve max pump temp
-            else:
-                if pump_on:
-                    self._logger.debug("pump max temp reached, pump turned off")
-                    await self.actor_off(self.agitator)
-                await asyncio.sleep(1)
-
-    # subroutine that controlls temperature via pid controll
-    async def temp_control(self):
-        await self.actor_on(self.heater,0)
-        logging.info("Heater on with zero Power")
-        heat_percent_old = 0
-        while self.running:
-            current_kettle_power= self.heater_actor.power
-            # get current temeprature
-            sensor_value = current_temp = self.get_sensor_value(self.kettle.sensor).get("value")
-            # get the current target temperature for the kettle
-            target_temp = self.get_kettle_target_temp(self.id)
-            # if current temperature is higher the defined boil temp, use fixed heating percent instead of PID values for controlled boiling
-            if current_temp >= self.max_boil_temp:
-                heat_percent = self.max_output_boil
-            # if current temperature is above max pid temp (should be higher than mashout temp and lower then max boil temp) 100% output will be used untile boil temp is reached
-            elif current_temp >= self.max_pid_temp:
-                heat_percent = self.max_output
-            # at lower temepratures, PID algorythm will valculate heat percent value
-            else:
-                heat_percent = self.pid.calc(sensor_value, target_temp)
-
-            # Test with actor power
-            if (heat_percent != heat_percent_old) or (heat_percent != current_kettle_power):
-                await self.actor_set_power(self.heater,heat_percent)
-                heat_percent_old = heat_percent
-            await asyncio.sleep(self.sample_time)
-
-    async def run(self):
-        try:
-            self.sample_time = int(self.props.get("SampleTime",5))
-            self.max_output = 100
-            p = float(self.props.get("P", 117.0795))
-            i = float(self.props.get("I", 0.2747))
-            d = float(self.props.get("D", 41.58))
-            self.pid = PIDArduino(self.sample_time, p, i, d, 0, self.max_output)
-
-            self.work_time = float(self.props.get("Rest_Interval", 600))
-            self.rest_time = float(self.props.get("Rest_Time", 60))
-            self.max_output_boil = float(self.props.get("Max_Boil_Output", 85))
-            
-            self.TEMP_UNIT = self.get_config_value("TEMP_UNIT", "C")
-            boilthreshold = 98 if self.TEMP_UNIT == "C" else 208
-            maxpidtemp = 88 if self.TEMP_UNIT == "C" else 190
-            maxpumptemp = 88 if self.TEMP_UNIT == "C" else 190
-
-
-            self.max_boil_temp = float(self.props.get("Max_Boil_Temp", boilthreshold))
-            self.max_pid_temp = float(self.props.get("Max_PID_Temp", maxpidtemp))
-            self.max_pump_temp = float(self.props.get("Max_Pump_Temp", maxpumptemp))
-
-            self.kettle = self.get_kettle(self.id)
-            self.heater = self.kettle.heater
-            self.agitator = self.kettle.agitator
-            self.heater_actor = self.cbpi.actor.find_by_id(self.heater)
-
-            logging.info("CustomLogic P:{} I:{} D:{} {} {}".format(p, i, d, self.kettle, self.heater))
-
-            pump_controller = asyncio.create_task(self.pump_control())
-            temp_controller = asyncio.create_task(self.temp_control())
-
-            await pump_controller
-            await temp_controller
-
-        except asyncio.CancelledError as e:
-            pass
-        except Exception as e:
-            logging.error("BM_PIDSmartBoilWithPump Error {}".format(e))
-        finally:
-            self.running = False
-            await self.actor_off(self.heater)
-
-
-# Based on Arduino PID Library
-# See https://github.com/br3ttb/Arduino-PID-Library
-class PIDArduino(object):
-
-    def __init__(self, sampleTimeSec, kp, ki, kd, outputMin=float('-inf'),
-                 outputMax=float('inf'), getTimeMs=None):
-        if kp is None:
-            raise ValueError('kp must be specified')
-        if ki is None:
-            raise ValueError('ki must be specified')
-        if kd is None:
-            raise ValueError('kd must be specified')
-        if float(sampleTimeSec) <= float(0):
-            raise ValueError('sampleTimeSec must be greater than 0')
-        if outputMin >= outputMax:
-            raise ValueError('outputMin must be less than outputMax')
-
-        self._logger = logging.getLogger(type(self).__name__)
-        self._Kp = kp
-        self._Ki = ki * sampleTimeSec
-        self._Kd = kd / sampleTimeSec
-        self._sampleTime = sampleTimeSec * 1000
-        self._outputMin = outputMin
-        self._outputMax = outputMax
-        self._iTerm = 0
-        self._lastInput = 0
-        self._lastOutput = 0
-        self._lastCalc = 0
-
-        if getTimeMs is None:
-            self._getTimeMs = self._currentTimeMs
-        else:
-            self._getTimeMs = getTimeMs
-
-    def calc(self, inputValue, setpoint):
-        now = self._getTimeMs()
-
-        if (now - self._lastCalc) < self._sampleTime:
-            return self._lastOutput
-
-        # Compute all the working error variables
-        error = setpoint - inputValue
-        dInput = inputValue - self._lastInput
-
-        # In order to prevent windup, only integrate if the process is not saturated
-        if self._outputMax > self._lastOutput > self._outputMin:
-            self._iTerm += self._Ki * error
-            self._iTerm = min(self._iTerm, self._outputMax)
-            self._iTerm = max(self._iTerm, self._outputMin)
-
-        p = self._Kp * error
-        i = self._iTerm
-        d = -(self._Kd * dInput)
-
-        # Compute PID Output
-        self._lastOutput = p + i + d
-        self._lastOutput = min(self._lastOutput, self._outputMax)
-        self._lastOutput = max(self._lastOutput, self._outputMin)
-
-        # Log some debug info
-        self._logger.debug('P: {0}'.format(p))
-        self._logger.debug('I: {0}'.format(i))
-        self._logger.debug('D: {0}'.format(d))
-        self._logger.debug('output: {0}'.format(self._lastOutput))
-
-        # Remember some variables for next time
-        self._lastInput = inputValue
-        self._lastCalc = now
-        return self._lastOutput
-
-    def _currentTimeMs(self):
-        return time.time() * 1000
-
-
-def setup(cbpi):
-    '''
-    This method is called by the server during startup 
-    Here you need to register your plugins at the server
-    
-    :param cbpi: the cbpi core 
-    :return: 
-    '''
-
-    cbpi.plugin.register("BM_PID_SmartBoilWithPump", BM_PID_SmartBoilWithPump)
+import asyncio
+import logging
+from cbpi.api import *
+import time
+from cbpi.controller.step_controller import StepController
+import re
+
+
+@parameters([Property.Number(label="P", configurable=True, default_value=117.0795, description="P Value of PID"),
+             Property.Number(label="I", configurable=True, default_value=0.2747, description="I Value of PID"),
+             Property.Number(label="D", configurable=True, default_value=41.58, description="D Value of PID"),
+             Property.Select(label="SampleTime", options=[2,5], description="PID Sample time in seconds. Default: 5 (How often is the output calculation done)"),
+             Property.Number(label="Max_Pump_Temp", configurable=True, default_value=88,
+                             description="Max temp the pump can work in."),
+             Property.Number(label="Max_Boil_Output", configurable=True, default_value=85,
+                             description="Power when Max Boil Temperature is reached."),
+             Property.Number(label="Max_Boil_Temp", configurable=True, default_value=98,
+                             description="When Temperature reaches this, power will be reduced to Max Boil Output."),
+             Property.Number(label="Max_PID_Temp", configurable=True,
+                             description="When this temperature is reached, PID will be turned off"),
+             Property.Select(label="RestOnActiveTimer", options=["Yes","No"], description="Rest Pump only on active step timer (not during temp ramp). Default: Yes"),                             
+             Property.Number(label="Rest_Interval", configurable=True, default_value=600,
+                             description="Rest the pump after this many seconds during the mash."),
+             Property.Number(label="Rest_Time", configurable=True, default_value=60,
+                             description="Rest the pump for this many seconds every rest interval.")])
+class BM_PID_SmartBoilWithPump(CBPiKettleLogic):
+
+    def __init__(self, cbpi, id, props):
+        super().__init__(cbpi, id, props)
+        self._logger = logging.getLogger(type(self).__name__)
+        self.sample_time, self.max_output, self.pid = None, None, None
+        self.work_time, self.rest_time, self.max_output_boil = None, None, None
+        self.max_boil_temp, self.max_pid_temp, self.max_pump_temp = None, None, None
+        self.kettle, self.heater, self.agitator = None, None, None
+
+        self.controller : StepController = cbpi.step
+
+    async def on_stop(self):
+        # ensure to switch also pump off when logic stops
+        await self.actor_off(self.agitator)
+
+    async def get_activity(self):
+        active_step = None
+        data=self.controller.get_state()
+        try:
+            steps=data['steps']
+            for step in steps:
+                if step['status'] == "A":
+                    active_step=step 
+        except:
+           pass 
+
+        return active_step
+
+    # subroutine that controlls pump aue and ump stop if max pump temp is reached
+    async def pump_control(self):
+        #get pump based on agitator id
+        self.pump = self.cbpi.actor.find_by_id(self.agitator)
+
+        await self.actor_on(self.agitator)
+
+        pump_rest = True
+        if (self.rest_time == 0) or (self.work_time == 0):
+            pump_rest = False
+
+        while self.running:
+            # get current pump status
+            pump_on = self.pump.instance.state
+            # if the current temp is below the max pump temp, check if pause time is reached to pause pump
+            if (self.get_sensor_value(self.kettle.sensor).get("value") < self.max_pump_temp):
+                if pump_rest == True:
+                    self._logger.debug("starting pump")
+                    #switch the pump on
+                    await self.actor_on(self.agitator)
+                    # calculate time, when pump should do the next pause
+                    off_time = time.time() + self.work_time
+                    # run pump until next pause time is reached
+                    while time.time() < off_time:
+                        await asyncio.sleep(1)
+                        # stop cycle, if current temp is higher than max pump temp
+                        if self.get_sensor_value(self.kettle.sensor).get("value") >= self.max_pump_temp:
+                            break
+                    # pause pump when active pump Interval is completed
+                    try:
+                        active_step = await self.get_activity()
+                        state_text=active_step.get('state_text')
+                    except:
+                        active_step = None
+                    if self.rest_on_active_timer and active_step is not None:
+                        # check if timer is running or if step is ramping -> pump will be only paused if timer is running and not during ramp
+                        check_running_timer = re.compile('[0-9]{2}:[0-9]{2}:[0-9]{2}')
+                        if check_running_timer.match(state_text) is not None:
+                            self._logger.debug("resting pump")
+                            logging.debug("Timer is running")
+                            logging.debug("Step {}".format(state_text))
+                            await self.actor_off(self.agitator)
+                            await asyncio.sleep(self.rest_time)
+                    else:
+                            self._logger.debug("resting pump")
+                            await self.actor_off(self.agitator)
+                            await asyncio.sleep(self.rest_time)
+                else:
+                    await asyncio.sleep(1)
+            # If temperature is above max pump temp, and pump is on, switch it off
+            # Stops also the pump if user switches it on and temp is above max pump temp
+            else:
+                if pump_on:
+                    self._logger.debug("pump max temp reached, pump turned off")
+                    await self.actor_off(self.agitator)
+                await asyncio.sleep(1)
+
+    # subroutine that controls temperature via pid control
+    async def temp_control(self):
+        await self.actor_on(self.heater,0)
+        logging.info("Heater on with zero Power")
+        heat_percent_old = 0
+        while self.running:
+            current_kettle_power= self.heater_actor.power
+            # get current temperature
+            sensor_value = current_temp = self.get_sensor_value(self.kettle.sensor).get("value")
+            # get the current target temperature for the kettle
+            target_temp = self.get_kettle_target_temp(self.id)
+            # if current temperature is higher the defined boil temp, use fixed heating percent instead of PID values for controlled boiling
+            if current_temp >= self.max_boil_temp:
+                heat_percent = self.max_output_boil
+            # if current temperature is above max pid temp (should be higher than mashout temp and lower then max boil temp) 100% output will be used until boil temp is reached
+            elif current_temp >= self.max_pid_temp:
+                heat_percent = self.max_output
+            # at lower temperatures, PID algorithm will calculate heat percent value
+            else:
+                heat_percent = self.pid.calc(sensor_value, target_temp)
+
+            # Test with actor power
+            if (heat_percent != heat_percent_old) or (heat_percent != current_kettle_power):
+                await self.actor_set_power(self.heater,heat_percent)
+                heat_percent_old = heat_percent
+            await asyncio.sleep(self.sample_time)
+
+    async def run(self):
+        try:
+            self.sample_time = int(self.props.get("SampleTime",5))
+            self.max_output = 100
+            p = float(self.props.get("P", 117.0795))
+            i = float(self.props.get("I", 0.2747))
+            d = float(self.props.get("D", 41.58))
+            self.pid = PIDArduino(self.sample_time, p, i, d, 0, self.max_output)
+
+            self.work_time = float(self.props.get("Rest_Interval", 600))
+            self.rest_time = float(self.props.get("Rest_Time", 60))
+            self.max_output_boil = float(self.props.get("Max_Boil_Output", 85))
+            self.restonactivetimer = self.props.get("RestOnActiveTimer", "Yes")
+            self.rest_on_active_timer = True if self.restonactivetimer == "Yes" else False
+            
+            self.TEMP_UNIT = self.get_config_value("TEMP_UNIT", "C")
+            boilthreshold = 98 if self.TEMP_UNIT == "C" else 208
+            maxpidtemp = 88 if self.TEMP_UNIT == "C" else 190
+            maxpumptemp = 88 if self.TEMP_UNIT == "C" else 190
+
+
+            self.max_boil_temp = float(self.props.get("Max_Boil_Temp", boilthreshold))
+            self.max_pid_temp = float(self.props.get("Max_PID_Temp", maxpidtemp))
+            self.max_pump_temp = float(self.props.get("Max_Pump_Temp", maxpumptemp))
+
+            self.kettle = self.get_kettle(self.id)
+            self.heater = self.kettle.heater
+            self.agitator = self.kettle.agitator
+            self.heater_actor = self.cbpi.actor.find_by_id(self.heater)
+
+            logging.info("CustomLogic P:{} I:{} D:{} {} {}".format(p, i, d, self.kettle, self.heater))
+
+            pump_controller = asyncio.create_task(self.pump_control())
+            temp_controller = asyncio.create_task(self.temp_control())
+
+            await pump_controller
+            await temp_controller
+
+        except asyncio.CancelledError as e:
+            pass
+        except Exception as e:
+            logging.error("BM_PIDSmartBoilWithPump Error {}".format(e))
+        finally:
+            self.running = False
+            await self.actor_off(self.heater)
+
+
+# Based on Arduino PID Library
+# See https://github.com/br3ttb/Arduino-PID-Library
+class PIDArduino(object):
+
+    def __init__(self, sampleTimeSec, kp, ki, kd, outputMin=float('-inf'),
+                 outputMax=float('inf'), getTimeMs=None):
+        if kp is None:
+            raise ValueError('kp must be specified')
+        if ki is None:
+            raise ValueError('ki must be specified')
+        if kd is None:
+            raise ValueError('kd must be specified')
+        if float(sampleTimeSec) <= float(0):
+            raise ValueError('sampleTimeSec must be greater than 0')
+        if outputMin >= outputMax:
+            raise ValueError('outputMin must be less than outputMax')
+
+        self._logger = logging.getLogger(type(self).__name__)
+        self._Kp = kp
+        self._Ki = ki * sampleTimeSec
+        self._Kd = kd / sampleTimeSec
+        self._sampleTime = sampleTimeSec * 1000
+        self._outputMin = outputMin
+        self._outputMax = outputMax
+        self._iTerm = 0
+        self._lastInput = 0
+        self._lastOutput = 0
+        self._lastCalc = 0
+
+        if getTimeMs is None:
+            self._getTimeMs = self._currentTimeMs
+        else:
+            self._getTimeMs = getTimeMs
+
+    def calc(self, inputValue, setpoint):
+        now = self._getTimeMs()
+
+        if (now - self._lastCalc) < self._sampleTime:
+            return self._lastOutput
+
+        # Compute all the working error variables
+        error = setpoint - inputValue
+        dInput = inputValue - self._lastInput
+
+        # In order to prevent windup, only integrate if the process is not saturated
+        if self._outputMax > self._lastOutput > self._outputMin:
+            self._iTerm += self._Ki * error
+            self._iTerm = min(self._iTerm, self._outputMax)
+            self._iTerm = max(self._iTerm, self._outputMin)
+
+        p = self._Kp * error
+        i = self._iTerm
+        d = -(self._Kd * dInput)
+
+        # Compute PID Output
+        self._lastOutput = p + i + d
+        self._lastOutput = min(self._lastOutput, self._outputMax)
+        self._lastOutput = max(self._lastOutput, self._outputMin)
+
+        # Log some debug info
+        self._logger.debug('P: {0}'.format(p))
+        self._logger.debug('I: {0}'.format(i))
+        self._logger.debug('D: {0}'.format(d))
+        self._logger.debug('output: {0}'.format(self._lastOutput))
+
+        # Remember some variables for next time
+        self._lastInput = inputValue
+        self._lastCalc = now
+        return self._lastOutput
+
+    def _currentTimeMs(self):
+        return time.time() * 1000
+
+
+def setup(cbpi):
+    '''
+    This method is called by the server during startup 
+    Here you need to register your plugins at the server
+    
+    :param cbpi: the cbpi core 
+    :return: 
+    '''
+
+    cbpi.plugin.register("BM_PID_SmartBoilWithPump", BM_PID_SmartBoilWithPump)
```

### Comparing `cbpi4-BM_PID_SmartBoilWithPump-0.1.6/cbpi4_BM_PID_SmartBoilWithPump.egg-info/PKG-INFO` & `cbpi4-BM_PID_SmartBoilWithPump-0.1.7/cbpi4_BM_PID_SmartBoilWithPump.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-Metadata-Version: 2.1
-Name: cbpi4-BM-PID-SmartBoilWithPump
-Version: 0.1.6
-Summary: CraftBeerPi4 PID Kettle Logic Plugin
-Home-page: https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump
-Author: ['Alexander Vollkopf', 'Guy Lev']
-Author-email: avollkopf@web.de
-License: GPLv3
-Description: # CBPi4 Braumeister Smart Boil with Pump KettleLogic
-        
-        ### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
-        
-        ## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
-        - The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
-        - It runs on PID control until it reaches a specified temperature. Above that temperature it heates w/o PID logic until a specified boil temp is reached.
-        - Power to run boil can be specified in the plugin
-        - Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
-        
-        
-        ### Installation:
-        
-        You can install it directly via pypi.org:	
-        - sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
-        
-        Alternativeley you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
-        - sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
-        
-        
-        ## Parameters:
-        
-        ![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
-        
-        - Configurable:
-        	- P: Proportional - Takes current value into account
-        	- I: Integral - Takes past values into account
-        	- D: Derivative - Takes future values into account
-        	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
-        	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
-        	- Max Boil Output: Maximum Power during when Boil Temp is reached
-        	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
-        	- Max PID Temp: PID is switched off above this temperature
-        	- Rest Interval: Time interval in seconds after which Pump is switched off
-        	- Rest Time: Pump is switched off for specified time in seconds
-        	
-        - Fixed in Code:
-        	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
-        
-        
-        Changelog:
-        
-        - 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
-        - 11.05.22: (0.1.5) Updated README (removed cbpi add)
-        - 10.05.22: (0.1.4) removed cbpi dependency
-        - 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be sitched on at start and off if temp is above controll limit. But no pump pause is triggered
-        - 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
-        - 21.11.21: Updated setup and Readme 
-        - 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
-        - 01.11.21: Merged Pull request from madhatguy ansd fixed some bugs
-        - 15.03.21: Support for cbpi >= 4.0.0.32
-        - 31.10.21: Changed logic to coroutines
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: cbpi4-BM-PID-SmartBoilWithPump
+Version: 0.1.7
+Summary: CraftBeerPi4 PID Kettle Logic Plugin
+Home-page: https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump
+Author: ['Alexander Vollkopf', 'Guy Lev']
+Author-email: avollkopf@web.de
+License: GPLv3
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CBPi4 Braumeister Smart Boil with Pump KettleLogic
+
+### This Kettle Logic can be used to run a Speidel Braumeister with CraftbeerPi4. It is based on this cbpi3 Plugin (https://github.com/cgspeck/cbpi-pidsmartboil-withpump)
+
+## Mash & Boil in single Kettle (e.g. Speidel Braumeister)
+- The Kettle logic is intended to be used in a single Kettle. It is a PID logic. PID parameters can be for instance derived from the PID AutoTune plugin (https://github.com/avollkopf/cbpi4-PIDAutoTune)
+- It runs on PID control until it reaches a specified temperature. Above that temperature it heats w/o PID logic until a specified boil temp is reached.
+- Power to run boil can be specified in the plugin
+- Pump Intervals cen be set to have a pump rest on specified intervals for a specified time (e.g. 60 seconds every 600 seconds which is a default for the Braumeister controller)
+
+
+### Installation:
+
+You can install it directly via pypi.org:	
+- sudo pip3 install cbpi4-BM-PID-SmartBoilWithPump 
+
+Alternatively you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
+- sudo pip3 install https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/archive/main.zip
+
+
+## Parameters:
+
+![Settings](https://github.com/avollkopf/cbpi4-BM_PID_SmartBoilWithPump/blob/main/cbpi4-BM_PID_SmartBoilWithPump-logic.png?raw=true)
+
+- Configurable:
+	- P: Proportional - Takes current value into account
+	- I: Integral - Takes past values into account
+	- D: Derivative - Takes future values into account
+	- SampleTime - 2 or 5 seconds -> how often the logic calculates the power setting
+	- Max Pump Temp: Pump is switched off above this temperature and cannot be switched back on
+	- Max Boil Output: Maximum Power during when Boil Temp is reached
+	- Max Boil Temp: When Temp is reached, power is set to Max Boil Output
+	- Max PID Temp: PID is switched off above this temperature
+	- RestOnActiveTimer: Yes: Pump will rest only on active step timer. No: Pump rest is not dependent on mash steps
+	- Rest Interval: Time interval in seconds after which Pump is switched off
+	- Rest Time: Pump is switched off for specified time in seconds
+	
+- Fixed in Code:
+	- Max Output: Maximum Power (%) to be used for PID during Ramp up -> 100%
+
+
+Changelog:
+
+- 26.05.24: (0.1.7) De(activation) of pump pause during active timer as Option. Automode will now also work w/o steps
+- 14.06.22: (0.1.6) Disable pump pause during temperature ramp -> pause will take effect only on active timer
+- 11.05.22: (0.1.5) Updated README (removed cbpi add)
+- 10.05.22: (0.1.4) removed cbpi dependency
+- 30.12.21: (0.1.3) Fixed 0 pump/rest time -> Pump will be switched on at start and off if temp is above control limit. But no pump pause is triggered
+- 01.12.21: (0.1.2) Added security feature: current kettle power is monitored continuously and overwritten in case it's different from the logic loop value
+- 21.11.21: Updated setup and Readme 
+- 15.11.21: Adapted to cbpi 4.0.0.45 with actor power settings
+- 01.11.21: Merged Pull request from madhatguy and fixed some bugs
+- 15.03.21: Support for cbpi >= 4.0.0.32
+- 31.10.21: Changed logic to coroutines
+
+
```

