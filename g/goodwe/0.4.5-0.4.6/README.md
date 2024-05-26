# Comparing `tmp/goodwe-0.4.5.tar.gz` & `tmp/goodwe-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.4.5.tar", last modified: Tue May 21 20:41:45 2024, max compression
+gzip compressed data, was "goodwe-0.4.6.tar", last modified: Sun May 26 18:02:40 2024, max compression
```

## Comparing `goodwe-0.4.5.tar` & `goodwe-0.4.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:41:45.668945 goodwe-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 20:41:38.000000 goodwe-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-21 20:41:45.668945 goodwe-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-21 20:41:38.000000 goodwe-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 20:41:42.000000 goodwe-0.4.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:41:45.668945 goodwe-0.4.5/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    29140 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-21 20:41:38.000000 goodwe-0.4.5/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:41:45.668945 goodwe-0.4.5/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-21 20:41:45.000000 goodwe-0.4.5/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-21 20:41:45.000000 goodwe-0.4.5/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:41:45.000000 goodwe-0.4.5/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 20:41:45.000000 goodwe-0.4.5/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 20:41:38.000000 goodwe-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 20:41:45.672945 goodwe-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:41:45.668945 goodwe-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-21 20:41:38.000000 goodwe-0.4.5/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:02:40.972476 goodwe-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-26 18:02:33.000000 goodwe-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-26 18:02:40.972476 goodwe-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-26 18:02:33.000000 goodwe-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 18:02:38.000000 goodwe-0.4.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:02:40.972476 goodwe-0.4.6/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30083 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37707 2024-05-26 18:02:33.000000 goodwe-0.4.6/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:02:40.972476 goodwe-0.4.6/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-26 18:02:40.000000 goodwe-0.4.6/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-26 18:02:40.000000 goodwe-0.4.6/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:02:40.000000 goodwe-0.4.6/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 18:02:40.000000 goodwe-0.4.6/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-26 18:02:33.000000 goodwe-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-26 18:02:40.976476 goodwe-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:02:40.972476 goodwe-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-26 18:02:33.000000 goodwe-0.4.6/tests/test_sensor.py
```

### Comparing `goodwe-0.4.5/LICENSE` & `goodwe-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/PKG-INFO` & `goodwe-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.5
+Version: 0.4.6
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.5/README.md` & `goodwe-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/__init__.py` & `goodwe-0.4.6/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/const.py` & `goodwe-0.4.6/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/dt.py` & `goodwe-0.4.6/goodwe/dt.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,18 @@
     # Modbus registers of inverter settings, offsets are modbus register addresses
     __all_settings: Tuple[Sensor, ...] = (
         Timestamp("time", 40313, "Inverter time"),
 
         Integer("shadow_scan", 40326, "Shadow Scan", "", Kind.PV),
         Integer("grid_export", 40327, "Grid Export Enabled", "", Kind.GRID),
         Integer("grid_export_limit", 40328, "Grid Export Limit", "%", Kind.GRID),
+        Integer("start", 40330, "Start / Power On", "", Kind.GRID),
+        Integer("stop", 40331, "Stop / Power Off", "", Kind.GRID),
+        Integer("restart", 40332, "Restart", "", Kind.GRID),
+        Integer("grid_export_hw", 40345, "Grid Export Enabled (HW)", "", Kind.GRID),
     )
 
     # Settings for single phase inverters
     __settings_single_phase: Tuple[Sensor, ...] = (
         Long("grid_export_limit", 40328, "Grid Export Limit", "W", Kind.GRID),
     )
 
@@ -192,14 +196,15 @@
             count = (setting.size_ + (setting.size_ % 2)) // 2
             response = await self._read_from_socket(self._read_command(setting.offset, count))
             return setting.read_value(response)
         except RequestRejectedException as ex:
             if ex.message == ILLEGAL_DATA_ADDRESS:
                 logger.debug("Unsupported setting %s", setting.id_)
                 self._settings.pop(setting.id_, None)
+                raise ValueError(f'Unknown setting "{setting.id_}"')
             return None
 
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
         if setting:
             await self._write_setting(setting, value)
         else:
```

### Comparing `goodwe-0.4.5/goodwe/es.py` & `goodwe-0.4.6/goodwe/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,29 +170,29 @@
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
         super().__init__(host, port, comm_addr if comm_addr else 0xf7, timeout, retries)
         self._settings: dict[str, Sensor] = {s.id_: s for s in self.__all_settings}
 
     def _supports_eco_mode_v2(self) -> bool:
         if self.arm_version < 14:
             return False
-        if "EMU" in self.serial_number:
+        if "EMU" in self.serial_number or "EMJ" in self.serial_number:
             return self.dsp1_version >= 11
-        if "ESU" in self.serial_number:
+        if "ESU" in self.serial_number or "ESA" in self.serial_number:
             return self.dsp1_version >= 22
-        if "BPS" in self.serial_number:
+        if "BPS" in self.serial_number or "BPU" in self.serial_number:
             return self.dsp1_version >= 10
         return False
 
     async def read_device_info(self):
         response = await self._read_from_socket(self._READ_DEVICE_VERSION_INFO)
         response = response.response_data()
         self.firmware = self._decode(response[0:5]).rstrip()
         self.model_name = self._decode(response[5:15]).rstrip()
         self.serial_number = self._decode(response[31:47])
-        self.software_version = self._decode(response[51:63])
+        self.arm_firmware = self._decode(response[51:63])  # AKA software_version
         try:
             if len(self.firmware) >= 2:
                 self.dsp1_version = int(self.firmware[0:2])
             if len(self.firmware) >= 4:
                 self.dsp2_version = int(self.firmware[2:4])
             if len(self.firmware) >= 5:
                 self.arm_version = int(self.firmware[4], base=36)
@@ -216,17 +216,20 @@
             setting: Sensor | None = self._settings.get(setting_id)
             if not setting:
                 raise ValueError(f'Unknown setting "{setting_id}"')
             return await self._read_setting(setting)
         elif setting_id.startswith("modbus"):
             response = await self._read_from_socket(self._read_command(int(setting_id[7:]), 1))
             return int.from_bytes(response.read(2), byteorder="big", signed=True)
-        else:
+        elif setting_id in self._settings:
+            logger.debug("Reading setting %s", setting_id)
             all_settings = await self.read_settings_data()
             return all_settings.get(setting_id)
+        else:
+            raise ValueError(f'Unknown setting "{setting_id}"')
 
     async def _read_setting(self, setting: Sensor) -> Any:
         count = (setting.size_ + (setting.size_ % 2)) // 2
         if self._is_modbus_setting(setting):
             response = await self._read_from_socket(self._read_command(setting.offset, count))
             return setting.read_value(response)
         else:
@@ -292,15 +295,15 @@
         return tuple(result)
 
     async def get_operation_mode(self) -> OperationMode | None:
         mode_id = await self.read_setting('work_mode')
         try:
             mode = OperationMode(mode_id)
         except ValueError:
-            logger.debug("Unknown work_mode value %d", mode_id)
+            logger.debug("Unknown work_mode value %s", mode_id)
             return None
         if OperationMode.ECO != mode:
             return mode
         eco_mode = await self.read_setting('eco_mode_1')
         if eco_mode.is_eco_charge_mode():
             return OperationMode.ECO_CHARGE
         elif eco_mode.is_eco_discharge_mode():
```

### Comparing `goodwe-0.4.5/goodwe/et.py` & `goodwe-0.4.6/goodwe/et.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,15 @@
         Apparent4("apparent_power2", 35361, "Apparent Power L2", Kind.GRID),
         Apparent4("apparent_power3", 35363, "Apparent Power L3", Kind.GRID),
     )
 
     # Modbus registers of inverter settings, offsets are modbus register addresses
     __all_settings: Tuple[Sensor, ...] = (
         Integer("comm_address", 45127, "Communication Address", ""),
-        Integer("modbus_baud_rate", 45132, "Modbus Baud rate", ""),
+        Long("modbus_baud_rate", 45132, "Modbus Baud rate", ""),
         Timestamp("time", 45200, "Inverter time"),
 
         Integer("sensitivity_check", 45246, "Sensitivity Check Mode", "", Kind.AC),
         Integer("cold_start", 45248, "Cold Start", "", Kind.AC),
         Integer("shadow_scan", 45251, "Shadow Scan", "", Kind.PV),
         Integer("backup_supply", 45252, "Backup Supply", "", Kind.UPS),
         Integer("unbalanced_output", 45264, "Unbalanced Output", "", Kind.AC),
@@ -353,14 +353,16 @@
         Integer("battery_discharge_depth_offline", 45358, "Battery Discharge Depth (off-line)", "%", Kind.BAT),
 
         Decimal("power_factor", 45482, 100, "Power Factor"),
 
         Integer("work_mode", 47000, "Work Mode", "", Kind.AC),
         Integer("dred", 47010, "DRED/Remote Shutdown", "", Kind.AC),
 
+        Integer("meter_target_power_offset", 47120, "Meter Target Power Offset", "W", Kind.AC),
+
         Integer("battery_soc_protection", 47500, "Battery SoC Protection", "", Kind.BAT),
 
         Integer("grid_export", 47509, "Grid Export Enabled", "", Kind.GRID),
         Integer("grid_export_limit", 47510, "Grid Export Limit", "W", Kind.GRID),
 
         Integer("battery_protocol_code", 47514, "Battery Protocol Code", "", Kind.BAT),
 
@@ -622,14 +624,15 @@
             count = (setting.size_ + (setting.size_ % 2)) // 2
             response = await self._read_from_socket(self._read_command(setting.offset, count))
             return setting.read_value(response)
         except RequestRejectedException as ex:
             if ex.message == ILLEGAL_DATA_ADDRESS:
                 logger.debug("Unsupported setting %s", setting.id_)
                 self._settings.pop(setting.id_, None)
+                raise ValueError(f'Unknown setting "{setting.id_}"')
             return None
 
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
         if setting:
             await self._write_setting(setting, value)
         else:
@@ -681,15 +684,15 @@
         return tuple(result)
 
     async def get_operation_mode(self) -> OperationMode | None:
         mode_id = await self.read_setting('work_mode')
         try:
             mode = OperationMode(mode_id)
         except ValueError:
-            logger.debug("Unknown work_mode value %d", mode_id)
+            logger.debug("Unknown work_mode value %s", mode_id)
             return None
         if OperationMode.ECO != mode:
             return mode
         eco_mode = await self.read_setting('eco_mode_1')
         if eco_mode.is_eco_charge_mode():
             return OperationMode.ECO_CHARGE
         elif eco_mode.is_eco_discharge_mode():
```

### Comparing `goodwe-0.4.5/goodwe/exceptions.py` & `goodwe-0.4.6/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/inverter.py` & `goodwe-0.4.6/goodwe/inverter.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/modbus.py` & `goodwe-0.4.6/goodwe/modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/model.py` & `goodwe-0.4.6/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/goodwe/protocol.py` & `goodwe-0.4.6/goodwe/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -478,23 +478,25 @@
     It is suffixed with 2 bytes of plain checksum of header+payload.
 
     Response starts again with 0xAA, 0x55, then 0x7F, 0xC0.
     5-6th bytes are some response type, byte 7 is length of the response payload.
     The last 2 bytes are again plain checksum of header+payload.
     """
 
-    def __init__(self, payload: str, response_type: str):
+    def __init__(self, payload: str, response_type: str, offset: int = 0, value: int = 0):
         super().__init__(
             bytes.fromhex(
                 "AA55C07F"
                 + payload
                 + self._checksum(bytes.fromhex("AA55C07F" + payload)).hex()
             ),
             lambda x: self._validate_aa55_response(x, response_type),
         )
+        self.first_address: int = offset
+        self.value = value
 
     @staticmethod
     def _checksum(data: bytes) -> bytes:
         checksum = 0
         for each in data:
             checksum += each
         return checksum.to_bytes(2, byteorder="big", signed=False)
@@ -530,41 +532,61 @@
             return False
         return True
 
     def trim_response(self, raw_response: bytes):
         """Trim raw response from header and checksum data"""
         return raw_response[7:-2]
 
+    def __repr__(self):
+        if self.request[4] == 1:
+            if self.request[5] == 2:
+                return f'READ device info ({self.request.hex()})'
+            elif self.request[5] == 6:
+                return f'READ runtime data ({self.request.hex()})'
+            elif self.request[5] == 9:
+                return f'READ settings ({self.request.hex()})'
+        else:
+            return self.request.hex()
+
 
 class Aa55ReadCommand(Aa55ProtocolCommand):
     """
     Inverter modbus READ command for retrieving <count> modbus registers starting at register # <offset>
     """
 
     def __init__(self, offset: int, count: int):
-        super().__init__("011A03" + "{:04x}".format(offset) + "{:02x}".format(count), "019A")
+        super().__init__("011A03" + "{:04x}".format(offset) + "{:02x}".format(count), "019A", offset, count)
+
+    def __repr__(self):
+        if self.value > 1:
+            return f'READ {self.value} registers from {self.first_address} ({self.request.hex()})'
+        else:
+            return f'READ register {self.first_address} ({self.request.hex()})'
 
 
 class Aa55WriteCommand(Aa55ProtocolCommand):
     """
     Inverter aa55 WRITE command setting single register # <register> value <value>
     """
 
     def __init__(self, register: int, value: int):
-        super().__init__("023905" + "{:04x}".format(register) + "01" + "{:04x}".format(value), "02B9")
+        super().__init__("023905" + "{:04x}".format(register) + "01" + "{:04x}".format(value), "02B9", register, value)
+
+    def __repr__(self):
+        return f'WRITE {self.value} to register {self.first_address} ({self.request.hex()})'
 
 
 class Aa55WriteMultiCommand(Aa55ProtocolCommand):
     """
     Inverter aa55 WRITE command setting multiple register # <register> value <value>
     """
 
     def __init__(self, offset: int, values: bytes):
         super().__init__("02390B" + "{:04x}".format(offset) + "{:02x}".format(len(values)) + values.hex(),
-                         "02B9")
+                         "02B9", offset, len(values) // 2)
 
 
 class ModbusRtuProtocolCommand(ProtocolCommand):
     """
     Inverter communication protocol seen on newer generation of inverters, based on Modbus
     protocol over UDP transport layer.
     The modbus communication is rather simple, there are "registers" at specified addresses/offsets,
```

### Comparing `goodwe-0.4.5/goodwe/sensor.py` & `goodwe-0.4.6/goodwe/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         super().__init__(id_, offset, name, 2, unit, kind)
         self.scale = scale
 
     def read_value(self, data: ProtocolResponse):
         return read_decimal2(data, self.scale)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
-        return int.to_bytes(int(value * self.scale), length=2, byteorder="big", signed=True)
+        return int.to_bytes(int(float(value) * self.scale), length=2, byteorder="big", signed=True)
 
 
 class Float(Sensor):
     """Sensor representing signed int value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, scale: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 4, unit, kind)
@@ -864,15 +864,15 @@
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
     return float(value) / 10 if value != 0xffff else 0
 
 
 def encode_voltage(value: Any) -> bytes:
     """Encode voltage value to raw (2 unsigned bytes) payload"""
-    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=False)
+    return int.to_bytes(int(float(value) * 10), length=2, byteorder="big", signed=False)
 
 
 def read_current(buffer: ProtocolResponse, offset: int = None) -> float:
     """Retrieve current [A] value (2 unsigned bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
@@ -885,20 +885,20 @@
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
     return float(value) / 10
 
 
 def encode_current(value: Any) -> bytes:
     """Encode current value to raw (2 unsigned bytes) payload"""
-    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=False)
+    return int.to_bytes(int(float(value) * 10), length=2, byteorder="big", signed=False)
 
 
 def encode_current_signed(value: Any) -> bytes:
     """Encode current value to raw (2 signed bytes) payload"""
-    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=True)
+    return int.to_bytes(int(float(value) * 10), length=2, byteorder="big", signed=True)
 
 
 def read_freq(buffer: ProtocolResponse, offset: int = None) -> float:
     """Retrieve frequency [Hz] value (2 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
```

### Comparing `goodwe-0.4.5/goodwe.egg-info/PKG-INFO` & `goodwe-0.4.6/goodwe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.5
+Version: 0.4.6
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.5/setup.cfg` & `goodwe-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/tests/test_dt.py` & `goodwe-0.4.6/tests/test_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self.assertSensor('vnbus', 305.4, 'V', data)
         self.assertSensor('derating_mode', 0, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
         self.assertFalse(self.sensor_map, f"Some sensors were not tested {self.sensor_map}")
 
     def test_GW6000_DT_setting(self):
-        self.assertEqual(4, len(self.settings()))
+        self.assertEqual(8, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('Timestamp', type(settings.get("time")).__name__)
         self.assertEqual('Integer', type(settings.get("grid_export")).__name__)
         self.assertEqual('Integer', type(settings.get("grid_export_limit")).__name__)
 
     def test_GW6000_DT_read_setting(self):
         self.loop.run_until_complete(self.read_setting('shadow_scan'))
```

### Comparing `goodwe-0.4.5/tests/test_es.py` & `goodwe-0.4.6/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/tests/test_et.py` & `goodwe-0.4.6/tests/test_et.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         self.assertSensor('meter_apparent_power_total', -1403, 'VA', data)
         self.assertSensor('meter_type', 1, '', data)
         self.assertSensor('meter_sw_version', 3, '', data)
 
         self.assertFalse(self.sensor_map, f"Some sensors were not tested {self.sensor_map}")
 
     def test_GW10K_ET_setting(self):
-        self.assertEqual(65, len(self.settings()))
+        self.assertEqual(66, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('Timestamp', type(settings.get("time")).__name__)
         self.assertEqual('EcoModeV1', type(settings.get("eco_mode_1")).__name__)
 
     def test_GW10K_ET_read_setting(self):
         self.loop.run_until_complete(self.read_setting('work_mode'))
         self.assertEqual('f703b798000136c7', self.request.hex())
@@ -334,15 +334,15 @@
         self.assertEqual(159, self.dsp_svn_version)
         self.assertEqual(19, self.arm_version)
         self.assertEqual(207, self.arm_svn_version)
         self.assertEqual('04029-08-S11', self.firmware)
         self.assertEqual('02041-19-S00', self.arm_firmware)
 
     def test_GW10K_ET_settings_fw819(self):
-        self.assertEqual(72, len(self.settings()))
+        self.assertEqual(73, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('EcoModeV2', type(settings.get("eco_mode_1")).__name__)
         self.assertEqual(None, settings.get("peak_shaving_mode"))
 
     def test_set_operation_mode_ECO_CHARGE(self):
         self.loop.run_until_complete(
             self.set_operation_mode(OperationMode.ECO_CHARGE, eco_mode_power=40, eco_mode_soc=80))
@@ -375,15 +375,15 @@
         self.assertEqual(167, self.dsp_svn_version)
         self.assertEqual(23, self.arm_version)
         self.assertEqual(237, self.arm_svn_version)
         self.assertEqual('04029-10-S11', self.firmware)
         self.assertEqual('02041-23-S00', self.arm_firmware)
 
     def test_GW10K_ET_setting_fw1023(self):
-        self.assertEqual(80, len(self.settings()))
+        self.assertEqual(81, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('PeakShavingMode', type(settings.get("peak_shaving_mode")).__name__)
 
     def test_GW10K_ET_runtime_data_fw1023(self):
         # Reset sensors
         self.loop.run_until_complete(self.read_device_info())
         self.sensor_map = {s.id_: s.unit for s in self.sensors()}
```

### Comparing `goodwe-0.4.5/tests/test_modbus.py` & `goodwe-0.4.6/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/tests/test_protocol.py` & `goodwe-0.4.6/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.5/tests/test_sensor.py` & `goodwe-0.4.6/tests/test_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,103 +26,117 @@
     def test_byteH(self):
         testee = ByteH("", 0, "", "", None)
 
         data = MockResponse("2039")
         self.assertEqual(32, testee.read(data))
 
         self.assertEqual("2039", testee.encode_value(32, bytes.fromhex("3039")).hex())
+        self.assertEqual("2039", testee.encode_value("32", bytes.fromhex("3039")).hex())
         self.assertEqual("ff39", testee.encode_value(-1, bytes.fromhex("3039")).hex())
         self.assertEqual("7f39", testee.encode_value(127, bytes.fromhex("3039")).hex())
         self.assertEqual("20ff", testee.encode_value(32, bytes.fromhex("ffff")).hex())
 
     def test_byteL(self):
         testee = ByteL("", 0, "", "", None)
 
         data = MockResponse("307f")
         self.assertEqual(127, testee.read(data))
 
         self.assertEqual("3020", testee.encode_value(32, bytes.fromhex("3039")).hex())
+        self.assertEqual("3020", testee.encode_value("32", bytes.fromhex("3039")).hex())
         self.assertEqual("30ff", testee.encode_value(-1, bytes.fromhex("3039")).hex())
         self.assertEqual("307f", testee.encode_value(127, bytes.fromhex("3039")).hex())
         self.assertEqual("ff20", testee.encode_value(32, bytes.fromhex("ffff")).hex())
 
     def test_integer(self):
         testee = Integer("", 0, "", "", None)
 
         data = MockResponse("0031")
         self.assertEqual(49, testee.read(data))
         self.assertEqual("0031", testee.encode_value(49).hex())
+        self.assertEqual("0031", testee.encode_value("49").hex())
 
         data = MockResponse("ff9e")
         self.assertEqual(65438, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(65438).hex())
+        self.assertEqual("ff9e", testee.encode_value("65438").hex())
 
     def test_integer_signed(self):
         testee = IntegerS("", 0, "", "", None)
 
         data = MockResponse("0031")
         self.assertEqual(49, testee.read(data))
         self.assertEqual("0031", testee.encode_value(49).hex())
+        self.assertEqual("0031", testee.encode_value("49").hex())
 
         data = MockResponse("ff9e")
         self.assertEqual(-98, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(-98).hex())
+        self.assertEqual("ff9e", testee.encode_value("-98").hex())
 
     def test_decimal(self):
         testee = Decimal("", 0, 10, "", "", None)
 
         data = MockResponse("0031")
         self.assertEqual(4.9, testee.read(data))
         self.assertEqual("0031", testee.encode_value(4.9).hex())
+        self.assertEqual("0031", testee.encode_value("4.9").hex())
 
         data = MockResponse("ff9e")
         self.assertEqual(-9.8, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(-9.8).hex())
+        self.assertEqual("ff9e", testee.encode_value("-9.8").hex())
 
     def test_voltage(self):
         testee = Voltage("", 0, "", None)
 
         data = MockResponse("0cfe")
         self.assertEqual(332.6, testee.read(data))
         self.assertEqual("0cfe", testee.encode_value(332.6).hex())
+        self.assertEqual("0cfe", testee.encode_value("332.6").hex())
 
         data = MockResponse("1f64")
         self.assertEqual(803.6, testee.read(data))
         self.assertEqual("1f64", testee.encode_value(803.6).hex())
+        self.assertEqual("1f64", testee.encode_value("803.6").hex())
 
         data = MockResponse("a000")
         self.assertEqual(4096.0, testee.read(data))
 
         data = MockResponse("ffff")
         self.assertEqual(0, testee.read(data))
 
     def test_current(self):
         testee = Current("", 0, "", None)
 
         data = MockResponse("0031")
         self.assertEqual(4.9, testee.read(data))
         self.assertEqual("0031", testee.encode_value(4.9).hex())
+        self.assertEqual("0031", testee.encode_value("4.9").hex())
 
         data = MockResponse("ff9e")
         self.assertEqual(6543.8, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(6543.8).hex())
+        self.assertEqual("ff9e", testee.encode_value("6543.8").hex())
 
         data = MockResponse("ffff")
         self.assertEqual(0, testee.read(data))
 
     def test_current_signed(self):
         testee = CurrentS("", 0, "", None)
 
         data = MockResponse("0031")
         self.assertEqual(4.9, testee.read(data))
         self.assertEqual("0031", testee.encode_value(4.9).hex())
+        self.assertEqual("0031", testee.encode_value("4.9").hex())
 
         data = MockResponse("ff9e")
         self.assertEqual(-9.8, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(-9.8).hex())
+        self.assertEqual("ff9e", testee.encode_value("-9.8").hex())
 
     def test_power4(self):
         testee = Power4("", 0, "", None)
 
         data = MockResponse("0000069f")
         self.assertEqual(1695, testee.read(data))
```

