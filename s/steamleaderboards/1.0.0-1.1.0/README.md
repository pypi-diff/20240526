# Comparing `tmp/steamleaderboards-1.0.0.tar.gz` & `tmp/steamleaderboards-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamleaderboards-1.0.0.tar", max compression
+gzip compressed data, was "steamleaderboards-1.1.0.tar", max compression
```

## Comparing `steamleaderboards-1.0.0.tar` & `steamleaderboards-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2024-05-24 23:19:06.948186 steamleaderboards-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1962 2024-05-25 01:52:35.242334 steamleaderboards-1.0.0/README.md
--rw-r--r--   0        0        0      983 2024-05-25 01:11:24.553294 steamleaderboards-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5460 2024-05-25 01:05:23.296288 steamleaderboards-1.0.0/steamleaderboards/__init__.py
--rw-r--r--   0        0        0     1728 2024-05-25 01:09:21.964292 steamleaderboards-1.0.0/steamleaderboards/__main__.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 steamleaderboards-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-24 23:19:06.948186 steamleaderboards-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2076 2024-05-25 01:55:51.395337 steamleaderboards-1.1.0/README.md
+-rw-r--r--   0        0        0      983 2024-05-26 08:32:26.181580 steamleaderboards-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5560 2024-05-26 08:31:57.084580 steamleaderboards-1.1.0/steamleaderboards/__init__.py
+-rw-r--r--   0        0        0     2187 2024-05-26 08:28:43.829577 steamleaderboards-1.1.0/steamleaderboards/__main__.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 steamleaderboards-1.1.0/PKG-INFO
```

### Comparing `steamleaderboards-1.0.0/LICENSE.txt` & `steamleaderboards-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `steamleaderboards-1.0.0/README.md` & `steamleaderboards-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 # `steamleaderboards`
 
 Retrieve and parse Steam leaderboards
 
 </div>
 
+## Links
+
+[![PyPI](https://img.shields.io/pypi/v/steamleaderboards)](https://pypi.org/project/steamleaderboards)
+
 ## History
 
 It was created with the Isaac Daily Run scoreboards in mind, but it can be used for other games that have a public leaderboard as well.
 
 ## Usage
 
 ### In code
```

### Comparing `steamleaderboards-1.0.0/pyproject.toml` & `steamleaderboards-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steamleaderboards"
-version = "1.0.0"
+version = "1.1.0"
 description = "Retrieve and parse Steam leaderboards"
 authors = ["Stefano Pigozzi <me@steffo.eu>"]
 maintainers = ["Stefano Pigozzi <me@steffo.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Steffo99/steamleaderboards"
 keywords = ["steam", "leaderboards", "csv", "xml", "valve"]
```

### Comparing `steamleaderboards-1.0.0/steamleaderboards/__init__.py` & `steamleaderboards-1.1.0/steamleaderboards/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from bs4 import BeautifulSoup
 import typing
+import time
 
 
 class LeaderboardGroup:
     def __init__(self, app_id):
         xml = requests.get(f"https://steamcommunity.com/stats/{app_id}/leaderboards/?xml=1")
         _bs = BeautifulSoup(xml.content, features="lxml-xml")
         self.leaderboards = []
@@ -48,21 +49,21 @@
         self.name = soup.find("name").text
         self.display_name = soup.display_name.text
         self.entries = int(soup.entries.text)
         self.sort_method = int(soup.sortmethod.text)
         self.display_type = int(soup.displaytype.text)
         self.app_id = app_id
 
-    def full(self) -> "Leaderboard":
-        return Leaderboard(protoleaderboard=self)
+    def full(self, *args, **kwargs) -> "Leaderboard":
+        return Leaderboard(*args, **kwargs, protoleaderboard=self)
 
 
 class Leaderboard:
     # noinspection PyMissingConstructor
-    def __init__(self, app_id=None, lbid=None, *, protoleaderboard=None):
+    def __init__(self, app_id=None, lbid=None, *, protoleaderboard=None, limit=None, delay=None):
         if protoleaderboard:
             self.url = protoleaderboard.url
             self.lbid = protoleaderboard.lbid
             self.name = protoleaderboard.name
             self.display_name = protoleaderboard.display_name
             self.entries = protoleaderboard.entries
             self.sort_method = protoleaderboard.sort_method
@@ -75,29 +76,35 @@
             self.name = None
             self.display_name = None
             self.entries = None
             self.sort_method = None
             self.display_type = None
         else:
             raise ValueError("No app_id, lbid or protoleaderboard specified")
+        if limit is None:
+            limit = 5000
+        if delay is None:
+            delay = 0.5
         next_request_url = self.url
         self.entries = []
         while next_request_url:
             xml = requests.get(next_request_url)
             _bs = BeautifulSoup(xml.content, features="lxml-xml")
             for entry in _bs.find_all("entry"):
                 self.entries.append(Entry(entry))
-            if _bs.response.entryend:
-                entry_end = int(_bs.response.entryend.text)
-                if entry_end < int(_bs.response.totalleaderboardentries.text):
-                    next_request_url = f"https://steamcommunity.com/stats/{self.app_id}/leaderboards/{self.lbid}/?xml=1&start={entry_end + 1}"
-                else:
+                if len(self.entries) >= limit:
                     next_request_url = None
+                    break
             else:
-                next_request_url = None
+                try:
+                    next_request_url = _bs.find_all("nextRequestURL")[0].text
+                except IndexError:
+                    next_request_url = None
+                else:
+                    time.sleep(delay)
 
     def __repr__(self):
         if self.name:
             return f'<Leaderboard "{self.name}" for {self.app_id} with {len(self.entries)}>'
         else:
             return f'<Leaderboard [{self.lbid}] for {self.app_id} with {len(self.entries)}>'
```

### Comparing `steamleaderboards-1.0.0/steamleaderboards/__main__.py` & `steamleaderboards-1.1.0/steamleaderboards/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import argparse
 import importlib.metadata
 import pathlib
 import sys
+import time
 from . import LeaderboardGroup, ProtoLeaderboard, Leaderboard, Entry
 
 
 parser = argparse.ArgumentParser(
 	description="Retrieve scoreboards for a specific Steam game"
 )
 
 parser.add_argument("-o", "--output-dir", dest="output_dir", help="The directory where downloaded leaderboards should be stored in.", type=pathlib.Path)
 parser.add_argument("app_id", type=int, nargs="+")
+parser.add_argument("-d", "--request-delay", dest="request_delay", help="How long to wait between two requests to the scoreboard API.", type=float, default=0.5)
+parser.add_argument("-l", "--limit", dest="limit", help="How many entries to retrieve for each scoreboard.", type=int, default=5000)
 parser.add_argument("-V", "--version", action="version", version=importlib.metadata.version("steamleaderboards"))
 
 def main():
 	args = parser.parse_args()
 
 	output_dir: pathlib.Path = (args.output_dir or pathlib.Path(".")).absolute()
 	if output_dir.exists() and not output_dir.is_dir():
@@ -27,18 +30,20 @@
 		print(f"using output directory: {output_dir}", file=sys.stderr)
 
 	for app_id in args.app_id:
 		print(f"fetching leaderboards for: {app_id}", file=sys.stderr)
 		lg: LeaderboardGroup = LeaderboardGroup(app_id)
 		for proto in lg.leaderboards:
 			print(f"fetching full leaderboard: {app_id} {proto.name}", file=sys.stderr)
-			full: Leaderboard = proto.full()
+			full: Leaderboard = proto.full(limit=args.limit, delay=args.request_delay)
 			with open(output_dir.joinpath(f"{full.app_id}_{full.name}.csv"), mode="w") as file:
 				file.write(f"rank,steam_id,score,ugcid,details\n")
 				for entry in full.entries:
 					file.write(f"{entry.rank!r},{entry.steam_id!r},{entry.score!r},{entry.ugcid!r},{entry.details!r}\n")
+			print(f"done, resting for {args.request_delay} seconds", file=sys.stderr)
+			time.sleep(args.request_delay)
 		if len(lg.leaderboards) == 0:
 			print(f"game has no leaderboards", file=sys.stderr)
 
 
 if __name__ == "__main__":
 	main()
```

### Comparing `steamleaderboards-1.0.0/PKG-INFO` & `steamleaderboards-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamleaderboards
-Version: 1.0.0
+Version: 1.1.0
 Summary: Retrieve and parse Steam leaderboards
 Home-page: https://github.com/Steffo99/steamleaderboards
 License: MIT
 Keywords: steam,leaderboards,csv,xml,valve
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
@@ -35,14 +35,18 @@
 
 # `steamleaderboards`
 
 Retrieve and parse Steam leaderboards
 
 </div>
 
+## Links
+
+[![PyPI](https://img.shields.io/pypi/v/steamleaderboards)](https://pypi.org/project/steamleaderboards)
+
 ## History
 
 It was created with the Isaac Daily Run scoreboards in mind, but it can be used for other games that have a public leaderboard as well.
 
 ## Usage
 
 ### In code
```

