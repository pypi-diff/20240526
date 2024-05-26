# Comparing `tmp/lyriks-0.2.3.tar.gz` & `tmp/lyriks-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.2.3.tar", last modified: Sat May 25 21:53:21 2024, max compression
+gzip compressed data, was "lyriks-0.2.4.tar", last modified: Sun May 26 00:42:58 2024, max compression
```

## Comparing `lyriks-0.2.3.tar` & `lyriks-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.049552 lyriks-0.2.3/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:53:21.049552 lyriks-0.2.3/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 21:52:06.000000 lyriks-0.2.3/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.046218 lyriks-0.2.3/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.3/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-25 21:52:06.000000 lyriks-0.2.3/lyriks/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.3/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.3/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     7546 2024-05-25 21:49:30.000000 lyriks-0.2.3/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     3010 2024-05-25 20:47:16.000000 lyriks-0.2.3/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.049552 lyriks-0.2.3/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 21:52:06.000000 lyriks-0.2.3/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 21:53:21.049552 lyriks-0.2.3/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-26 00:42:58.369047 lyriks-0.2.4/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-26 00:41:30.000000 lyriks-0.2.4/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.4/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-26 00:41:30.000000 lyriks-0.2.4/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.4/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.4/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     8073 2024-05-26 00:41:08.000000 lyriks-0.2.4/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     3114 2024-05-26 00:41:08.000000 lyriks-0.2.4/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-26 00:41:30.000000 lyriks-0.2.4/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-26 00:42:58.369047 lyriks-0.2.4/setup.cfg
```

### Comparing `lyriks-0.2.3/PKG-INFO` & `lyriks-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.3-py3-none-any.whl
+pip install dist/lyriks-0.2.4-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.3/README.md` & `lyriks-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.3-py3-none-any.whl
+pip install dist/lyriks-0.2.4-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.3/lyriks/__init__.py` & `lyriks-0.2.4/lyriks/__init__.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.3/lyriks/cli.py` & `lyriks-0.2.4/lyriks/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from pathlib import Path
 
 PROGNAME = 'lyriks'
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog=PROGNAME, description='A command line tool that fetches lyrics from Genie.')
     path_help = f"""
                 The path to the music collection.
                 {PROGNAME} will recursively search for music files in this directory.
```

### Comparing `lyriks-0.2.3/lyriks/genie_client.py` & `lyriks-0.2.4/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.3/lyriks/lyrics.py` & `lyriks-0.2.4/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.3/lyriks/lyrics_fetcher.py` & `lyriks-0.2.4/lyriks/lyrics_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,30 +45,27 @@
             return False
 
         tags = file.tags
         if (TITLE_TAG not in tags or ALBUM_TAG not in tags or TRACKNUMBER_TAG not in tags or
                 MB_RGID_TAG not in tags or MB_RTID_TAG not in tags):
             return False
 
-        title = tags[TITLE_TAG][0]
-        album = tags[ALBUM_TAG][0]
+        title = tags[TITLE_TAG][0] or 'Unknown title'
+        album = tags[ALBUM_TAG][0] or 'Unknown album'
         track_number = int(tags[TRACKNUMBER_TAG][0].split('/')[0])
         rg_mbid = tags[MB_RGID_TAG][0]
         track_mbid = tags[MB_RTID_TAG][0]
 
+        # Handle empty MBIDs
+        if not rg_mbid or not track_mbid:
+            return False
+
         # Check artist for Genie URL
-        if self.check_artist and MB_RAID_TAG in tags and ALBUMARTIST_TAG in tags:
-            albumartist_mbid = tags[MB_RAID_TAG][0]
-            albumartist = tags[ALBUMARTIST_TAG][0]
-            artist = self.get_artist(albumartist_mbid, albumartist)
-            if artist and not artist.has_genie_url:
-                if artist.id not in self.missing_artists:
-                    print(f'No Genie URL found for artist {artist.name} [{artist.id}]')
-                    self.missing_artists.add(artist.id)
-                return False
+        if self.check_artist and not self.has_artist_genie_url(tags):
+            return False
 
         # Resolve release for the track
         track_release = self.get_release(track_mbid, album)
         if not track_release:
             return False
 
         # Resolve Genie album
@@ -100,14 +97,37 @@
                 print(' - not writing static lyrics, timed lyrics already exist')
             else:
                 print(f' - writing to {static_lyrics_file}')
                 lyrics.write_to_file(static_lyrics_file)
 
         return True
 
+    def has_artist_genie_url(self, tags):
+        """
+        Check if the artist has a Genie URL.
+        :return: True if we're unable to check or if this artist has a Genie URL, False otherwise.
+        """
+        if MB_RAID_TAG not in tags or ALBUMARTIST_TAG not in tags:
+            return True
+
+        albumartist_mbid = tags[MB_RAID_TAG][0]
+        if not albumartist_mbid:  # handle empty MBID
+            return True
+
+        albumartist = tags[ALBUMARTIST_TAG][0] or 'Unknown artist'
+        artist = self.get_artist(albumartist_mbid, albumartist)
+        if not artist or artist.has_genie_url:
+            return True
+
+        if artist.id not in self.missing_artists:
+            print(f'No Genie URL found for artist {artist.name} [{artist.id}]')
+            self.missing_artists.add(artist.id)
+
+        return False
+
     def get_artist(self, artist_mbid: str, artist_name: str) -> Artist | None:
         if artist_mbid in self.artist_cache:
             return self.artist_cache[artist_mbid]
 
         print(f'Fetching artist info for {artist_name}', end='')
 
         artist = get_artist(artist_mbid)
```

### Comparing `lyriks-0.2.3/lyriks/mb_client.py` & `lyriks-0.2.4/lyriks/mb_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,18 @@
     response = requests.get(artist_url, headers={'User-Agent': USER_AGENT, 'Accept': 'application/json'})
     try:
         response_json = response.json()
     except JSONDecodeError:
         print(f'Error: could not fetch artist data for {artist_mbid}')
         return None
 
+    if 'error' in response_json:
+        print(f'Error: {response_json['error']}')
+        return None
+
     return Artist(response_json)
 
 
 def get_releases(browse_url: str) -> list[Release]:
     handle_rate_limit()
 
     response = requests.get(browse_url, headers={'User-Agent': USER_AGENT, 'Accept': 'application/json'})
```

### Comparing `lyriks-0.2.3/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.4/lyriks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.3-py3-none-any.whl
+pip install dist/lyriks-0.2.4-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.3/pyproject.toml` & `lyriks-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.2.3"
+version = "0.2.4"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

