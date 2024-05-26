# Comparing `tmp/tgqSim-0.3.0.tar.gz` & `tmp/tgqSim-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.3.0.tar", last modified: Sat May 25 08:21:31 2024, max compression
+gzip compressed data, was "tgqSim-0.3.1.tar", last modified: Sat May 25 08:47:30 2024, max compression
```

## Comparing `tgqSim-0.3.0.tar` & `tgqSim-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.540982 tgqSim-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-25 08:21:29.000000 tgqSim-0.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-25 08:21:29.000000 tgqSim-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-25 08:21:31.540982 tgqSim-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-25 08:21:29.000000 tgqSim-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 08:21:31.540982 tgqSim-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-25 08:21:30.000000 tgqSim-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.539982 tgqSim-0.3.0/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.540982 tgqSim-0.3.0/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24053 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-25 08:21:30.000000 tgqSim-0.3.0/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.540982 tgqSim-0.3.0/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    66824 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    78328 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.540982 tgqSim-0.3.0/tgqSim/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-25 08:21:29.000000 tgqSim-0.3.0/tgqSim/utils/dev_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:21:31.539982 tgqSim-0.3.0/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-25 08:21:31.000000 tgqSim-0.3.0/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-25 08:21:31.000000 tgqSim-0.3.0/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 08:21:31.000000 tgqSim-0.3.0/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-25 08:21:31.000000 tgqSim-0.3.0/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-25 08:21:31.000000 tgqSim-0.3.0/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.446931 tgqSim-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-25 08:47:28.000000 tgqSim-0.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-25 08:47:28.000000 tgqSim-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-25 08:47:30.446931 tgqSim-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-25 08:47:28.000000 tgqSim-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 08:47:30.446931 tgqSim-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-25 08:47:29.000000 tgqSim-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.445931 tgqSim-0.3.1/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.446931 tgqSim-0.3.1/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24042 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-25 08:47:29.000000 tgqSim-0.3.1/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.446931 tgqSim-0.3.1/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    66824 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    78328 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.446931 tgqSim-0.3.1/tgqSim/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-25 08:47:28.000000 tgqSim-0.3.1/tgqSim/utils/dev_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:47:30.445931 tgqSim-0.3.1/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-25 08:47:30.000000 tgqSim-0.3.1/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-25 08:47:30.000000 tgqSim-0.3.1/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 08:47:30.000000 tgqSim-0.3.1/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-25 08:47:30.000000 tgqSim-0.3.1/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-25 08:47:30.000000 tgqSim-0.3.1/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.3.0/LICENSE` & `tgqSim-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/PKG-INFO` & `tgqSim-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.3.0
+Version: 0.3.1
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.3.0/setup.py` & `tgqSim-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.3.0',
+    version='0.3.1',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.3.0/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.3.1/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.3.1/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.3.1/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/QuantumCircuit.py` & `tgqSim-0.3.1/tgqSim/QuantumCircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         cuda_version = dev_tools.get_cuda_version().replace(".", "-")
         lib_name = f"cuda_{cuda_version}_tgq_simulator.so"
         current_file_path = os.path.abspath(__file__)
         current_directory = os.path.dirname(current_file_path)
         dll_path = os.path.abspath(current_directory + '/lib/' + lib_name)
         lib = ctypes.CDLL(dll_path)
         lib.execute_circuit.argtypes = [
-            np.ctypeslib.ndpointer(ctypes.POINTER(ctypes.c_double * 2)),
+            ctypes.POINTER(ctypes.POINTER(ctypes.c_double*2)),
             ctypes.POINTER(GateInfo),
             ctypes.c_int,
             ctypes.c_int,
             ctypes.c_int
         ]
         lib.execute_circuit.restype = None
         gateInfo = []
@@ -213,17 +213,17 @@
                 gate_obj.gateName = gate_info[0].encode(encoding='utf-8')
             if len(gate_info) > 1:
                 gate_obj.theta = gate_info[1]
             gateInfo.append(gate_obj)
         gateInfoCData = (GateInfo * len(gateInfo))(*gateInfo)
         # 申请内存首地址，不在Python端申请内存
         # 在C语言中申请统一内存，减少多次拷贝动作
-        self.state = ctypes.POINTER(ctypes.c_double * 2)()
+        self.state = ctypes.POINTER(ctypes.c_double*2)()
         lib.execute_circuit(ctypes.byref(self.state), gateInfoCData, len(gateInfo), self.width, self.deviceid[0])
-        self.state = np.array(np.ctypeslib.as_array(self.state, shape=(2**self.width)), dtype=np.complex128)
+        self.state = np.array(np.ctypeslib.as_array(self.state, shape=(2**self.width,)), dtype=np.complex128)
     def run_with_noise(self, shots:int=1000):
         noise_type = ["bit_flip", "asymmetric_depolarization", "depolarize", "phase_flip", "phase_damp", "amplitude_damp"]
         result_dict = {}
         tmp_circuit = self.gate_list
         for _ in range(shots):
             new_circuit = []
             for (gate_pos, gate_info) in self.noise_circuit:
```

### Comparing `tgqSim-0.3.0/tgqSim/draw_circuit_tools.py` & `tgqSim-0.3.1/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.3.1/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.3.1/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim/utils/dev_tools.py` & `tgqSim-0.3.1/tgqSim/utils/dev_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.3.0/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.3.1/tgqSim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.3.0
+Version: 0.3.1
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.3.0/tgqSim.egg-info/SOURCES.txt` & `tgqSim-0.3.1/tgqSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

