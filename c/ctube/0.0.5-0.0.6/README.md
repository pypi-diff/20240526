# Comparing `tmp/ctube-0.0.5.tar.gz` & `tmp/ctube-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.5.tar", max compression
+gzip compressed data, was "ctube-0.0.6.tar", max compression
```

## Comparing `ctube-0.0.5.tar` & `ctube-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.5/LICENSE
--rw-r--r--   0        0        0      610 2024-05-25 18:52:20.547021 ctube-0.0.5/README.md
--rw-r--r--   0        0        0       22 2024-05-25 18:52:15.213735 ctube-0.0.5/ctube/__init__.py
--rw-r--r--   0        0        0     4661 2024-05-25 18:52:56.416704 ctube-0.0.5/ctube/app.py
--rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/callbacks.py
--rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.5/ctube/cli.py
--rw-r--r--   0        0        0     2428 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/cmds.py
--rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/colors.py
--rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/containers.py
--rw-r--r--   0        0        0     4252 2024-05-25 19:05:42.476915 ctube-0.0.5/ctube/download.py
--rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/errors.py
--rw-r--r--   0        0        0     2119 2024-05-25 18:07:35.045348 ctube-0.0.5/ctube/extractors.py
--rw-r--r--   0        0        0     2084 2024-05-25 18:58:32.066191 ctube-0.0.5/ctube/helpers.py
--rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/parser.py
--rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/paths.py
--rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/printers.py
--rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.5/ctube/terminal.py
--rw-r--r--   0        0        0      622 2024-05-25 18:52:26.703634 ctube-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 ctube-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.6/LICENSE
+-rw-r--r--   0        0        0      610 2024-05-25 22:03:41.153679 ctube-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 22:03:57.640149 ctube-0.0.6/ctube/__init__.py
+-rw-r--r--   0        0        0     5151 2024-05-25 21:58:13.207804 ctube-0.0.6/ctube/app.py
+-rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/callbacks.py
+-rw-r--r--   0        0        0      552 2024-05-25 21:58:58.300542 ctube-0.0.6/ctube/cli.py
+-rw-r--r--   0        0        0     2428 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/cmds.py
+-rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/colors.py
+-rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/containers.py
+-rw-r--r--   0        0        0     4171 2024-05-25 21:59:24.906863 ctube-0.0.6/ctube/download.py
+-rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/errors.py
+-rw-r--r--   0        0        0     2119 2024-05-25 18:07:35.045348 ctube-0.0.6/ctube/extractors.py
+-rw-r--r--   0        0        0     2327 2024-05-25 21:35:04.168284 ctube-0.0.6/ctube/helpers.py
+-rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/parser.py
+-rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/paths.py
+-rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/printers.py
+-rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.6/ctube/terminal.py
+-rw-r--r--   0        0        0      641 2024-05-25 22:07:54.264059 ctube-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 ctube-0.0.6/PKG-INFO
```

### Comparing `ctube-0.0.5/LICENSE` & `ctube-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/README.md` & `ctube-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.5-blue)
+![Version](https://img.shields.io/badge/version-0.0.6-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
```

### Comparing `ctube-0.0.5/ctube/app.py` & `ctube-0.0.6/ctube/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import sys
 from typing import List, Optional, Tuple
+from urllib.error import URLError
 from innertube.clients import InnerTube
 from ctube.download import Downloader
 from ctube.errors import InvalidIndexSyntax
 from ctube.terminal import Prompt
 from ctube.containers import MusicItem
 from ctube.colors import Color
 from ctube.cmds import Command
-from ctube.helpers import get_filtered_music_items, handle_connection_errors
+from ctube.helpers import (
+    get_filtered_music_items, 
+    handle_connection_errors,
+    connected_to_internet
+)
 from ctube.parser import parse_user_input
 from ctube.callbacks import (
     on_progress_callback, 
     on_complete_callback
 )
 from ctube.printers import (
     print_header, 
@@ -97,32 +102,41 @@
                 artist_music_data: Tuple[List[MusicItem], str]
                 self._music_items, self._artist_name = artist_music_data
                 write(f"Collected music for {self._artist_name}", Color.GREEN)
                 print_music_items(self._music_items)
 
     def _download(self, indexes: str):
         if not self._music_items or not self._artist_name:
-            write("You need to search for music first. Use the search or id command", Color.RED)
+            write("You need to search for music first. ", Color.RED)
+            write("Use the search/id command", Color.RED)
         elif not indexes:
             write("Missing argument: indexes", Color.RED)
+        elif not connected_to_internet():
+            write("No internet connection", Color.RED)
         else:
             try:
                 filtered_items = get_filtered_music_items(self._music_items, indexes)
             except InvalidIndexSyntax as error:
                 write(str(error), Color.RED)
             else:
                 print('\033[?25l', end="")
                 if len(filtered_items) == len(self._music_items):
                     write(f"Selected items: ALL", Color.BLUE)
                 else:
                     write(f"Selected items:", Color.BLUE)
                 for item in filtered_items:
                     write(f"\u2022 {item.title}", Color.BOLD)
+
                 for item in filtered_items:
                     write(f":: Downloading: {item.title}", Color.GREEN)
-                    self.downloader.download(item=item, artist=self._artist_name)
-                    print('\033[?25h', end="")
+                    try:
+                        self.downloader.download(item=item, artist=self._artist_name)
+                    except (URLError, TimeoutError) as error:
+                        write(f"A connection error occurred while downloading: {item.title}", Color.RED)
+                        write(f"Reason: {str(error)}", Color.RED)
+                        break
+                print('\033[?25h', end="")
 
     @staticmethod
     def _exit():
         sys.stdout.write('\033[?25h')
         sys.exit(0)
```

### Comparing `ctube-0.0.5/ctube/callbacks.py` & `ctube-0.0.6/ctube/callbacks.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/cmds.py` & `ctube-0.0.6/ctube/cmds.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/colors.py` & `ctube-0.0.6/ctube/colors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/download.py` & `ctube-0.0.6/ctube/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from pathvalidate import sanitize_filename
 from enum import Enum
 from urllib import request
 from urllib.error import HTTPError
 from typing import Callable, List
 from ctube.containers import MusicItem, DownloadData
-from ctube.helpers import handle_connection_errors
 from pytubefix import Playlist, Stream, YouTube
 from pytubefix.exceptions import (
         MembersOnly, 
         RecordingUnavailable, 
         VideoPrivate, 
         VideoUnavailable
 )
@@ -51,15 +50,14 @@
         self.on_complete_callback(data)
 
     def _on_progress_callback(self, data: DownloadData, bytes_remaining: int, stream: Stream) -> None:
         filesize = stream.filesize
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
-    @handle_connection_errors
     def download(self, item: MusicItem, artist: str) -> List[YouTube]:
         playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{item.playlist_id}")
         failed_downloads: List[YouTube] = []
 
         response = request.urlopen(item.thumbnail_url)
         image_data = response.read()
```

### Comparing `ctube-0.0.5/ctube/extractors.py` & `ctube-0.0.6/ctube/extractors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/helpers.py` & `ctube-0.0.6/ctube/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import requests
 from typing import List , Callable
 from urllib.error import URLError
 from httpx import ReadTimeout, ConnectTimeout, ConnectError
 from innertube.errors import RequestError
 from ctube.containers import MusicItem
 from ctube.errors import InvalidIndexSyntax
 from ctube.parser import parse_indexes
@@ -45,7 +46,15 @@
         except RequestError:
             write("Invalid request", Color.RED)
         except (ConnectTimeout, ReadTimeout):
             write("An error occurred. try again.", Color.RED)
         except (ConnectError, URLError):
             write("No internet connection", Color.RED)
     return inner
+
+
+def connected_to_internet(url: str = 'http://www.google.com/', timeout: int = 5) -> bool:
+    try:
+        _ = requests.head(url, timeout=timeout)
+        return True
+    except requests.ConnectionError:
+        return False
```

### Comparing `ctube-0.0.5/ctube/parser.py` & `ctube-0.0.6/ctube/parser.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/printers.py` & `ctube-0.0.6/ctube/printers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/ctube/terminal.py` & `ctube-0.0.6/ctube/terminal.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.5/pyproject.toml` & `ctube-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
@@ -12,14 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pydub = "^0.25.1"
 eyed3 = "^0.9.7"
 innertube = "^2.1.16"
 pytubefix = "^5.4.2"
 pathvalidate = "^3.2.0"
+requests="^2.32.2"
 
 [tool.poetry.scripts]
 ctube = "ctube.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ctube-0.0.5/PKG-INFO` & `ctube-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,19 +16,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eyed3 (>=0.9.7,<0.10.0)
 Requires-Dist: innertube (>=2.1.16,<3.0.0)
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.5-blue)
+![Version](https://img.shields.io/badge/version-0.0.6-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
```

