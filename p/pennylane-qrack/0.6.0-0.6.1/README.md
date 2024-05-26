# Comparing `tmp/pennylane_qrack-0.6.0.tar.gz` & `tmp/pennylane_qrack-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane_qrack-0.6.0.tar", last modified: Sat May 25 18:21:06 2024, max compression
+gzip compressed data, was "pennylane_qrack-0.6.1.tar", last modified: Sun May 26 15:09:40 2024, max compression
```

## Comparing `pennylane_qrack-0.6.0.tar` & `pennylane_qrack-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-25 18:21:06.262899 pennylane_qrack-0.6.0/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       18 2024-05-25 18:20:55.000000 pennylane_qrack-0.6.0/MANIFEST.in
--rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-25 18:21:06.262899 pennylane_qrack-0.6.0/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3364 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/README.rst
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-25 18:21:06.261899 pennylane_qrack-0.6.0/pennylane_qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-25 13:36:03.000000 pennylane_qrack-0.6.0/pennylane_qrack/QrackDeviceConfig.toml
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/pennylane_qrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-24 10:23:28.000000 pennylane_qrack-0.6.0/pennylane_qrack/_version.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    22154 2024-05-24 10:23:28.000000 pennylane_qrack-0.6.0/pennylane_qrack/qrack_device.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-25 18:21:06.262899 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/
--rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      468 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/entry_points.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       64 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2024-05-25 18:21:06.000000 pennylane_qrack-0.6.0/pennylane_qrack.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-05-25 18:21:06.262899 pennylane_qrack-0.6.0/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2401 2024-05-25 17:54:38.000000 pennylane_qrack-0.6.0/setup.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-25 18:21:06.262899 pennylane_qrack-0.6.0/tests/
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)    17655 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/tests/test_apply.py
--rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1715 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/tests/test_integration.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     3783 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.0/tests/test_units.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.465235 pennylane_qrack-0.6.1/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       18 2024-05-25 18:20:55.000000 pennylane_qrack-0.6.1/MANIFEST.in
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-26 15:09:40.465235 pennylane_qrack-0.6.1/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3364 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/README.rst
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.460235 pennylane_qrack-0.6.1/_skbuild/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.461235 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.461235 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.463235 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-26 15:09:30.000000 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/QrackDeviceConfig.toml
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-26 15:09:30.000000 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-26 15:09:30.000000 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/_version.py
+-rw-r--r--   0 iamu      (1000) iamu      (1000)  4159848 2024-05-26 15:06:57.000000 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/libqrack_device.so
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    22662 2024-05-26 15:09:30.000000 pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.464235 pennylane_qrack-0.6.1/pennylane_qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     6144 2024-05-25 13:36:03.000000 pennylane_qrack-0.6.1/pennylane_qrack/QrackDeviceConfig.toml
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      657 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/pennylane_qrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      691 2024-05-26 15:07:24.000000 pennylane_qrack-0.6.1/pennylane_qrack/_version.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    22662 2024-05-26 14:30:40.000000 pennylane_qrack-0.6.1/pennylane_qrack/qrack_device.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.465235 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/
+-rw-r--r--   0 iamu      (1000) iamu      (1000)     4563 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      835 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       79 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/entry_points.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       64 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       16 2024-05-26 15:09:40.000000 pennylane_qrack-0.6.1/pennylane_qrack.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2024-05-26 15:09:40.465235 pennylane_qrack-0.6.1/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2401 2024-05-25 17:54:38.000000 pennylane_qrack-0.6.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2024-05-26 15:09:40.465235 pennylane_qrack-0.6.1/tests/
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)    17655 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/tests/test_apply.py
+-rwxrwxr-x   0 iamu      (1000) iamu      (1000)     1715 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/tests/test_integration.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     3783 2024-05-23 14:13:50.000000 pennylane_qrack-0.6.1/tests/test_units.py
```

### Comparing `pennylane_qrack-0.6.0/LICENSE` & `pennylane_qrack-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/PKG-INFO` & `pennylane_qrack-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.6.0
+Version: 0.6.1
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pennylane_qrack-0.6.0/README.rst` & `pennylane_qrack-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/pennylane_qrack/QrackDeviceConfig.toml` & `pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/QrackDeviceConfig.toml`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/pennylane_qrack/__init__.py` & `pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/pennylane_qrack/_version.py` & `pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `pennylane_qrack-0.6.0/pennylane_qrack/qrack_device.py` & `pennylane_qrack-0.6.1/_skbuild/linux-x86_64-3.12/cmake-install/pennylane_qrack/qrack_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
             for q in device_wires:
                 self._state.mcr(Pauli.PauliZ, par[0], control_wires, q)
 
         # translate op wire labels to consecutive wire labels used by the device
         device_wires = self.map_wires((op.control_wires + op.wires) if op.control_wires else op.wires)
         par = op.parameters
 
-        if opname in [''.join(p) for p in product(["Toffoli", "C(Toffoli)", "CNOT", "C(CNOT)", "MultiControlledX", "C(PauliX)"], ["", ".inv"])]:
+        if opname in [''.join(p) for p in it.product(["Toffoli", "C(Toffoli)", "CNOT", "C(CNOT)", "MultiControlledX", "C(PauliX)"], ["", ".inv"])]:
             self._state.mcx(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(PauliY)", "C(PauliY).inv"]:
             self._state.mcy(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(PauliZ)", "C(PauliZ).inv"]:
             self._state.mcz(device_wires.labels[:-1], device_wires.labels[-1])
         elif opname in ["C(Hadamard)", "C(Hadamard).inv"]:
             self._state.mch(device_wires.labels[:-1], device_wires.labels[-1])
@@ -416,14 +416,22 @@
             self._state.mcmtrx(device_wires.labels[:-1], [1, cmath.exp(1j * par[1]), cmath.exp(1j * par[0]), cmath.exp(1j * (par[0] + par[1]))], device_wires.labels[-1])
         elif opname == "C(U2).inv":
             self._state.mcmtrx(device_wires.labels[:-1], [1, cmath.exp(1j * -par[1]), cmath.exp(1j * -par[0]), cmath.exp(1j * (-par[0] - par[1]))], device_wires.labels[-1])
         elif opname == "U3":
             self._state.u(device_wires.labels[-1], par[0], par[1], par[2])
         elif opname == "U3.inv":
             self._state.u(device_wires.labels[-1], -par[0], -par[1], -par[2])
+        elif opname == "Rot":
+            self._state.r(Pauli.PauliZ, par[0], device_wires.labels[-1])
+            self._state.r(Pauli.PauliY, par[1], device_wires.labels[-1])
+            self._state.r(Pauli.PauliZ, par[2], device_wires.labels[-1])
+        elif opname == "Rot.inv":
+            self._state.r(Pauli.PauliZ, -par[2], device_wires.labels[-1])
+            self._state.r(Pauli.PauliY, -par[1], device_wires.labels[-1])
+            self._state.r(Pauli.PauliZ, -par[0], device_wires.labels[-1])
         elif opname == "C(U3)":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], par[0], par[1], par[2])
         elif opname == "C(U3).inv":
             self._state.mcu(device_wires.labels[:-1], device_wires.labels[-1], -par[0], -par[1], -par[2])
         elif opname == "QFT":
             self._state.qft(device_wires.labels)
             for i in range(len(wires) >> 1):
```

### Comparing `pennylane_qrack-0.6.0/pennylane_qrack.egg-info/PKG-INFO` & `pennylane_qrack-0.6.1/pennylane_qrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-qrack
-Version: 0.6.0
+Version: 0.6.1
 Summary: PennyLane plugin for Qrack.
 Home-page: http://github.com/vm6502q
 Maintainer: vm6502q
 Maintainer-email: stranoj@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pennylane_qrack-0.6.0/setup.py` & `pennylane_qrack-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/tests/test_apply.py` & `pennylane_qrack-0.6.1/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/tests/test_integration.py` & `pennylane_qrack-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pennylane_qrack-0.6.0/tests/test_units.py` & `pennylane_qrack-0.6.1/tests/test_units.py`

 * *Files identical despite different names*

