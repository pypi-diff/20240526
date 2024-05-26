# Comparing `tmp/lyriks-0.2.4.tar.gz` & `tmp/lyriks-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.2.4.tar", last modified: Sun May 26 00:42:58 2024, max compression
+gzip compressed data, was "lyriks-0.2.5.tar", last modified: Sun May 26 01:03:17 2024, max compression
```

## Comparing `lyriks-0.2.4.tar` & `lyriks-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-26 00:42:58.369047 lyriks-0.2.4/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-26 00:41:30.000000 lyriks-0.2.4/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.4/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-26 00:41:30.000000 lyriks-0.2.4/lyriks/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.4/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.4/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     8073 2024-05-26 00:41:08.000000 lyriks-0.2.4/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     3114 2024-05-26 00:41:08.000000 lyriks-0.2.4/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 00:42:58.369047 lyriks-0.2.4/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-26 00:42:58.000000 lyriks-0.2.4/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-26 00:41:30.000000 lyriks-0.2.4/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-26 00:42:58.369047 lyriks-0.2.4/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 01:03:17.514945 lyriks-0.2.5/
+-rw-r--r--   0 max       (1000) max       (1000)     1959 2024-05-26 01:03:17.514945 lyriks-0.2.5/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-26 01:02:52.000000 lyriks-0.2.5/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 01:03:17.514945 lyriks-0.2.5/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.5/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-26 01:02:52.000000 lyriks-0.2.5/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.5/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.5/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     8073 2024-05-26 00:41:08.000000 lyriks-0.2.5/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     3114 2024-05-26 01:00:26.000000 lyriks-0.2.5/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-26 01:03:17.514945 lyriks-0.2.5/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1959 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-26 01:03:17.000000 lyriks-0.2.5/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      531 2024-05-26 01:02:52.000000 lyriks-0.2.5/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-26 01:03:17.514945 lyriks-0.2.5/setup.cfg
```

### Comparing `lyriks-0.2.4/PKG-INFO` & `lyriks-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.4
+Version: 0.2.5
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.28
 Requires-Dist: mutagen>=1.45
 
 # lyriks
 
 A command line tool that fetches lyrics from [Genie](https://www.genie.co.kr/).
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.4-py3-none-any.whl
+pip install dist/lyriks-0.2.5-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.4/README.md` & `lyriks-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.4-py3-none-any.whl
+pip install dist/lyriks-0.2.5-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.4/lyriks/__init__.py` & `lyriks-0.2.5/lyriks/__init__.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.4/lyriks/cli.py` & `lyriks-0.2.5/lyriks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from pathlib import Path
 
 PROGNAME = 'lyriks'
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog=PROGNAME, description='A command line tool that fetches lyrics from Genie.')
     path_help = f"""
                 The path to the music collection.
                 {PROGNAME} will recursively search for music files in this directory.
```

### Comparing `lyriks-0.2.4/lyriks/genie_client.py` & `lyriks-0.2.5/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.4/lyriks/lyrics.py` & `lyriks-0.2.5/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.4/lyriks/lyrics_fetcher.py` & `lyriks-0.2.5/lyriks/lyrics_fetcher.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.4/lyriks/mb_client.py` & `lyriks-0.2.5/lyriks/mb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     try:
         response_json = response.json()
     except JSONDecodeError:
         print(f'Error: could not fetch artist data for {artist_mbid}')
         return None
 
     if 'error' in response_json:
-        print(f'Error: {response_json['error']}')
+        print(f'Error: {response_json["error"]}')
         return None
 
     return Artist(response_json)
 
 
 def get_releases(browse_url: str) -> list[Release]:
     handle_rate_limit()
```

### Comparing `lyriks-0.2.4/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.5/lyriks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.4
+Version: 0.2.5
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.28
 Requires-Dist: mutagen>=1.45
 
 # lyriks
 
 A command line tool that fetches lyrics from [Genie](https://www.genie.co.kr/).
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.4-py3-none-any.whl
+pip install dist/lyriks-0.2.5-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.4/pyproject.toml` & `lyriks-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "lyriks"
-version = "0.2.4"
+version = "0.2.5"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "requests>=2.28",
     "mutagen>=1.45",
 ]
 
 [project.scripts]
 lyriks = "lyriks:main"
```

