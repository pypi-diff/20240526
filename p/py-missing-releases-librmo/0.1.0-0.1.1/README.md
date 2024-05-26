# Comparing `tmp/py_missing_releases_librmo-0.1.0.tar.gz` & `tmp/py_missing_releases_librmo-0.1.1.tar.gz`

## Comparing `py_missing_releases_librmo-0.1.0.tar` & `py_missing_releases_librmo-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/__init__.py
--rwxr-xr-x   0        0        0     1336 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/_database.py
--rwxr-xr-x   0        0        0      606 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/_utils.py
--rwxr-xr-x   0        0        0     3964 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/missing_releases.py
--rwxr-xr-x   0        0        0     3086 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/README.md
--rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      473 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/.vscode/launch.json
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/__init__.py
+-rwxr-xr-x   0        0        0     1336 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/_database.py
+-rwxr-xr-x   0        0        0      606 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/_utils.py
+-rwxr-xr-x   0        0        0     4199 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/missing_releases.py
+-rwxr-xr-x   0        0        0     3086 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/README.md
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 py_missing_releases_librmo-0.1.1/PKG-INFO
```

### Comparing `py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/_database.py` & `py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/_database.py`

 * *Files identical despite different names*

### Comparing `py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/_utils.py` & `py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/_utils.py`

 * *Files identical despite different names*

### Comparing `py_missing_releases_librmo-0.1.0/src/py_missing_releases_librmo/missing_releases.py` & `py_missing_releases_librmo-0.1.1/src/py_missing_releases_librmo/missing_releases.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 @dataclass
 class Release():
     name: str
     artist: AlbumArtist
     mb_id: str
     url: str
+    year: int
 
 
 class MissingReleases():
 
     librmo_config_dir: str = os.path.join(
         str(Path.home()), ".config/librmo")
     librmo_db_name: str = 'media.db'
@@ -71,16 +72,20 @@
                 if 'secondary-types' in r:
                     if 'Live' in r['secondary-types']:
                         continue
                     if 'Compilation' in r['secondary-types']:
                         continue
                     if 'Demo' in r['secondary-types']:
                         continue
+                release_year = 0
+                if 'first-release-date' in r:
+                    release_year = str(
+                        r['first-release-date']).split('-', 1)[0]
                 self.full_album_releases.append(
-                    Release(name=r['title'], mb_id=r['id'], url='', artist=a))
+                    Release(name=r['title'], mb_id=r['id'], url='', artist=a, year=release_year))
         # self._debug(self.full_album_releases)
 
     def _get_albumartists(self):
         self.albumartists = []
         for a in self.known_album_releases:
             response = self.mb.get_release_group(a.mb_id)
             if response.error is True:
@@ -100,21 +105,21 @@
         # self._debug(self.albumartists)
 
     def _get_album_groups(self):
         self.known_album_releases = []
         album_groups = self.db.get_all_album_groups()
         for a in album_groups:
             self.known_album_releases.append(
-                Release(name=a[1], mb_id=a[0], url='', artist=None))
+                Release(name=a[1], mb_id=a[0], url='', artist=None, year=0))
         # self._debug(self.known_album_releases)
 
     def _connect_librmo(self):
         self.db = DB(os.path.join(self.librmo_config_dir, self.librmo_db_name))
 
-    def execute(self) -> list:
+    def execute(self) -> list[Release]:
         self._connect_librmo()
         self._get_album_groups()
         self._get_albumartists()
         self._query_album_releases()
         self._compare_releases()
         return self.missing_releases
```

### Comparing `py_missing_releases_librmo-0.1.0/.gitignore` & `py_missing_releases_librmo-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_missing_releases_librmo-0.1.0/LICENSE` & `py_missing_releases_librmo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_missing_releases_librmo-0.1.0/README.md` & `py_missing_releases_librmo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_missing_releases_librmo-0.1.0/pyproject.toml` & `py_missing_releases_librmo-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 [project]
 name = "py_missing_releases_librmo"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Samuel Shiels" },
 ]
 description = "Uses information stored in librmo to discover missing album releases from your music artists"
 readme = "README.md"
 requires-python = ">=3.11.5"
 classifiers = [
```

### Comparing `py_missing_releases_librmo-0.1.0/PKG-INFO` & `py_missing_releases_librmo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py_missing_releases_librmo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uses information stored in librmo to discover missing album releases from your music artists
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

