# Comparing `tmp/z_units-0.1.5.tar.gz` & `tmp/z_units-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z_units-0.1.5.tar", last modified: Thu Mar  7 14:59:20 2024, max compression
+gzip compressed data, was "z_units-0.1.6.tar", last modified: Sun May 26 14:40:00 2024, max compression
```

## Comparing `z_units-0.1.5.tar` & `z_units-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.5/LICENSE
--rw-r--r--   0        0        0     2230 2023-08-06 13:06:52.210501 z_units-0.1.5/README.md
--rw-r--r--   0        0        0      480 2024-03-07 14:59:20.232331 z_units-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.5/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.5/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.5/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2024-02-28 16:19:08.866264 z_units-0.1.5/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1427 2024-02-29 15:39:09.222012 z_units-0.1.5/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-02-29 15:39:09.222514 z_units-0.1.5/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-02-29 15:39:08.927430 z_units-0.1.5/tests/test_nonlinear_convertion.py
--rw-r--r--   0        0        0    19712 2024-02-28 16:19:08.561210 z_units-0.1.5/tests/test_quantity.py
--rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.5/tests/test_unit.py
--rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.5/z_units/__init__.py
--rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.5/z_units/config.py
--rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.5/z_units/constant.py
--rw-r--r--   0        0        0     4305 2024-02-27 15:34:48.026430 z_units-0.1.5/z_units/quantity.py
--rw-r--r--   0        0        0    24085 2024-02-28 16:15:26.023923 z_units-0.1.5/z_units/unit.py
--rw-r--r--   0        0        0     9490 2024-02-28 16:04:55.908646 z_units-0.1.5/z_units/unit_registry.py
--rw-r--r--   0        0        0     1102 2024-02-27 15:34:48.026430 z_units-0.1.5/z_units/util.py
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 z_units-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2228 2024-05-26 13:57:35.549761 z_units-0.1.6/README.md
+-rw-r--r--   0        0        0      480 2024-05-26 14:40:00.794226 z_units-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.6/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.6/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.6/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2024-05-26 14:15:57.128043 z_units-0.1.6/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1427 2024-05-26 14:15:57.128043 z_units-0.1.6/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-05-26 14:15:57.128043 z_units-0.1.6/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-26 14:15:56.911766 z_units-0.1.6/tests/test_nonlinear_convertion.py
+-rw-r--r--   0        0        0    19710 2024-05-26 14:15:39.654279 z_units-0.1.6/tests/test_quantity.py
+-rw-r--r--   0        0        0      475 2024-05-26 14:15:20.920988 z_units-0.1.6/tests/test_unit.py
+-rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.6/zunits/__init__.py
+-rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.6/zunits/config.py
+-rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.6/zunits/constant.py
+-rw-r--r--   0        0        0     4305 2024-02-27 15:34:48.026430 z_units-0.1.6/zunits/quantity.py
+-rw-r--r--   0        0        0    24085 2024-02-28 16:15:26.023923 z_units-0.1.6/zunits/unit.py
+-rw-r--r--   0        0        0     9490 2024-02-28 16:04:55.908646 z_units-0.1.6/zunits/unit_registry.py
+-rw-r--r--   0        0        0     1102 2024-02-27 15:34:48.026430 z_units-0.1.6/zunits/util.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 z_units-0.1.6/PKG-INFO
```

### Comparing `z_units-0.1.5/LICENSE` & `z_units-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/README.md` & `z_units-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ```shell
 pip install z-units
 ```
 
 ## Quickstart
 
 ```python
->>> from z_units import quantity as q
+>>> from zunits import quantity as q
 >>> f = q.MolarFlow(3)
 >>> f
 <MolarFlow(3, 'kmol/s')>
 f.value, f.unit
 (3, <Unit('kmol/s')>)
 >>> f.to('kmol/h')
 <MolarFlow(10800.0, 'kmol/h')>
@@ -28,15 +28,15 @@
 True
 >>> q.Pressure(15, 'psi').to('MPag')
 <Pressure(0.0020963594, 'MPag')>
 ```
 Related to gauge pressure, local atmospheric pressure (default: 101325 Pa) can be altered:
 
 ```python
->>> from z_units import config
+>>> from zunits import config
 # Before
 >>> q.Pressure(100, 'kPa').to('kPag')
 <Pressure(-1.325, 'kPag')>
 # Set to 50e3 Pa (50 kPa)
 >>> config.set_local_atmospheric_pressure(50e3)
 # After
 >>> q.Pressure(100, 'kPa').to('kPag')
```

### Comparing `z_units-0.1.5/tests/.pytest_cache/v/cache/nodeids` & `z_units-0.1.6/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/tests/test_quantity.py` & `z_units-0.1.6/tests/test_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from math import isclose
 
-from z_units import quantity as q
-from z_units.config import set_local_atmospheric_pressure, set_standard_temperature, get_standard_temperature
+from zunits import quantity as q
+from zunits.config import set_local_atmospheric_pressure, set_standard_temperature, get_standard_temperature
 
 
 def test_length():
     x = q.Length(1)
     assert x.unit.symbol == 'm'
     assert x.unit == x.base_unit
     assert f'{x:u}' == '1 m'
```

### Comparing `z_units-0.1.5/z_units/config.py` & `z_units-0.1.6/zunits/config.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/z_units/quantity.py` & `z_units-0.1.6/zunits/quantity.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/z_units/unit.py` & `z_units-0.1.6/zunits/unit.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/z_units/unit_registry.py` & `z_units-0.1.6/zunits/unit_registry.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/z_units/util.py` & `z_units-0.1.6/zunits/util.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.5/PKG-INFO` & `z_units-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z-units
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple unit converter for chemical engineers
 Author-Email: zenius <zenius@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zxzenius/z-units
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -22,15 +22,15 @@
 ```shell
 pip install z-units
 ```
 
 ## Quickstart
 
 ```python
->>> from z_units import quantity as q
+>>> from zunits import quantity as q
 >>> f = q.MolarFlow(3)
 >>> f
 <MolarFlow(3, 'kmol/s')>
 f.value, f.unit
 (3, <Unit('kmol/s')>)
 >>> f.to('kmol/h')
 <MolarFlow(10800.0, 'kmol/h')>
@@ -38,15 +38,15 @@
 True
 >>> q.Pressure(15, 'psi').to('MPag')
 <Pressure(0.0020963594, 'MPag')>
 ```
 Related to gauge pressure, local atmospheric pressure (default: 101325 Pa) can be altered:
 
 ```python
->>> from z_units import config
+>>> from zunits import config
 # Before
 >>> q.Pressure(100, 'kPa').to('kPag')
 <Pressure(-1.325, 'kPag')>
 # Set to 50e3 Pa (50 kPa)
 >>> config.set_local_atmospheric_pressure(50e3)
 # After
 >>> q.Pressure(100, 'kPa').to('kPag')
```

