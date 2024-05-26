# Comparing `tmp/tmc_2209_raspberry_pi-0.4.5.tar.gz` & `tmp/tmc_2209_raspberry_pi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmc_2209_raspberry_pi-0.4.5.tar", last modified: Wed Apr 17 16:57:40 2024, max compression
+gzip compressed data, was "tmc_2209_raspberry_pi-0.5.tar", last modified: Sun May 26 10:25:47 2024, max compression
```

## Comparing `tmc_2209_raspberry_pi-0.4.5.tar` & `tmc_2209_raspberry_pi-0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.127421 tmc_2209_raspberry_pi-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.131421 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/
--rw-r--r--   0 runner    (1001) docker     (127)    19929 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/TMC_2209_StepperDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_GPIO_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_uart.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 16:57:40.000000 tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:57:40.135421 tmc_2209_raspberry_pi-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 16:57:36.000000 tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:25:47.612242 tmc_2209_raspberry_pi-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35305 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-26 10:25:47.612242 tmc_2209_raspberry_pi-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 10:25:47.612242 tmc_2209_raspberry_pi-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:25:47.604242 tmc_2209_raspberry_pi-0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:25:47.608242 tmc_2209_raspberry_pi-0.5/src/TMC_2209/
+-rw-r--r--   0 runner    (1001) docker     (127)    20022 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/TMC_2209_StepperDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_GPIO_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_uart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:25:47.608242 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-26 10:25:47.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-26 10:25:47.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:25:47.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 10:25:47.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 10:25:47.000000 tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:25:47.608242 tmc_2209_raspberry_pi-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 10:25:43.000000 tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_uart.py
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/LICENSE` & `tmc_2209_raspberry_pi-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/PKG-INFO` & `tmc_2209_raspberry_pi-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.5
+Version: 0.5
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,16 +12,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: RPi.GPIO
 Requires-Dist: pyserial
+Provides-Extra: raspberry-pi
+Requires-Dist: RPi.GPIO; extra == "raspberry-pi"
+Provides-Extra: raspberry-pi5
+Requires-Dist: gpiozero; extra == "raspberry-pi5"
+Provides-Extra: nvidia-jetson
+Requires-Dist: Jetson.GPIO; extra == "nvidia-jetson"
+Provides-Extra: luckfox-pico
+Requires-Dist: python-periphery; extra == "luckfox-pico"
 
 # TMC_2209_Raspberry_Pi
 
 [![PyPI python version TMC-2209-Raspberry-Pi](https://badgen.net/pypi/python/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![PyPI version TMC-2209-Raspberry-Pi](https://badgen.net/pypi/v/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![PyPI downloads TMC-2209-Raspberry-Pi](https://img.shields.io/pypi/dm/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![GitHub issues](https://img.shields.io/github/issues/Chr157i4n/TMC2209_Raspberry_Pi.svg)](https://GitHub.com/Chr157i4n/TMC2209_Raspberry_Pi/issues/)
@@ -31,15 +38,15 @@
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
 So if you move the motor with high speed using this library the motor will lose steps.
 
-My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
+Tested on a [Bigtreetech TMC2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.2) and [Bigtreetech TMC2209 V1.3](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.3).
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
@@ -73,14 +80,32 @@
 
 - enable the serial port in
 
     ```shell
     sudo raspi-config
     ```
 
+### Board Support
+
+The following table shows the supported boards and which libraries for GPIO access is beeing used for that board.
+
+Library | Installation Parameter | Boards
+-- | -- | --
+RPi.GPIO | RASPBERRY_PI | Pi4, Pi3 etc.
+gpiozero | RASPBERRY_PI5 | Pi5
+Jetson.GPIO | NVIDIA_JETSON | Nvidia Jetson
+pheriphery | LUCKFOX_PICO | Luckfox Pico
+
+Those libraries are needed for this library to work. You can either install the correct library yourself.
+You can also install the needed GPIO library by specifing the Installation Parameter while installing this library:
+
+```shell
+pip3 install TMC-2209-Raspberry-Pi[RASPBERRY_PI]
+```
+
 ## Wiring
 
 Pin TMC2209 | connect to | Function
 -- | -- | --
 TX or PDN_UART with 1kOhm | TX of Raspberry Pi | send data to TMC via UART
 RX or PDN_UART directly | RX of Raspberry Pi | receive data from TMC via UART
 VDD | 3,3V of Raspberry Pi | optional, for more stable logic voltage
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/README.md` & `tmc_2209_raspberry_pi-0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
 So if you move the motor with high speed using this library the motor will lose steps.
 
-My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
+Tested on a [Bigtreetech TMC2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.2) and [Bigtreetech TMC2209 V1.3](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.3).
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
@@ -52,14 +52,32 @@
 
 - enable the serial port in
 
     ```shell
     sudo raspi-config
     ```
 
+### Board Support
+
+The following table shows the supported boards and which libraries for GPIO access is beeing used for that board.
+
+Library | Installation Parameter | Boards
+-- | -- | --
+RPi.GPIO | RASPBERRY_PI | Pi4, Pi3 etc.
+gpiozero | RASPBERRY_PI5 | Pi5
+Jetson.GPIO | NVIDIA_JETSON | Nvidia Jetson
+pheriphery | LUCKFOX_PICO | Luckfox Pico
+
+Those libraries are needed for this library to work. You can either install the correct library yourself.
+You can also install the needed GPIO library by specifing the Installation Parameter while installing this library:
+
+```shell
+pip3 install TMC-2209-Raspberry-Pi[RASPBERRY_PI]
+```
+
 ## Wiring
 
 Pin TMC2209 | connect to | Function
 -- | -- | --
 TX or PDN_UART with 1kOhm | TX of Raspberry Pi | send data to TMC via UART
 RX or PDN_UART directly | RX of Raspberry Pi | receive data from TMC via UART
 VDD | 3,3V of Raspberry Pi | optional, for more stable logic voltage
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/setup.cfg` & `tmc_2209_raspberry_pi-0.5/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TMC_2209_Raspberry_Pi
-version = 0.4.5
+version = 0.5
 author = Christian Köhlke
 author_email = christian@koehlke.de
 description = this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 project_urls = 
@@ -20,17 +20,26 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	RPi.GPIO
 	pyserial
 
 [options.packages.find]
 where = src
 
+[options.extras_require]
+RASPBERRY_PI = 
+	RPi.GPIO
+RASPBERRY_PI5 = 
+	gpiozero
+NVIDIA_JETSON = 
+	Jetson.GPIO
+LUCKFOX_PICO = 
+	python-periphery
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/TMC_2209_StepperDriver.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/TMC_2209_StepperDriver.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 1. change setting in the TMC-driver via UART
 2. move the motor via STEP/DIR pins
 """
 
 import time
 import statistics
 import logging
-from ._TMC_2209_GPIO_board import GPIO, BOARD
+from ._TMC_2209_GPIO_board import TMC_gpio, Gpio, GpioMode, GpioPUD, BOARD
 from ._TMC_2209_uart import TMC_UART as tmc_uart
 from ._TMC_2209_logger import TMC_logger, Loglevel
 from ._TMC_2209_move import MovementAbsRel, MovementPhase, StopMode
 from . import _TMC_2209_math as tmc_math
 
 
 
@@ -97,27 +97,27 @@
     _movement_thread = None
 
     _deinit_finished = False
 
 
 
     def __init__(self, pin_en, pin_step=-1, pin_dir=-1, baudrate=115200, serialport="/dev/serial0",
-                 driver_address=0, gpio_mode=GPIO.BCM, loglevel=None, logprefix=None,
+                 driver_address=0, gpio_mode=None, loglevel=None, logprefix=None,
                  log_handlers: list = None, log_formatter : logging.Formatter = None,
                  skip_uart_init: bool = False):
         """constructor
 
         Args:
             pin_en (int): EN pin number
             pin_step (int, optional): STEP pin number. Defaults to -1.
             pin_dir (int, optional): DIR pin number. Defaults to -1.
             baudrate (int, optional): baudrate. Defaults to 115200.
             serialport (str, optional): serialport path. Defaults to "/dev/serial0".
-            driver_address (int, optional): driver adress [0-3]. Defaults to 0.
-            gpio_mode (enum, optional): gpio mode. Defaults to GPIO.BCM.
+            driver_address (int, optional): driver address [0-3]. Defaults to 0.
+            gpio_mode (enum, optional): gpio mode. Defaults to None.
             loglevel (enum, optional): loglevel. Defaults to None.
             logprefix (str, optional): log prefix (name of the logger).
                 Defaults to None (standard TMC prefix).
             log_handlers (list, optional): list of logging handlers.
                 Defaults to None (log to console).
             log_formatter (logging.Formatter, optional): formatter for the log messages.
                 Defaults to None (messages are logged in the format
@@ -127,30 +127,29 @@
         if logprefix is None:
             logprefix = f"TMC2209 {driver_address}"
         self.tmc_logger = TMC_logger(loglevel, logprefix, log_handlers, log_formatter)
         self.tmc_uart = tmc_uart(self.tmc_logger, serialport, baudrate, driver_address)
 
 
         self.tmc_logger.log("Init", Loglevel.INFO)
-        GPIO.setwarnings(False)
-        GPIO.setmode(gpio_mode)
+        TMC_gpio.init(gpio_mode)
 
         self.tmc_logger.log(f"EN Pin: {pin_en}", Loglevel.DEBUG)
         self._pin_en = pin_en
-        GPIO.setup(self._pin_en, GPIO.OUT, initial=GPIO.HIGH)
+        TMC_gpio.gpio_setup(self._pin_en, GpioMode.OUT, initial=Gpio.HIGH)
 
         self.tmc_logger.log(f"STEP Pin: {pin_step}", Loglevel.DEBUG)
         if pin_step != -1:
             self._pin_step = pin_step
-            GPIO.setup(self._pin_step, GPIO.OUT, initial=GPIO.LOW)
+            TMC_gpio.gpio_setup(self._pin_step, GpioMode.OUT, initial=Gpio.LOW)
 
         self.tmc_logger.log(f"DIR Pin: {pin_dir}", Loglevel.DEBUG)
         if pin_dir != -1:
             self._pin_dir = pin_dir
-            GPIO.setup(self._pin_dir, GPIO.OUT, initial=self._direction)
+            TMC_gpio.gpio_setup(self._pin_dir, GpioMode.OUT, initial=self._direction)
 
         self.tmc_logger.log("GPIO Init finished", Loglevel.INFO)
 
         if not skip_uart_init:
             self.read_steps_per_rev()
             self.clear_gstat()
 
@@ -167,22 +166,22 @@
         if self._deinit_finished is False:
             self.tmc_logger.log("Deinit", Loglevel.INFO)
 
             self.set_motor_enabled(False)
 
             self.tmc_logger.log("GPIO cleanup", Loglevel.INFO)
             if self._pin_step != -1:
-                GPIO.cleanup(self._pin_step)
+                TMC_gpio.gpio_cleanup(self._pin_step)
             if self._pin_dir != -1:
-                GPIO.cleanup(self._pin_dir)
+                TMC_gpio.gpio_cleanup(self._pin_dir)
             if self._pin_en != -1:
-                GPIO.cleanup(self._pin_en)
+                TMC_gpio.gpio_cleanup(self._pin_en)
             if self._pin_stallguard != -1:
-                GPIO.remove_event_detect(self._pin_stallguard)
-                GPIO.cleanup(self._pin_stallguard)
+                TMC_gpio.gpio_remove_event_detect(self._pin_stallguard)
+                TMC_gpio.gpio_cleanup(self._pin_stallguard)
 
             self.tmc_logger.log("Deinit finished", Loglevel.INFO)
             self._deinit_finished= True
         else:
             self.tmc_logger.log("Deinit already finished", Loglevel.INFO)
         del self.tmc_uart
         del self.tmc_logger
@@ -197,15 +196,15 @@
 
     def set_motor_enabled(self, en):
         """enables or disables the motor current output
 
         Args:
             en (bool): whether the motor current output should be enabled
         """
-        GPIO.output(self._pin_en, not en)
+        TMC_gpio.gpio_output(self._pin_en, not en)
         self.tmc_logger.log(f"Motor output active: {en}", Loglevel.INFO)
 
 
 
     def do_homing(self, diag_pin, revolutions = 10, threshold = None, speed_rpm = None):
         """homes the motor in the given direction using stallguard.
         this method is using vactual to move the motor and an interrupt on the DIAG pin
@@ -312,26 +311,26 @@
         self.tmc_logger.log("---", Loglevel.INFO)
 
 
 
     def reverse_direction_pin(self):
         """reverses the motor shaft direction"""
         self._direction = not self._direction
-        GPIO.output(self._pin_dir, self._direction)
+        TMC_gpio.gpio_output(self._pin_dir, self._direction)
 
 
 
     def set_direction_pin(self, direction):
         """sets the motor shaft direction to the given value: 0 = CCW; 1 = CW
 
         Args:
             direction (bool): motor shaft direction: False = CCW; True = CW
         """
         self._direction = direction
-        GPIO.output(self._pin_dir, direction)
+        TMC_gpio.gpio_output(self._pin_dir, direction)
 
 
 
     def read_steps_per_rev(self):
         """returns how many steps are needed for one revolution.
         this reads the value from the tmc driver.
 
@@ -371,14 +370,15 @@
 
         Returns:
             stop (enum): how the movement was finished
         """
         self._stop = StopMode.NO
         current_vactual = 0
         sleeptime = 0.05
+        time_to_stop = 0
         if vactual<0:
             acceleration = -acceleration
 
         if duration != 0:
             self.tmc_logger.log(f"vactual: {vactual} for {duration} sec",
                                 Loglevel.INFO)
         else:
@@ -483,19 +483,18 @@
 
         self.set_stallguard_threshold(threshold)
         self.set_coolstep_threshold(tmc_math.steps_to_tstep(
             min_speed, self.get_microstepping_resolution()))
         self._sg_callback = callback
         self._pin_stallguard = pin_stallguard
 
-        GPIO.setup(self._pin_stallguard, GPIO.IN, pull_up_down=GPIO.PUD_DOWN)
+        TMC_gpio.gpio_setup(self._pin_stallguard, GpioMode.IN, pull_up_down=GpioPUD.PUD_DOWN)
         # first remove existing events
-        GPIO.remove_event_detect(self._pin_stallguard)
-        GPIO.add_event_detect(self._pin_stallguard, GPIO.RISING, callback=self.stallguard_callback,
-                              bouncetime=300)
+        TMC_gpio.gpio_remove_event_detect(self._pin_stallguard)
+        TMC_gpio.gpio_add_event_detect(self._pin_stallguard, self.stallguard_callback)
 
 
 
     def stallguard_callback(self, gpio_pin):
         """the callback function for StallGuard.
         only checks whether the duration of the current movement is longer than
         _sg_delay and then calls the actual callback
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_comm.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_comm.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_logger.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_logger.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_move.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 TMC_2209 stepper driver communication module
 """
 
 import time
 from enum import Enum
 import math
 import threading
-from ._TMC_2209_GPIO_board import GPIO
+from ._TMC_2209_GPIO_board import TMC_gpio, Gpio
 from ._TMC_2209_logger import Loglevel
 
 
 
 class Direction(Enum):
     """movement direction of the motor"""
     CCW = 0
@@ -41,39 +41,39 @@
     """stopmode"""
     NO = 0
     SOFTSTOP = 1
     HARDSTOP = 2
 
 
 def set_movement_abs_rel(self, movement_abs_rel):
-    """set whether the movment should be relative or absolute by default.
+    """set whether the movement should be relative or absolute by default.
     See the Enum MovementAbsoluteRelative
 
     Args:
-        movement_abs_rel (enum): whether the movment should be relative or absolute
+        movement_abs_rel (enum): whether the movement should be relative or absolute
     """
     self._movement_abs_rel = movement_abs_rel
 
 
 
 def get_current_position(self):
     """returns the current motor position in µsteps
 
     Returns:
-        bool: current motor position
+        int: current motor position
     """
     return self._current_pos
 
 
 
 def set_current_position(self, new_pos):
     """overwrites the current motor position in µsteps
 
     Args:
-        new_pos (bool): new position of the motor in µsteps
+        new_pos (int): new position of the motor in µsteps
     """
     self._current_pos = new_pos
 
 
 
 def set_max_speed(self, speed):
     """sets the maximum motor speed in µsteps per second
@@ -110,18 +110,18 @@
         int: current maximum speed in steps/sec
     """
     return self._max_speed
 
 
 
 def set_acceleration(self, acceleration):
-    """sets the motor acceleration/decceleration in µsteps per sec per sec
+    """sets the motor acceleration/deceleration in µsteps per sec per sec
 
     Args:
-        acceleration (int): acceleration/decceleration in µsteps per sec per sec
+        acceleration (int): acceleration/deceleration in µsteps per sec per sec
     """
     if acceleration == 0.0:
         return
     acceleration = abs(acceleration)
     if self._acceleration != acceleration:
         # Recompute _n per Equation 17
         self._n = self._n * (self._acceleration / acceleration)
@@ -129,38 +129,38 @@
         self._c0 = 0.676 * math.sqrt(2.0 / acceleration) * 1000000.0 # Equation 15
         self._acceleration = acceleration
         self.compute_new_speed()
 
 
 
 def set_acceleration_fullstep(self, acceleration):
-    """sets the motor acceleration/decceleration in fullsteps per sec per sec
+    """sets the motor acceleration/deceleration in fullsteps per sec per sec
 
     Args:
-        acceleration (int): acceleration/decceleration in fullsteps per sec per sec
+        acceleration (int): acceleration/deceleration in fullsteps per sec per sec
     """
     self.set_acceleration(acceleration*self.get_microstepping_resolution())
 
 
 
 def get_acceleration(self):
-    """returns the motor acceleration/decceleration in steps per sec per sec
+    """returns the motor acceleration/deceleration in steps per sec per sec
 
     Returns:
-        int: acceleration/decceleration in µsteps per sec per sec
+        int: acceleration/deceleration in µsteps per sec per sec
     """
     return self._acceleration
 
 
 
 def stop(self, stop_mode = StopMode.HARDSTOP):
     """stop the current movement
 
     Args:
-        stop_mode (enum): whether the movement should be stopped immediatly or softly
+        stop_mode (enum): whether the movement should be stopped immediately or softly
             (Default value = StopMode.HARDSTOP)
     """
     self._stop = stop_mode
 
 
 
 def get_movement_phase(self):
@@ -173,15 +173,15 @@
 
 
 
 def run_to_position_steps(self, steps, movement_abs_rel = None):
     """runs the motor to the given position.
     with acceleration and deceleration
     blocks the code until finished or stopped from a different thread!
-    returns true when the movement if finshed normally and false,
+    returns true when the movement if finished normally and false,
     when the movement was stopped
 
     Args:
         steps (int): amount of steps; can be negative
         movement_abs_rel (enum): whether the movement should be absolut or relative
             (Default value = None)
 
@@ -227,15 +227,15 @@
 
 
 
 def run_to_position_steps_threaded(self, steps, movement_abs_rel = None):
     """runs the motor to the given position.
     with acceleration and deceleration
     does not block the code
-    returns true when the movement if finshed normally and false,
+    returns true when the movement if finished normally and false,
     when the movement was stopped
 
     Args:
         steps (int): amount of steps; can be negative
         movement_abs_rel (enum): whether the movement should be absolut or relative
             (Default value = None)
 
@@ -264,16 +264,16 @@
     return self.run_to_position_steps_threaded(round(revolutions * self._steps_per_rev),
                                                 movement_abs_rel)
 
 
 
 def wait_for_movement_finished_threaded(self):
     """wait for the motor to finish the movement,
-    if startet threaded
-    returns true when the movement if finshed normally and false,
+    if started threaded
+    returns true when the movement if finished normally and false,
     when the movement was stopped
 
     Returns:
         enum: how the movement was finished
     """
     self._movement_thread.join()
     return self._stop
@@ -302,15 +302,15 @@
     """returns the calculated current speed depending on the acceleration
 
     this code is based on:
     "Generate stepper-motor speed profiles in real time" by David Austin
     https://www.embedded.com/generate-stepper-motor-speed-profiles-in-real-time/
     https://web.archive.org/web/20140705143928/http://fab.cba.mit.edu/classes/MIT/961.09/projects/i0/Stepper_Motor_Speed_Profile.pdf
     """
-    distance_to = self.distance_to_go() # +ve is clockwise from curent location
+    distance_to = self.distance_to_go() # +ve is clockwise from current location
     steps_to_stop = (self._speed * self._speed) / (2.0 * self._acceleration) # Equation 16
     if ((distance_to == 0 and steps_to_stop <= 2) or
     (self._stop == StopMode.SOFTSTOP and steps_to_stop <= 1)):
         # We are at the target and its time to stop
         self._step_interval = 0
         self._speed = 0.0
         self._n = 0
@@ -326,35 +326,35 @@
             if ((steps_to_stop >= distance_to) or self._direction == Direction.CCW or
                 self._stop == StopMode.SOFTSTOP):
                 self._n = -steps_to_stop # Start deceleration
                 self._movement_phase = MovementPhase.DECELERATING
         elif self._n < 0:
             # Currently decelerating, need to accel again?
             if (steps_to_stop < distance_to) and self._direction == Direction.CW:
-                self._n = -self._n # Start accceleration
+                self._n = -self._n # Start acceleration
                 self._movement_phase = MovementPhase.ACCELERATING
     elif distance_to < 0:
         # We are clockwise from the target
         # Need to go anticlockwise from here, maybe decelerate
         if self._n > 0:
             # Currently accelerating, need to decel now? Or maybe going the wrong way?
             if (((steps_to_stop >= -distance_to) or self._direction == Direction.CW or
                 self._stop == StopMode.SOFTSTOP)):
                 self._n = -steps_to_stop # Start deceleration
                 self._movement_phase = MovementPhase.DECELERATING
         elif self._n < 0:
             # Currently decelerating, need to accel again?
             if (steps_to_stop < -distance_to) and self._direction == Direction.CCW:
-                self._n = -self._n # Start accceleration
+                self._n = -self._n # Start acceleration
                 self._movement_phase = MovementPhase.ACCELERATING
     # Need to accelerate or decelerate
     if self._n == 0:
         # First step from stopped
         self._cn = self._c0
-        GPIO.output(self._pin_step, GPIO.LOW)
+        TMC_gpio.gpio_output(self._pin_step, Gpio.LOW)
         if distance_to > 0:
             self.set_direction_pin(1)
             self.tmc_logger.log("going CW", Loglevel.MOVEMENT)
         else:
             self.set_direction_pin(0)
             self.tmc_logger.log("going CCW", Loglevel.MOVEMENT)
         self._movement_phase = MovementPhase.ACCELERATING
@@ -370,15 +370,15 @@
     if self._direction == 0:
         self._speed = -self._speed
 
 
 
 def run_speed(self):
     """this methods does the actual steps with the current speed"""
-    # Dont do anything unless we actually have a step interval
+    # Don't do anything unless we actually have a step interval
     if not self._step_interval:
         return False
 
     curtime = time.time_ns()/1000
 
     if curtime - self._last_step_time >= self._step_interval:
 
@@ -395,13 +395,13 @@
 
 
 def make_a_step(self):
     """method that makes on step
 
     for the TMC2209 there needs to be a signal duration of minimum 100 ns
     """
-    GPIO.output(self._pin_step, GPIO.HIGH)
+    TMC_gpio.gpio_output(self._pin_step, Gpio.HIGH)
     time.sleep(1/1000/1000)
-    GPIO.output(self._pin_step, GPIO.LOW)
+    TMC_gpio.gpio_output(self._pin_step, Gpio.LOW)
     time.sleep(1/1000/1000)
 
     self.tmc_logger.log("one step", Loglevel.MOVEMENT)
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_reg.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_reg.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_test.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 #pylint: disable=no-member
 #pylint: disable=bare-except
 """
 TMC_2209 stepper driver communication module
 """
 
 import time
-from ._TMC_2209_GPIO_board import GPIO
+from ._TMC_2209_GPIO_board import TMC_gpio, Gpio
 from ._TMC_2209_logger import Loglevel
 from ._TMC_2209_move import MovementAbsRel, MovementPhase
 from . import _TMC_2209_reg as tmc_reg
 
 
 
 def test_dir_step_en(self):
     """tests the EN, DIR and STEP pin
 
     this sets the EN, DIR and STEP pin to HIGH, LOW and HIGH
     and checks the IOIN Register of the TMC meanwhile
     """
     pin_dir_ok = pin_step_ok = pin_en_ok = True
 
-    GPIO.output(self._pin_step, GPIO.HIGH)
-    GPIO.output(self._pin_dir, GPIO.HIGH)
-    GPIO.output(self._pin_en, GPIO.HIGH)
+    TMC_gpio.gpio_output(self._pin_step, Gpio.HIGH)
+    TMC_gpio.gpio_output(self._pin_dir, Gpio.HIGH)
+    TMC_gpio.gpio_output(self._pin_en, Gpio.HIGH)
     time.sleep(0.1)
     ioin = self.read_ioin()
     if not ioin & tmc_reg.io_dir:
         pin_dir_ok = False
     if not ioin & tmc_reg.io_step:
         pin_step_ok = False
     if not ioin & tmc_reg.io_enn:
         pin_en_ok = False
 
-    GPIO.output(self._pin_step, GPIO.LOW)
-    GPIO.output(self._pin_dir, GPIO.LOW)
-    GPIO.output(self._pin_en, GPIO.LOW)
+    TMC_gpio.gpio_output(self._pin_step, Gpio.LOW)
+    TMC_gpio.gpio_output(self._pin_dir, Gpio.LOW)
+    TMC_gpio.gpio_output(self._pin_en, Gpio.LOW)
     time.sleep(0.1)
     ioin = self.read_ioin()
     if ioin & tmc_reg.io_dir:
         pin_dir_ok = False
     if ioin & tmc_reg.io_step:
         pin_step_ok = False
     if ioin & tmc_reg.io_enn:
         pin_en_ok = False
 
-    GPIO.output(self._pin_step, GPIO.HIGH)
-    GPIO.output(self._pin_dir, GPIO.HIGH)
-    GPIO.output(self._pin_en, GPIO.HIGH)
+    TMC_gpio.gpio_output(self._pin_step, Gpio.HIGH)
+    TMC_gpio.gpio_output(self._pin_dir, Gpio.HIGH)
+    TMC_gpio.gpio_output(self._pin_en, Gpio.HIGH)
     time.sleep(0.1)
     ioin = self.read_ioin()
     if not ioin & tmc_reg.io_dir:
         pin_dir_ok = False
     if not ioin & tmc_reg.io_step:
         pin_step_ok = False
     if not ioin & tmc_reg.io_enn:
@@ -81,17 +81,17 @@
 
 def test_step(self):
     """test method"""
     self.set_direction_pin(1)
 
     for _ in range(100):
         self._current_pos += 1
-        GPIO.output(self._pin_step, GPIO.HIGH)
+        TMC_gpio.gpio_output(self._pin_step, Gpio.HIGH)
         time.sleep(0.001)
-        GPIO.output(self._pin_step, GPIO.LOW)
+        TMC_gpio.gpio_output(self._pin_step, Gpio.LOW)
         time.sleep(0.01)
 
 
 
 def test_uart(self):
     """test method"""
     self.tmc_logger.log("---")
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209/_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209/_TMC_2209_uart.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMC_2209_Raspberry_Pi
-Version: 0.4.5
+Version: 0.5
 Summary: this is a Python libary to drive a stepper motor with a Trinamic TMC2209 stepper driver and a Raspberry Pi
 Home-page: https://github.com/Chr157i4n/TMC2209_Raspberry_Pi
 Author: Christian Köhlke
 Author-email: christian@koehlke.de
 Project-URL: Bug Tracker, https://github.com/Chr157i4n/TMC2209_Raspberry_Pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,16 +12,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: RPi.GPIO
 Requires-Dist: pyserial
+Provides-Extra: raspberry-pi
+Requires-Dist: RPi.GPIO; extra == "raspberry-pi"
+Provides-Extra: raspberry-pi5
+Requires-Dist: gpiozero; extra == "raspberry-pi5"
+Provides-Extra: nvidia-jetson
+Requires-Dist: Jetson.GPIO; extra == "nvidia-jetson"
+Provides-Extra: luckfox-pico
+Requires-Dist: python-periphery; extra == "luckfox-pico"
 
 # TMC_2209_Raspberry_Pi
 
 [![PyPI python version TMC-2209-Raspberry-Pi](https://badgen.net/pypi/python/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![PyPI version TMC-2209-Raspberry-Pi](https://badgen.net/pypi/v/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![PyPI downloads TMC-2209-Raspberry-Pi](https://img.shields.io/pypi/dm/TMC-2209-Raspberry-Pi)](https://pypi.org/project/TMC-2209-Raspberry-Pi)
 [![GitHub issues](https://img.shields.io/github/issues/Chr157i4n/TMC2209_Raspberry_Pi.svg)](https://GitHub.com/Chr157i4n/TMC2209_Raspberry_Pi/issues/)
@@ -31,15 +38,15 @@
 This is a library to drive a stepper motor with a TMC2209 stepper driver and a Raspberry Pi.
 
 This code is still experimental, so use it on your own risk.
 
 This library is programmed in pure Python. The performance of Python is not good enough to drive the motor with high speed.
 So if you move the motor with high speed using this library the motor will lose steps.
 
-My TMC2209 is a [Bigtreetech TMC 2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-TMC2209-V1.2)
+Tested on a [Bigtreetech TMC2209 V1.2](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.2) and [Bigtreetech TMC2209 V1.3](https://github.com/bigtreetech/BIGTREETECH-Stepper-Motor-Driver/tree/master/TMC2209/V1.3).
 
 It has a rSense of 110 mOhm and it uses one Pin (PDN_UART) for UART RX and TX.
 So the PD_UART-Pin needs to be connected to the Raspberrry Pis RX-Pin directly and to the TX-Pin with an 1kOhm resistor.
 You can read more about this in the datasheet from Trinamic.
 
 Because the TMC2209 uses one shared pin for transmit and receive in the UART communication line, the Raspberry Pi also receives what it sends.
 Well, the Pi receives 4 bytes from itself and 8 bytes from the driver. So the Pi receives a total of 12 bytes and only the last 8 are the reply, of which only 4 are data bytes.
@@ -73,14 +80,32 @@
 
 - enable the serial port in
 
     ```shell
     sudo raspi-config
     ```
 
+### Board Support
+
+The following table shows the supported boards and which libraries for GPIO access is beeing used for that board.
+
+Library | Installation Parameter | Boards
+-- | -- | --
+RPi.GPIO | RASPBERRY_PI | Pi4, Pi3 etc.
+gpiozero | RASPBERRY_PI5 | Pi5
+Jetson.GPIO | NVIDIA_JETSON | Nvidia Jetson
+pheriphery | LUCKFOX_PICO | Luckfox Pico
+
+Those libraries are needed for this library to work. You can either install the correct library yourself.
+You can also install the needed GPIO library by specifing the Installation Parameter while installing this library:
+
+```shell
+pip3 install TMC-2209-Raspberry-Pi[RASPBERRY_PI]
+```
+
 ## Wiring
 
 Pin TMC2209 | connect to | Function
 -- | -- | --
 TX or PDN_UART with 1kOhm | TX of Raspberry Pi | send data to TMC via UART
 RX or PDN_UART directly | RX of Raspberry Pi | receive data from TMC via UART
 VDD | 3,3V of Raspberry Pi | optional, for more stable logic voltage
```

### Comparing `tmc_2209_raspberry_pi-0.4.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt` & `tmc_2209_raspberry_pi-0.5/src/TMC_2209_Raspberry_Pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_math.py` & `tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_math.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_move.py` & `tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_move.py`

 * *Files identical despite different names*

### Comparing `tmc_2209_raspberry_pi-0.4.5/tests/test_TMC_2209_uart.py` & `tmc_2209_raspberry_pi-0.5/tests/test_TMC_2209_uart.py`

 * *Files identical despite different names*

