# Comparing `tmp/twitch_archiver-4.0.8.tar.gz` & `tmp/twitch_archiver-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_archiver-4.0.8.tar", last modified: Sat May 18 22:39:08 2024, max compression
+gzip compressed data, was "twitch_archiver-4.0.9.tar", last modified: Sat May 25 23:54:31 2024, max compression
```

## Comparing `twitch_archiver-4.0.8.tar` & `twitch_archiver-4.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitcharchiver/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/realtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    32460 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/vod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 23:54:31.000000 twitch_archiver-4.0.9/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:31.926054 twitch_archiver-4.0.9/twitcharchiver/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/downloaders/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/downloaders/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/downloaders/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/downloaders/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-25 23:54:26.000000 twitch_archiver-4.0.9/twitcharchiver/vod.py
```

### Comparing `twitch_archiver-4.0.8/LICENSE` & `twitch_archiver-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/PKG-INFO` & `twitch_archiver-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.8
+Version: 4.0.9
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch_archiver-4.0.8/README.md` & `twitch_archiver-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/pyproject.toml` & `twitch_archiver-4.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "4.0.8"
+version = "4.0.9"
 dependencies = [
     "requests>=2.28.0",
     "m3u8>=0.3.12",
 ]
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
```

### Comparing `twitch_archiver-4.0.8/twitch_archiver.egg-info/PKG-INFO` & `twitch_archiver-4.0.9/twitch_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.8
+Version: 4.0.9
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch_archiver-4.0.8/twitch_archiver.egg-info/SOURCES.txt` & `twitch_archiver-4.0.9/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/__init__.py` & `twitch_archiver-4.0.9/twitcharchiver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from twitcharchiver.utils import (
     getenv,
     check_update_available,
     get_latest_version,
     get_temp_dir,
 )
 
-__version__ = "4.0.8"
+__version__ = "4.0.9"
 
 from twitcharchiver.vod import Vod, ArchivedVod
 
 
 def main():
     """
     Main processing for twitch-archiver.
```

### Comparing `twitch_archiver-4.0.8/twitcharchiver/api.py` & `twitch_archiver-4.0.9/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/arguments.py` & `twitch_archiver-4.0.9/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/channel.py` & `twitch_archiver-4.0.9/twitcharchiver/channel.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/configuration.py` & `twitch_archiver-4.0.9/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/database.py` & `twitch_archiver-4.0.9/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/downloader.py` & `twitch_archiver-4.0.9/twitcharchiver/downloader.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/downloaders/chat.py` & `twitch_archiver-4.0.9/twitcharchiver/downloaders/chat.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/downloaders/realtime.py` & `twitch_archiver-4.0.9/twitcharchiver/downloaders/realtime.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/downloaders/stream.py` & `twitch_archiver-4.0.9/twitcharchiver/downloaders/stream.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/downloaders/video.py` & `twitch_archiver-4.0.9/twitcharchiver/downloaders/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     safe_move,
     build_output_dir_name,
     get_hash,
     format_vod_chapters,
     time_since_date,
     write_json_file,
     get_temp_dir,
+    sanitize_command,
 )
 from twitcharchiver.vod import Vod, ArchivedVod
 
 # time in seconds between checking for new VOD parts if VOD is currently live and being updated
 CHECK_INTERVAL = 60
 
 
@@ -626,18 +627,22 @@
                 Path(self._output_dir, "parts", "segments.txt"), "w", encoding="utf8"
             ) as _segment_file:
                 for _part in self._completed_parts:
                     _segment_file.write(
                         f"file '{Path(self._output_dir, 'parts', _part)}'\n"
                     )
 
-            with subprocess.Popen(
+            _command = (
                 f"ffmpeg -hide_banner -fflags +genpts -f concat -safe 0 -y -i "
-                f'"{str(Path(self._output_dir, "parts", "segments.txt"))}" '
-                f'-c copy "{str(Path(self._output_dir, "merged.ts"))}"',
+                f'\'{str(Path(self._output_dir, "parts", "segments.txt"))}\' '
+                f'-c copy \'{str(Path(self._output_dir, "merged.ts"))}\''
+            )
+
+            with subprocess.Popen(
+                sanitize_command(_command),
                 shell=True,
                 stderr=subprocess.PIPE,
                 universal_newlines=True,
                 encoding="cp437",
             ) as _p:
                 # get progress from ffmpeg output and print progress bar
                 if not self._quiet:
@@ -674,25 +679,25 @@
         _corrupt_parts: set[MpegSegment] = set()
 
         # get dts offset of first available part
         _dts_offset = self._get_dts_offset()
 
         # create ffmpeg command
         _ffmpeg_cmd = (
-            f'ffmpeg -hide_banner -y -i "{Path(self._output_dir, "merged.ts")}" '
+            f'ffmpeg -hide_banner -y -i \'{Path(self._output_dir, "merged.ts")}\' '
         )
         # insert metadata if present
         if Path(self._output_dir, "parts", "chapters.txt").exists():
-            _ffmpeg_cmd += f'-i "{Path(self._output_dir, "parts", "chapters.txt")}" -map_metadata 1 '
+            _ffmpeg_cmd += f'-i \'{Path(self._output_dir, "parts", "chapters.txt")}\' -map_metadata 1 '
 
-        _ffmpeg_cmd += f'-c:a copy -c:v copy "{Path(self._output_dir, "vod.mp4")}"'
+        _ffmpeg_cmd += f'-c:a copy -c:v copy \'{Path(self._output_dir, "vod.mp4")}\''
 
         # convert merged .ts file to .mp4
         with subprocess.Popen(
-            _ffmpeg_cmd,
+            sanitize_command(_ffmpeg_cmd),
             shell=True,
             stderr=subprocess.PIPE,
             universal_newlines=True,
             encoding="cp437",
         ) as _p:
             # get progress from ffmpeg output and catch corrupt segments
             _ffmpeg_log = ""
@@ -770,17 +775,21 @@
         # fetch parts from dir
         _parts = self.get_completed_parts()
 
         if _parts:
             # fetch id of first part
             _part_id = int(_parts[0].replace(".ts", ""))
 
-            with subprocess.Popen(
+            _command = (
                 f"ffprobe -v quiet -print_format json -show_format -show_streams "
-                f'"{Path(self._output_dir, "parts", _parts[0])}"',
+                f'"{Path(self._output_dir, "parts", _parts[0])}"'
+            )
+
+            with subprocess.Popen(
+                sanitize_command(_command),
                 shell=True,
                 stdout=subprocess.PIPE,
                 universal_newlines=True,
                 encoding="cp437",
             ) as _p:
                 _ts_file_data = ""
                 for _line in _p.stdout:
@@ -805,18 +814,22 @@
         self._log.debug("Verifying length of VOD file.")
 
         # skip verification if .ignorelength present
         if Path(self._output_dir, ".ignorelength").is_file():
             self._log.debug(".ignorelength file present - skipping verification.")
             return True
 
+        _command = (
+            f'ffprobe -v quiet -i \'{Path(self._output_dir, "vod.mp4")}\' '
+            f"-show_entries format=duration -of default=noprint_wrappers=1:nokey=1"
+        )
+
         # retrieve vod file duration
         _p = subprocess.run(
-            f'ffprobe -v quiet -i "{Path(self._output_dir, "vod.mp4")}" '
-            f"-show_entries format=duration -of default=noprint_wrappers=1:nokey=1",
+            sanitize_command(_command),
             shell=True,
             capture_output=True,
             encoding="cp437",
         )
 
         if _p.returncode:
             raise VideoVerificationError(
```

### Comparing `twitch_archiver-4.0.8/twitcharchiver/exceptions.py` & `twitch_archiver-4.0.9/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/logger.py` & `twitch_archiver-4.0.9/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/processing.py` & `twitch_archiver-4.0.9/twitcharchiver/processing.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/twitch.py` & `twitch_archiver-4.0.9/twitcharchiver/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.8/twitcharchiver/utils.py` & `twitch_archiver-4.0.9/twitcharchiver/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,31 @@
     else:
         _dir_name = " - ".join(
             [format_timestamp(created_at), sanitize_text(title), "STREAM_ONLY"]
         )
     return _dir_name
 
 
+def sanitize_command(command: str):
+    """
+    Sanitizes a command to be passes to subprocess, single and double quotes mean different things depending on the
+    operating system.
+
+    :param command: Command to sanitize
+    :return: Sanitized command
+    """
+    if os.name == "nt":
+        # Windows command formatting
+        return command
+
+    # Linux / MacOS command formatting
+    elif os.name == "posix":
+        return command.replace('"', "'")
+
+
 def format_timestamp(timestamp: float):
     """
     Formats a given UTC timestamp to the YYYY-MM-DD_HH-MM-SS format.
 
     :param timestamp: UTC timestamp to convert
     :return: timestamp in YYYY-MM-DD_HH-MM-SS format
     """
```

### Comparing `twitch_archiver-4.0.8/twitcharchiver/vod.py` & `twitch_archiver-4.0.9/twitcharchiver/vod.py`

 * *Files identical despite different names*

