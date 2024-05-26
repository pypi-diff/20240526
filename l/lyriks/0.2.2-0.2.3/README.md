# Comparing `tmp/lyriks-0.2.2.tar.gz` & `tmp/lyriks-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.2.2.tar", last modified: Sat May 25 21:09:37 2024, max compression
+gzip compressed data, was "lyriks-0.2.3.tar", last modified: Sat May 25 21:53:21 2024, max compression
```

## Comparing `lyriks-0.2.2.tar` & `lyriks-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.966672 lyriks-0.2.2/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:09:37.966672 lyriks-0.2.2/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 21:07:48.000000 lyriks-0.2.2/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.963339 lyriks-0.2.2/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.2/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-25 21:07:48.000000 lyriks-0.2.2/lyriks/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.2/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.2/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     7123 2024-05-25 21:06:54.000000 lyriks-0.2.2/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     3010 2024-05-25 20:47:16.000000 lyriks-0.2.2/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.966672 lyriks-0.2.2/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 21:07:48.000000 lyriks-0.2.2/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 21:09:37.966672 lyriks-0.2.2/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.049552 lyriks-0.2.3/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:53:21.049552 lyriks-0.2.3/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 21:52:06.000000 lyriks-0.2.3/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.046218 lyriks-0.2.3/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.3/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-25 21:52:06.000000 lyriks-0.2.3/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.3/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.3/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     7546 2024-05-25 21:49:30.000000 lyriks-0.2.3/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     3010 2024-05-25 20:47:16.000000 lyriks-0.2.3/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:53:21.049552 lyriks-0.2.3/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 21:53:21.000000 lyriks-0.2.3/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 21:52:06.000000 lyriks-0.2.3/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 21:53:21.049552 lyriks-0.2.3/setup.cfg
```

### Comparing `lyriks-0.2.2/PKG-INFO` & `lyriks-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.2
+Version: 0.2.3
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
-pip install dist/lyriks-0.2.2-py3-none-any.whl
+pip install dist/lyriks-0.2.3-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.2/README.md` & `lyriks-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.2-py3-none-any.whl
+pip install dist/lyriks-0.2.3-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.2/lyriks/__init__.py` & `lyriks-0.2.3/lyriks/__init__.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.2/lyriks/cli.py` & `lyriks-0.2.3/lyriks/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from pathlib import Path
 
 PROGNAME = 'lyriks'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog=PROGNAME, description='A command line tool that fetches lyrics from Genie.')
     path_help = f"""
                 The path to the music collection.
                 {PROGNAME} will recursively search for music files in this directory.
```

### Comparing `lyriks-0.2.2/lyriks/genie_client.py` & `lyriks-0.2.3/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.2/lyriks/lyrics.py` & `lyriks-0.2.3/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.2/lyriks/lyrics_fetcher.py` & `lyriks-0.2.3/lyriks/lyrics_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 
 from .genie_client import fetch_genie_album_song_ids, GenieSong, fetch_lyrics
 from .mb_client import Artist, Release, get_artist, get_release_by_track, get_releases_by_release_group
 
 TITLE_TAG = 'title'
 ALBUM_TAG = 'album'
 TRACKNUMBER_TAG = 'tracknumber'
+ALBUMARTIST_TAG = 'albumartist'
 MB_RGID_TAG = 'musicbrainz_releasegroupid'
 MB_RTID_TAG = 'musicbrainz_releasetrackid'
+MB_RAID_TAG = 'musicbrainz_albumartistid'
 
 
 class LyricsFetcher:
     def __init__(self, check_artist: bool = False, dry_run: bool = False, force: bool = False):
         self.check_artist = check_artist
         self.dry_run = dry_run
         self.force = force
-        self.artist_cache = {}
-        self.release_cache = {}
+        self.artist_cache: dict[str, Artist] = {}
+        self.release_cache: dict[str, Release] = {}
         self.genie_cache = {}
-        self.missing_artists = set()
-        self.missing_releases = set()
+        self.missing_artists: set[str] = set()
+        self.missing_releases: set[str] = set()
 
     def fetch_lyrics(self, filename: str) -> bool:
         basename = filename.rsplit('.', 1)[0]
         timed_lyrics_file = f'{basename}.lrc'
         static_lyrics_file = f'{basename}.txt'
 
         has_timed_lyrics = path.exists(timed_lyrics_file)
@@ -49,30 +51,30 @@
 
         title = tags[TITLE_TAG][0]
         album = tags[ALBUM_TAG][0]
         track_number = int(tags[TRACKNUMBER_TAG][0].split('/')[0])
         rg_mbid = tags[MB_RGID_TAG][0]
         track_mbid = tags[MB_RTID_TAG][0]
 
+        # Check artist for Genie URL
+        if self.check_artist and MB_RAID_TAG in tags and ALBUMARTIST_TAG in tags:
+            albumartist_mbid = tags[MB_RAID_TAG][0]
+            albumartist = tags[ALBUMARTIST_TAG][0]
+            artist = self.get_artist(albumartist_mbid, albumartist)
+            if artist and not artist.has_genie_url:
+                if artist.id not in self.missing_artists:
+                    print(f'No Genie URL found for artist {artist.name} [{artist.id}]')
+                    self.missing_artists.add(artist.id)
+                return False
+
         # Resolve release for the track
         track_release = self.get_release(track_mbid, album)
         if not track_release:
             return False
 
-        # Check artist for Genie URL
-        if self.check_artist:
-            artist_info = track_release.artist_credit[0]['artist']
-            artist_mbid = artist_info['id']
-            if artist_mbid not in self.artist_cache:  # only check each artist once
-                artist = self.get_artist(artist_mbid, artist_info['name'])
-                if artist and not artist.has_genie_url:
-                    print(f'No Genie URL found for artist {artist.name} [{artist.id}]')
-                    self.missing_artists.add(artist)
-                    return False
-
         # Resolve Genie album
         songs = self.get_genie_album(track_release, rg_mbid)
         if not songs or track_release.get_track_count() != len(songs):
             return False
 
         print(f'Fetching lyrics for {title}', end='')
 
@@ -171,32 +173,36 @@
             if rg_release.get_track_count() != release.get_track_count():
                 continue
             album_id = rg_release.get_genie_album_id()
             if album_id is not None:
                 return album_id
 
         print(f'No Genie URL found for release {release.title} [{release.id}]')
-        self.missing_releases.add(release)
+        self.missing_releases.add(release.id)
 
         return None
 
     def write_report(self, file: str | PathLike[str]):
         with open(file, 'w') as f:
             f.write('<!DOCTYPE html>\n')
             f.write('<html>\n')
             f.write('<head><title>lyriks report</title></head>\n')
             f.write('<body>\n')
             f.write('<h1>lyriks report</h1>\n')
             f.write('<h2>Artists missing Genie URLs</h2>\n')
             f.write('<ul>\n')
-            for artist in self.missing_artists:
-                url = f'https://musicbrainz.org/artist/{artist.id}'
-                f.write(f'<li><a href="{url}">{html.escape(artist.name)}</a></li>\n')
+            for artist_mbid in self.missing_artists:
+                url = f'https://musicbrainz.org/artist/{artist_mbid}'
+                artist = self.artist_cache[artist_mbid]
+                artist_name = artist.name if artist else 'Unknown artist'
+                f.write(f'<li><a href="{url}">{html.escape(artist_name)}</a></li>\n')
             f.write('</ul>\n')
             f.write('<h2>Releases missing Genie URLs</h2>\n')
             f.write('<ul>\n')
-            for release in self.missing_releases:
-                url = f'https://musicbrainz.org/release/{release.id}'
-                f.write(f'<li><a href="{url}">{html.escape(release.title)}</a></li>\n')
+            for release_mbid in self.missing_releases:
+                url = f'https://musicbrainz.org/release/{release_mbid}'
+                release = self.release_cache[release_mbid]
+                release_name = release.title if release else 'Unknown release'
+                f.write(f'<li><a href="{url}">{html.escape(release_name)}</a></li>\n')
             f.write('</ul>\n')
             f.write('</body>\n')
             f.write('</html>')
```

### Comparing `lyriks-0.2.2/lyriks/mb_client.py` & `lyriks-0.2.3/lyriks/mb_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.2/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.3/lyriks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.2
+Version: 0.2.3
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
-pip install dist/lyriks-0.2.2-py3-none-any.whl
+pip install dist/lyriks-0.2.3-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.2/pyproject.toml` & `lyriks-0.2.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.2.2"
+version = "0.2.3"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

