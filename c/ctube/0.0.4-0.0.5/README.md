# Comparing `tmp/ctube-0.0.4.tar.gz` & `tmp/ctube-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.4.tar", max compression
+gzip compressed data, was "ctube-0.0.5.tar", max compression
```

## Comparing `ctube-0.0.4.tar` & `ctube-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.4/LICENSE
--rw-r--r--   0        0        0      610 2024-05-25 13:44:20.828071 ctube-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-05-25 13:45:20.440579 ctube-0.0.4/ctube/__init__.py
--rw-r--r--   0        0        0     4575 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/app.py
--rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/callbacks.py
--rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.4/ctube/cli.py
--rw-r--r--   0        0        0     2428 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/cmds.py
--rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/colors.py
--rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/containers.py
--rw-r--r--   0        0        0     4024 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/download.py
--rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/errors.py
--rw-r--r--   0        0        0     2119 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/extractors.py
--rw-r--r--   0        0        0     1430 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/helpers.py
--rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/parser.py
--rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/paths.py
--rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/printers.py
--rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/terminal.py
--rw-r--r--   0        0        0      622 2024-05-25 13:45:14.753991 ctube-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 ctube-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.5/LICENSE
+-rw-r--r--   0        0        0      610 2024-05-25 18:52:20.547021 ctube-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 18:52:15.213735 ctube-0.0.5/ctube/__init__.py
+-rw-r--r--   0        0        0     4661 2024-05-25 18:52:56.416704 ctube-0.0.5/ctube/app.py
+-rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/callbacks.py
+-rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.5/ctube/cli.py
+-rw-r--r--   0        0        0     2428 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/cmds.py
+-rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/colors.py
+-rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/containers.py
+-rw-r--r--   0        0        0     4252 2024-05-25 19:05:42.476915 ctube-0.0.5/ctube/download.py
+-rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/errors.py
+-rw-r--r--   0        0        0     2119 2024-05-25 18:07:35.045348 ctube-0.0.5/ctube/extractors.py
+-rw-r--r--   0        0        0     2084 2024-05-25 18:58:32.066191 ctube-0.0.5/ctube/helpers.py
+-rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/parser.py
+-rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/paths.py
+-rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/printers.py
+-rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/terminal.py
+-rw-r--r--   0        0        0      622 2024-05-25 18:52:26.703634 ctube-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 ctube-0.0.5/PKG-INFO
```

### Comparing `ctube-0.0.4/LICENSE` & `ctube-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/README.md` & `ctube-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.4-blue)
+![Version](https://img.shields.io/badge/version-0.0.5-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
 
 ### installation
 ```shell
 pip install ctube
 ```
 
 ---
 <p align="center">
-    <img src=".github/ctube.gif" alt="ctube.gfi">
+    <img src=".github/ctube.gif" alt="ctube.gif">
 </p>
```

### Comparing `ctube-0.0.4/ctube/app.py` & `ctube-0.0.5/ctube/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from innertube.clients import InnerTube
 from ctube.download import Downloader
 from ctube.errors import InvalidIndexSyntax
 from ctube.terminal import Prompt
 from ctube.containers import MusicItem
 from ctube.colors import Color
 from ctube.cmds import Command
-from ctube.helpers import get_filtered_music_items
+from ctube.helpers import get_filtered_music_items, handle_connection_errors
 from ctube.parser import parse_user_input
 from ctube.callbacks import (
     on_progress_callback, 
     on_complete_callback
 )
 from ctube.printers import (
     print_header, 
@@ -66,26 +66,28 @@
             elif cmd_name == Command.ID.value.name:
                 self._id(args)
             elif cmd_name == Command.DOWNLOAD.value.name:
                 self._download(args)
             else:
                 write("Invalid syntax", Color.RED)
 
+    @handle_connection_errors
     def _search(self, artist_name: str) -> None:
         if not artist_name:
             write("Missing argument: artist name", Color.RED)
         else:
             data = self.client.search(artist_name)
             try:
                 artist_id = extract_artist_id(data)
             except (KeyError, TypeError, IndexError):
                 write(f"Artist '{artist_name}' not found", Color.RED)
             else:
                 self._id(artist_id)
 
+    @handle_connection_errors
     def _id(self, artist_id: str) -> None:
         if not artist_id:
             write("Missing argument: artist id", Color.RED)
         else:
             data = self.client.browse(f"MPAD{artist_id}")
             try:
                 artist_music_data = extract_artist_music(data)
```

### Comparing `ctube-0.0.4/ctube/callbacks.py` & `ctube-0.0.5/ctube/callbacks.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/cmds.py` & `ctube-0.0.5/ctube/cmds.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/colors.py` & `ctube-0.0.5/ctube/colors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/download.py` & `ctube-0.0.5/ctube/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from pathvalidate import sanitize_filename
 from enum import Enum
 from urllib import request
+from urllib.error import HTTPError
 from typing import Callable, List
 from ctube.containers import MusicItem, DownloadData
+from ctube.helpers import handle_connection_errors
 from pytubefix import Playlist, Stream, YouTube
 from pytubefix.exceptions import (
         MembersOnly, 
         RecordingUnavailable, 
         VideoPrivate, 
         VideoUnavailable
 )
@@ -49,14 +51,15 @@
         self.on_complete_callback(data)
 
     def _on_progress_callback(self, data: DownloadData, bytes_remaining: int, stream: Stream) -> None:
         filesize = stream.filesize
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
+    @handle_connection_errors
     def download(self, item: MusicItem, artist: str) -> List[YouTube]:
         playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{item.playlist_id}")
         failed_downloads: List[YouTube] = []
 
         response = request.urlopen(item.thumbnail_url)
         image_data = response.read()
 
@@ -110,13 +113,16 @@
                     data, 
                     filepath  # type: ignore
                     # pytubefix says that 'filepath' can be None, 
                     # but this is not possible.
                 )
             )
 
-            audio_stream.download(
-                output_path=final_destination,
-                skip_existing=self.skip_existing
-            )
+            try:
+                audio_stream.download(
+                    output_path=final_destination,
+                    skip_existing=self.skip_existing
+                )
+            except HTTPError:
+                failed_downloads.append(youtube)
 
         return failed_downloads
```

### Comparing `ctube-0.0.4/ctube/extractors.py` & `ctube-0.0.5/ctube/extractors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/parser.py` & `ctube-0.0.5/ctube/parser.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/printers.py` & `ctube-0.0.5/ctube/printers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/ctube/terminal.py` & `ctube-0.0.5/ctube/terminal.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.4/pyproject.toml` & `ctube-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
```

### Comparing `ctube-0.0.4/PKG-INFO` & `ctube-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -20,25 +20,25 @@
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.4-blue)
+![Version](https://img.shields.io/badge/version-0.0.5-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
 
 ### installation
 ```shell
 pip install ctube
 ```
 
 ---
 <p align="center">
-    <img src=".github/ctube.gif" alt="ctube.gfi">
+    <img src=".github/ctube.gif" alt="ctube.gif">
 </p>
```

