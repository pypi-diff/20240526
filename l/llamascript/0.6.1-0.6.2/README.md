# Comparing `tmp/llamascript-0.6.1.tar.gz` & `tmp/llamascript-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamascript-0.6.1.tar", last modified: Wed May 15 15:22:58 2024, max compression
+gzip compressed data, was "llamascript-0.6.2.tar", last modified: Sun May 26 01:31:54 2024, max compression
```

## Comparing `llamascript-0.6.1.tar` & `llamascript-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-15 15:22:49.000000 llamascript-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 15:22:58.351679 llamascript-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-15 15:22:49.000000 llamascript-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/llamascript/
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-15 15:22:49.000000 llamascript-0.6.1/llamascript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:22:58.351679 llamascript-0.6.1/llamascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 15:22:58.000000 llamascript-0.6.1/llamascript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:22:58.351679 llamascript-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 15:22:49.000000 llamascript-0.6.1/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-26 01:31:54.506520 llamascript-0.6.2/
+-rw-r--r--   0 lewis-family   (501) staff       (20)    11324 2024-04-30 20:50:05.000000 llamascript-0.6.2/LICENSE
+-rw-r--r--   0 lewis-family   (501) staff       (20)     3079 2024-05-26 01:31:54.505241 llamascript-0.6.2/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2615 2024-05-25 13:56:53.000000 llamascript-0.6.2/README.md
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-26 01:31:54.501473 llamascript-0.6.2/llamascript/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     6467 2024-05-26 01:31:01.000000 llamascript-0.6.2/llamascript/__init__.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-05-26 01:31:54.504332 llamascript-0.6.2/llamascript.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     3079 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      262 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       48 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/entry_points.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/requires.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       12 2024-05-26 01:31:54.000000 llamascript-0.6.2/llamascript.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-05-26 01:31:54.506683 llamascript-0.6.2/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      942 2024-05-15 15:16:17.000000 llamascript-0.6.2/setup.py
```

### Comparing `llamascript-0.6.1/LICENSE` & `llamascript-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llamascript-0.6.1/PKG-INFO` & `llamascript-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.1
+Version: 0.6.2
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.6.1/README.md` & `llamascript-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `llamascript-0.6.1/llamascript/__init__.py` & `llamascript-0.6.2/llamascript/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 import asyncio
 import ollama
 import logging
 import sys
 import subprocess
 import os
 
+dbg = False
+
+def debug(message):
+    if dbg:
+        print(message)
+
 # Set up logging
 logging.basicConfig(level=logging.WARNING)
 
 
 class llama:
     def __init__(self):
         self.model = ""
@@ -37,19 +43,21 @@
             split_line = line.split(" ", 1)
             prompt = split_line[1] if len(split_line) > 1 else ""
             self.system = [{"role": "system", "content": prompt}]
 
     def CHAT(self, stream: bool = False):
         for _ in range(3):
             try:
+                debug("Attempting to chat with model...")
                 response = ollama.chat(
                     model=self.model,
                     messages=self.system + [{"role": "user", "content": self.data}],
                     stream=stream,
                 )
+                debug("Chat successful.")
                 if stream:
                     for message in response:
                         print(message["message"]["content"], end="")
                     print()
                 else:
                     print(response["message"]["content"])
                 break
@@ -96,18 +104,15 @@
                         print(stdout.decode())
             print("Removing Modelfile...")
             os.remove(filename)
 
         except Exception as e:
             logging.error("Error creating model file: %s", e)
             print(f"Error creating model file {filename}.")
-        
-    def REPEAT(self, command, repeat_count):
-        for _ in range(repeat_count):
-            self.execute_command(command)
+            sys.exit(1)
 
     def execute_command(self, command):
         if command.startswith("PROMPT INPUT"):
             self.INPUT("PROMPT")
         elif command.startswith("CHAT"):
             self.CHAT()
         else:
@@ -120,25 +125,15 @@
                 i = 0
                 while i < len(lines):
                     line = lines[i].strip()
                     if not line:
                         i += 1
                         continue
                     command = line.split(" ")
-                    if command[0] == "REPEAT":
-                        repeat_count = int(command[1]) if len(command) > 1 else 1
-                        repeat_commands = []
-                        i += 1
-                        while i < len(lines) and not lines[i].strip().startswith("ENDREPEAT"):
-                            repeat_commands.append(lines[i].strip())
-                            i += 1
-                        for _ in range(repeat_count):
-                            for repeat_command in repeat_commands:
-                                self.execute_command(repeat_command)
-                    elif command[0] == "USE":
+                    if command[0] == "USE":
                         self.USE(line)
                     elif len(command) > 1 and command[1] == "INPUT":
                         self.INPUT(command[0])
                     elif command[0] == "SYSTEM":
                         self.SYSTEM(line=line)
                     elif command[0] == "PROMPT":
                         self.PROMPT(line=line)
@@ -151,25 +146,21 @@
                         parameters = {
                             "model": self.model,
                             "temperature": command[2] if len(command) > 2 else 0.7,
                             "system_message": self.system[0]["content"],
                         }
                         self.CREATE_MODEL("Modelfile", parameters, model_name)
                     elif command[0] == "CHAT":
-                        if len(command) > 1 and command[1] == "STREAM":
-                            stream = command[1] == True
+                        if len(command) > 1 and command[1] == "STREAM":\
+                            self.CHAT(stream=True)
                         else:
-                            stream = False
-                        self.CHAT(stream=stream)
-                    elif command[0] == "REPEAT":
-                        repeat_count = int(command[1]) if len(command) > 1 else 1
-                        repeat_command = " ".join(command[2:])
-                        self.REPEAT(repeat_command, repeat_count)
+                            self.CHAT()
                     else:
                         raise ValueError("Invalid command")
+                    i += 1
         except FileNotFoundError:
             logging.error("File %s not found.", filename)
             print(f"File {filename} not found.")
 
 
 import argparse
```

### Comparing `llamascript-0.6.1/llamascript.egg-info/PKG-INFO` & `llamascript-0.6.2/llamascript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamascript
-Version: 0.6.1
+Version: 0.6.2
 Summary: No-code AI chatbot using Ollama.
 Home-page: https://github.com/WolfTheDeveloper/llamascript
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llamascript-0.6.1/setup.py` & `llamascript-0.6.2/setup.py`

 * *Files identical despite different names*

