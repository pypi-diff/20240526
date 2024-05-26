# Comparing `tmp/pyjectify-0.6.tar.gz` & `tmp/pyjectify-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjectify-0.6.tar", last modified: Wed Mar  6 09:26:41 2024, max compression
+gzip compressed data, was "pyjectify-0.7.tar", last modified: Sun May 26 13:06:49 2024, max compression
```

## Comparing `pyjectify-0.6.tar` & `pyjectify-0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-06 09:26:37.000000 pyjectify-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-06 09:26:41.984308 pyjectify-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-06 09:26:37.000000 pyjectify-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify/windows/core/
--rw-r--r--   0 runner    (1001) docker     (127)    22767 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/core/defines.py
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/core/pe.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/core/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify/windows/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/modules/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/modules/inject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/modules/memscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/modules/pythonlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify/windows/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/utils/apisetschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-06 09:26:37.000000 pyjectify-0.6/pyjectify/windows/utils/syscall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:26:41.984308 pyjectify-0.6/pyjectify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-06 09:26:41.000000 pyjectify-0.6/pyjectify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-06 09:26:41.000000 pyjectify-0.6/pyjectify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 09:26:41.000000 pyjectify-0.6/pyjectify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 09:26:41.000000 pyjectify-0.6/pyjectify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-06 09:26:37.000000 pyjectify-0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 09:26:41.984308 pyjectify-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-26 13:06:42.000000 pyjectify-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-26 13:06:49.685485 pyjectify-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-26 13:06:42.000000 pyjectify-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.681485 pyjectify-0.7/pyjectify/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/pyjectify/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/pyjectify/windows/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    22789 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/core/defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/core/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/core/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/pyjectify/windows/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/modules/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/modules/inject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/modules/memscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/modules/pythonlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/pyjectify/windows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/utils/apisetschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-26 13:06:42.000000 pyjectify-0.7/pyjectify/windows/utils/syscall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:06:49.685485 pyjectify-0.7/pyjectify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-26 13:06:49.000000 pyjectify-0.7/pyjectify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-26 13:06:49.000000 pyjectify-0.7/pyjectify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:06:49.000000 pyjectify-0.7/pyjectify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 13:06:49.000000 pyjectify-0.7/pyjectify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-26 13:06:42.000000 pyjectify-0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:06:49.685485 pyjectify-0.7/setup.cfg
```

### Comparing `pyjectify-0.6/LICENSE` & `pyjectify-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/PKG-INFO` & `pyjectify-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjectify
-Version: 0.6
+Version: 0.7
 Summary: A Python library for memory manipulation, code injection and function hooking
 Author: Petitoto
 Project-URL: Homepage, https://github.com/Petitoto/pyjectify
 Project-URL: Bug Tracker, https://github.com/Petitoto/pyjectify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjectify-0.6/README.md` & `pyjectify-0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/__init__.py` & `pyjectify-0.7/pyjectify/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/core/defines.py` & `pyjectify-0.7/pyjectify/windows/core/defines.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,16 +509,16 @@
         ('PageAddress', DWORD),
         ('BlockSize', DWORD),
     ]
 
 class BASE_RELOCATION_ENTRY(ctypes.Structure):
     _pack_ = 1
     _fields_ = [
-        ('Offset', UINT, 12),
-        ('Type', UINT, 4),
+        ('Offset', ctypes.c_uint16, 12),
+        ('Type', ctypes.c_uint16, 4),
     ]
 
 
 # Process structs
 class PROCESSENTRY32(ctypes.Structure):
     _fields_ = [
         ('dwSize', DWORD),
```

### Comparing `pyjectify-0.6/pyjectify/windows/core/pe.py` & `pyjectify-0.7/pyjectify/windows/core/pe.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                         entry = self._fill_struct(BASE_RELOCATION_ENTRY, relocations.VirtualAddress + offset)
                         offset += ctypes.sizeof(BASE_RELOCATION_ENTRY)
                         
                         relocation_addr = relocation.PageAddress + entry.Offset
                         raw.seek(relocation_addr)
                         
                         if entry.Type == IMAGE_REL_BASED_ABSOLUTE:
-                            break
+                            continue
                         
                         elif entry.Type == IMAGE_REL_BASED_HIGH:
                             address = self._read_int(relocation_addr, 2) + HIWORD(delta)
                             raw.write(address.to_bytes(2, byteorder='little'))
                         
                         elif entry.Type == IMAGE_REL_BASED_LOW:
                             address = self._read_int(relocation_addr, 2) + LOWORD(delta)
@@ -271,14 +271,23 @@
                             raw.write(address.to_bytes(8, byteorder='little'))
                         
                         else:
                             raise InvalidPEHeader('Unknown relocation entry type - %s' % entry.Type)
                         
                     relocation = self._fill_struct(BASE_RELOCATION_BLOCK, relocations.VirtualAddress + offset)
             
+            if self.x86:
+                self.nt_header.OptionalHeader.ImageBase = DWORD(base_addr)
+                raw.seek(self.dos_header.e_lfanew + IMAGE_NT_HEADERS32.OptionalHeader.offset + IMAGE_OPTIONAL_HEADER32.ImageBase.offset)
+                raw.write(base_addr.to_bytes(4, byteorder='little'))
+            else:
+                self.nt_header.OptionalHeader.ImageBase = ULONGLONG(base_addr)
+                raw.seek(self.dos_header.e_lfanew + IMAGE_NT_HEADERS64.OptionalHeader.offset + IMAGE_OPTIONAL_HEADER64.ImageBase.offset)
+                raw.write(base_addr.to_bytes(8, byteorder='little'))
+            
             raw.seek(0)
             self.raw = raw.read()
             self.base_addr = base_addr
     
     
     def patch_import(self, thunk_addr: int, address: int) -> None:
         """Patch PE imports
```

### Comparing `pyjectify-0.6/pyjectify/windows/core/process.py` & `pyjectify-0.7/pyjectify/windows/core/process.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/modules/hook.py` & `pyjectify-0.7/pyjectify/windows/modules/hook.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/modules/inject.py` & `pyjectify-0.7/pyjectify/windows/modules/inject.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         
         Args:
             libpath: the path of the library to load in the target process
         
         Returns:
             A PyJectify's PE object representing the library loaded in the target process
         """
+        if not libpath:
+            return
+        
         addr = self._process.allocate(len(libpath))
         self._process.write(addr, libpath)
         kernel32_mod = self._process.get_module('kernel32.dll')
         loadlibrary_addr = kernel32_mod.base_addr + kernel32_mod.exports['LoadLibraryA']
         thread_h = self._process.start_thread(loadlibrary_addr, addr)
         lib_h = self._process.join_thread(thread_h)
         self._process.free(addr)
@@ -44,21 +47,22 @@
             if not lib_h:
                 raise WinAPIError('Remote LoadLibraryA failed')
             return self._process.module_from_hmodule(lib_h)
         else:
             return self._process.get_module(libpath)
     
     
-    def memory_loader(self, module: PE, prefer_base_addr: bool = True, copy_headers: bool = True) -> PE:
+    def memory_loader(self, module: PE, prefer_base_addr: bool = True, copy_headers: bool = True, call_entry_point: bool = True) -> PE:
         """Fully map a library from memory in the target process, resolving imports and ApiSet
         
         Args:
-            module: a PyJectify's PE object representinf the library to load in the target process
+            module: a PyJectify's PE object representing the library to load in the target process
             prefer_base_addr: specify whether to load the module at the PE's default base address
             copy_headers: specify whether to copy the PE headers to the target process memory
+            call_entry_point: specify whether to call the entry point with DLL_PROCESS_ATTACH flag
         
         Returns:
             A PyJectify's PE object representing the library loaded in the target process
         """
         start = 0
         if not copy_headers:
             start = module.sections_header[0].VirtualAddress
@@ -97,23 +101,24 @@
         
         self._process.write(module.base_addr+start, module.raw[start:])
         self._process.protect(module.base_addr+start, len(module.raw[start:]), PAGE_READONLY)
         
         for section_addr, section_size, protect in module.sections:
             self._process.protect(module.base_addr + section_addr, section_size, protect)
         
-        entry_point = module.base_addr + module.nt_header.OptionalHeader.AddressOfEntryPoint
-        
-        if self._process.x86:
-            entry_call = _entry_call_x86 % (entry_point.to_bytes(4, 'little'), module.base_addr.to_bytes(4, 'little'))
-        else:
-            entry_call = _entry_call_x64 % (entry_point.to_bytes(8, 'little'), module.base_addr.to_bytes(8, 'little'))
-        
-        entry_call_addr = self._process.allocate(len(entry_call), protect=PAGE_READWRITE)
-        self._process.write(entry_call_addr, entry_call)
-        self._process.protect(entry_call_addr, len(entry_call), PAGE_EXECUTE_READ)
-        
-        thread = self._process.start_thread(entry_call_addr)
-        self._process.join_thread(thread)
-        self._process.free(entry_call_addr)
+        if call_entry_point:
+            entry_point = module.base_addr + module.nt_header.OptionalHeader.AddressOfEntryPoint
+            
+            if self._process.x86:
+                entry_call = _entry_call_x86 % (entry_point.to_bytes(4, 'little'), module.base_addr.to_bytes(4, 'little'))
+            else:
+                entry_call = _entry_call_x64 % (entry_point.to_bytes(8, 'little'), module.base_addr.to_bytes(8, 'little'))
+            
+            entry_call_addr = self._process.allocate(len(entry_call), protect=PAGE_READWRITE)
+            self._process.write(entry_call_addr, entry_call)
+            self._process.protect(entry_call_addr, len(entry_call), PAGE_EXECUTE_READ)
+            
+            thread = self._process.start_thread(entry_call_addr)
+            self._process.join_thread(thread)
+            self._process.free(entry_call_addr)
         
         return module
```

### Comparing `pyjectify-0.6/pyjectify/windows/modules/memscan.py` & `pyjectify-0.7/pyjectify/windows/modules/memscan.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/modules/pythonlib.py` & `pyjectify-0.7/pyjectify/windows/modules/pythonlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     
     def setprogramname(self, programname: str) -> None:
         """Set the value of the argv[0] argument to the main() function
         
         Args:
             programname: the new programname
         """
-        programname = bytes(programname, encoding='utf-16le')
+        if programname:
+            programname = bytes(programname, encoding='utf-16le')
+        else:
+            programname = b'\x00'
+        
         addr = self._process.allocate(len(programname))
         self._process.write(addr, programname)
         
         py_setprogramname = self.python_mod.base_addr + self.python_mod.exports['Py_SetProgramName']
         
         thread = self._process.start_thread(py_setprogramname, addr)
         self._process.join_thread(thread)
@@ -48,15 +52,19 @@
     
     def setpath(self, pythonpath: str) -> None:
         """Set the default module search path
         
         Args:
             pythonpath: the PYTHON_PATH value
         """
-        pythonpath = bytes(pythonpath, encoding='utf-16le')
+        if pythonpath:
+            pythonpath = bytes(pythonpath, encoding='utf-16le')
+        else:
+            pythonpath = b'\x00'
+        
         addr = self._process.allocate(len(pythonpath))
         self._process.write(addr, pythonpath)
         
         py_setpath = self.python_mod.base_addr + self.python_mod.exports['Py_SetPath']
         
         thread = self._process.start_thread(py_setpath, addr)
         self._process.join_thread(thread)
@@ -67,15 +75,19 @@
     def setpythonhome(self, pythonhome: str) -> None:
         """Set the default "home" directory
         This method calls Py_SetPythonHome
         
         Args:
             pythonhome: the PYTHON_HOME value
         """
-        pythonhome = bytes(pythonhome, encoding='utf-16le')
+        if pythonhome:
+            pythonhome = bytes(pythonhome, encoding='utf-16le')
+        else:
+            pythonhome = b'\x00'
+        
         addr = self._process.allocate(len(pythonhome))
         self._process.write(addr, pythonhome)
         
         py_setpythonhome = self.python_mod.base_addr + self.python_mod.exports['Py_SetPythonHome']
         
         thread = self._process.start_thread(py_setpythonhome, addr)
         self._process.join_thread(thread)
@@ -116,18 +128,21 @@
     def exec(self, py_code: str) -> None:
         """Execute python code in the target process (acquire and then release the GIL). Python interpreter MUST be initialized.
         This method calls PyEval_RestoreThread + PyRun_SimpleString + PyEval_SaveThread
         
         Args:
             py_code: the python code to run
         """
+        if not py_code:
+            return
+        
         py_eval_restore_thread = self.python_mod.base_addr + self.python_mod.exports['PyEval_RestoreThread']
         py_run_simple_string = self.python_mod.base_addr + self.python_mod.exports['PyRun_SimpleString']
         py_eval_save_thread = self.python_mod.base_addr + self.python_mod.exports['PyEval_SaveThread']
-                
+        
         pycode_addr = self._process.allocate(len(py_code))
         self._process.write(pycode_addr, py_code)
         
         ret = self._process.run_funcs([(py_eval_restore_thread, self._tstate), (py_run_simple_string, pycode_addr), (py_eval_save_thread, 0)])
         self._tstate = ret[2]
         return
```

### Comparing `pyjectify-0.6/pyjectify/windows/utils/apisetschema.py` & `pyjectify-0.7/pyjectify/windows/utils/apisetschema.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify/windows/utils/syscall.py` & `pyjectify-0.7/pyjectify/windows/utils/syscall.py`

 * *Files identical despite different names*

### Comparing `pyjectify-0.6/pyjectify.egg-info/PKG-INFO` & `pyjectify-0.7/pyjectify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjectify
-Version: 0.6
+Version: 0.7
 Summary: A Python library for memory manipulation, code injection and function hooking
 Author: Petitoto
 Project-URL: Homepage, https://github.com/Petitoto/pyjectify
 Project-URL: Bug Tracker, https://github.com/Petitoto/pyjectify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjectify-0.6/pyjectify.egg-info/SOURCES.txt` & `pyjectify-0.7/pyjectify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

