# Comparing `tmp/rumchat_actor-1.2.0.tar.gz` & `tmp/rumchat_actor-1.3.0.tar.gz`

## Comparing `rumchat_actor-1.2.0.tar` & `rumchat_actor-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    22561 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/src/rumchat_actor/__init__.py
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/src/rumchat_actor/common_commands.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/src/rumchat_actor/__init__.py
+-rw-r--r--   0        0        0    26512 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/src/rumchat_actor/common_commands.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.3.0/PKG-INFO
```

### Comparing `rumchat_actor-1.2.0/.github/workflows/python-publish.yml` & `rumchat_actor-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.2.0/src/rumchat_actor/__init__.py` & `rumchat_actor-1.3.0/src/rumchat_actor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,16 +480,17 @@
         if not message.text.startswith(COMMAND_PREFIX):
             return
 
         #Get command name
         name = message.text.split()[0].removeprefix(COMMAND_PREFIX)
 
         #Is not a valid command
-        if name not in self.chat_commands and self.invalid_command_respond:
-            self.send_message(f"@{message.user.username} That is not a registered command.")
+        if name not in self.chat_commands:
+            if self.invalid_command_respond:
+                self.send_message(f"@{message.user.username} That is not a registered command.")
             return
 
         self.chat_commands[name].call(message)
 
     def register_command(self, command, name = None):
         """Register a command"""
         #Is a ChatCommand instance
```

### Comparing `rumchat_actor-1.2.0/src/rumchat_actor/common_commands.py` & `rumchat_actor-1.3.0/src/rumchat_actor/common_commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 """Rumble chat actor common commands
 
 Derivative classes for common chat commands.
 S.D.G."""
 
 import os
+import shutil
 import sys
 import tempfile
 import time
 import threading
+from tkinter import filedialog, Tk
 from cocorum.localvars import RUMBLE_BASE_URL, DEFAULT_TIMEOUT
 from browsermobproxy import Server
 from moviepy.editor import VideoFileClip, concatenate_videoclips
 import requests
 # import selenium
 from selenium import webdriver
 from selenium.webdriver.common.by import By
@@ -21,14 +23,17 @@
 
 OP_PATH = __file__[:__file__.rfind(os.sep)] #The path of the script
 BROWSERMOB_EXE = 'browsermob-proxy' #The Browsermob Proxy executable
 WAIT_FOR_LIVE_REFRESH_RATE = 10 #How often to refresh while waiting for a livestream to start
 CLIP_FILENAME_EXTENSION = "mp4" #The filename extension for saved clips
 CLIP_BITRATE = "4.5M" #The bitrate to use when saving clips. Deprecating
 STREAM_QUALITIES = {"360p" : "1.2M", "720p" : "2.8M", "1080p" : "4.5M"} #Valid resolutions of a livestream and the bitrates they use / should be saved with
+DEFAULT_CLIP_BITRATE = STREAM_QUALITIES["1080p"] #The default save quality for clips from a local recording
+VALID_CLIP_RECORDING_CONTAINERS = ["ts"] #Formats that the OBS recording can be in if recording-trimmed clips are to work
+TEMP_RECORDING_COPY_FILENAME = ".temp_recording_copy"
 NUM_TS_DOWNLOAD_TIME_CHECKS = 5 #How many times to test a TS chunk download to get its average download time
 TS_DOWNLOAD_SPEEDFACTOR_REQUIREMENT = 2 #TS chunks must be able to download this many times faster than their duration to be usable in a cache. Cannot be less than 1
 
 class TTSCommand(ChatCommand):
     """Text-to-speech command"""
     def __init__(self, *args, name = "tts", voices = {"default" : talkey.Talkey().say}, **kwargs):
         """Pass the same args and kwargs as ChatCommand, plus:
@@ -114,14 +119,15 @@
 class ClipDownloaderCommand(ChatCommand):
     """Save clips of the livestream by downloading stream chunks from Rumble, works remotely"""
     def __init__(self, actor, name = "clip", default_duration = 60, max_duration = 120, clip_save_path = "." + os.sep, browsermob_exe = BROWSERMOB_EXE):
         """actor: The Rumchat Actor
     name: The name of the command
     default_duration: How long the clip will last with no duration specified
     max_duration: How long the clip can possibly be (i.e. how much of the livestream to save)
+    clip_save_path: Where to save clips to when they are made
     browsermob_exe: The path to the Browsermob Proxy executable"""
         super().__init__(name = name, actor = actor, cooldown = default_duration)
         self.default_duration = default_duration
         self.max_duration = max_duration
         self.clip_save_path = clip_save_path #Where to save the completed clips
         self.browsermob_exe = browsermob_exe
         self.ready_to_clip = False
@@ -449,7 +455,123 @@
             self.running_clipsaves = 0
 
         #We are responsible for DVR tempfile closing
         if self.is_dvr:
             for tf in tempfiles:
                 tf.close()
         print("Complete")
+
+class ClipRecordingCommand(ChatCommand):
+    """Save clips of the livestream by duplicating then trimming an in-progress TS recording by OBS"""
+    def __init__(self, actor, name = "clip", default_duration = 60, max_duration = 120, recording_load_path = ".", clip_save_path = "." + os.sep):
+        """actor: The Rumchat Actor
+    name: The name of the command
+    default_duration: How long the clip will last with no duration specified
+    max_duration: How long the clip can possibly be
+    recording_load_path: Where recordings from OBS are stored, used for filedialog init
+    clip_save_path: Where to save clips to when they are made"""
+        super().__init__(name = name, actor = actor, cooldown = default_duration)
+        self.default_duration = default_duration
+        self.max_duration = max_duration
+        self.recording_load_path = recording_load_path
+        self.clip_save_path = clip_save_path #Where to save the completed clips
+        self.running_clipsaves = 0 #How many clip save operations are running
+        self.__recording_filename = None #The filename of the running OBS recording, asked later
+        print(self.recording_filename) #...now is later
+
+    @property
+    def recording_filename(self):
+        """The filename of the running OBS recording"""
+        #We do not know the filename yet
+        while not self.__recording_filename:
+            #Make and hide a background Tk window to allow filedialogs to appear
+            root = Tk()
+            root.withdraw()
+
+            #Ask for the OBS recording in progress
+            self.__recording_filename = filedialog.askopenfilename(
+                title = "Select OBS recording in progress",
+                initialdir = self.recording_load_path,
+                filetypes=(("Freezable video files", ";".join("*." + container for container in VALID_CLIP_RECORDING_CONTAINERS)),
+                                       ("All files", "*.*") ),
+                )
+
+            #Destroy the background window
+            root.destroy()
+
+        return self.__recording_filename
+
+    @property
+    def recording_container(self):
+        """The container format of the recording"""
+        return self.recording_filename.split(".")[-1]
+
+    @property
+    def recording_copy_fn(self):
+        """The filename of the temporary recording copy"""
+        return TEMP_RECORDING_COPY_FILENAME + "." + self.recording_container
+
+    def run(self, message):
+        """Make a clip. TODO mostly identical to ClipDownloaderCommand().run()"""
+        segs = message.text.split()
+        #Only called clip, no arguments
+        if len(segs) == 1:
+            self.save_clip(self.default_duration)
+
+        #Arguments were passed
+        else:
+            #The first argument is a number
+            if segs[1].isnumeric():
+                #Invalid length passed
+                if not 0 < int(segs[1]) <= self.max_duration:
+                    self.actor.send_message(f"@{message.user.username} Invalid clip length.")
+                    return
+
+                #Only length was specified
+                if len(segs) == 2:
+                    self.save_clip(int(segs[1]))
+
+                #A name was also specified
+                else:
+                    self.save_clip(int(segs[1]), "_".join(segs[2:]))
+
+            #The first argument is not a number, treat it as a filename
+            else:
+                self.save_clip(self.default_duration, "_".join(segs[1:]))
+
+    def save_clip(self, duration, filename = None):
+        """Save a clip with the given duration to the filename"""
+        #No filename specified, construct from time values
+        if not filename:
+            t = time.time()
+            filename = f"{round(t - duration)}-{round(t)}"
+
+        #Report clip save
+        self.actor.send_message(f"Saving clip {filename}, duration of {duration} seconds.")
+
+        #Run the clip save in a thread
+        saveclip_thread = threading.Thread(target = self.form_recording_into_clip, args = (duration, filename), daemon = True)
+        saveclip_thread.start()
+
+    def form_recording_into_clip(self, duration, filename):
+        """Do the actual file operations to save a clip"""
+        #Keep a counter of running clipsaves, may not be needed
+        self.running_clipsaves += 1
+
+        print("Making frozen copy of recording")
+        shutil.copy(self.recording_filename, self.recording_copy_fn)
+        print("Loading copy")
+        recording = VideoFileClip(self.recording_copy_fn)
+        print("Trimming")
+        clip = recording.subclip(max((recording.duration - duration, 0)), recording.duration)
+        print("Saving clip")
+        clip.write_videofile(self.clip_save_path + os.sep + filename + "." + CLIP_FILENAME_EXTENSION, logger = None)
+        print("Closing and deleting frozen copy")
+        recording.close()
+        os.system("rm " + self.recording_copy_fn)
+        print("Done.")
+
+        #Make note that the clipsave has finished
+        self.running_clipsaves -= 1
+        if self.running_clipsaves < 0:
+            print("ERROR: Running clipsaves is now negative. Resetting it to zero, but this should not happen.")
+            self.running_clipsaves = 0
```

### Comparing `rumchat_actor-1.2.0/LICENSE.txt` & `rumchat_actor-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.2.0/README.md` & `rumchat_actor-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.2.0/pyproject.toml` & `rumchat_actor-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rumchat_actor"
-version = "1.2.0"
+version = "1.3.0"
 keywords = ["rumble", "chat", "livestream", "bot"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "Automatically interact with your Rumble livestream chats."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `rumchat_actor-1.2.0/PKG-INFO` & `rumchat_actor-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rumchat_actor
-Version: 1.2.0
+Version: 1.3.0
 Summary: Automatically interact with your Rumble livestream chats.
 Project-URL: Homepage, https://github.com/thelabcat/rum-chat-actor
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: bot,chat,livestream,rumble
 Classifier: Development Status :: 4 - Beta
```

