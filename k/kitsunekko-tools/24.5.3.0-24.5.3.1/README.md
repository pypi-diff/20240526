# Comparing `tmp/kitsunekko_tools-24.5.3.0.tar.gz` & `tmp/kitsunekko_tools-24.5.3.1.tar.gz`

## Comparing `kitsunekko_tools-24.5.3.0.tar` & `kitsunekko_tools-24.5.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/format.sh
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/workflows/black.yml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__main__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__version__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/common.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/config.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/consts.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/file_downloader.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/ignore.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/mega_upload.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/__init__.py
--rw-r--r--   0        0        0     8859 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/download.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/file_entry.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/rate_limit.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/root_directory.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/__init__.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/download.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/parse.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/types.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/test_directory.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/test_parser.py
--rw-r--r--   0        0        0  1070007 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/entries_search_anime_response.json
--rw-r--r--   0        0        0   444457 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/entries_search_dramas_response.json
--rw-r--r--   0        0        0   663796 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/main_dir_page.html
--rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/subs_page.html
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/LICENSE
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/pyproject.toml
--rw-r--r--   0        0        0    42329 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/format.sh
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/__main__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/__version__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/common.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/config.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/consts.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/file_downloader.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/ignore.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/mega_upload.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/__init__.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/download.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/file_entry.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/rate_limit.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/root_directory.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/__init__.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/download.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/parse.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/types.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/test_directory.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/test_parser.py
+-rw-r--r--   0        0        0  1070007 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/data/entries_search_anime_response.json
+-rw-r--r--   0        0        0   444457 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/data/entries_search_dramas_response.json
+-rw-r--r--   0        0        0   663796 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/data/main_dir_page.html
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/tests/data/subs_page.html
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/LICENSE
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/pyproject.toml
+-rw-r--r--   0        0        0    42329 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.1/PKG-INFO
```

### Comparing `kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/config.yml` & `kitsunekko_tools-24.5.3.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/.github/workflows/ci-cd.yml` & `kitsunekko_tools-24.5.3.1/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/__main__.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/config.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
 
 import dataclasses
 import datetime
 import functools
 import io
+import os
 import os.path
 import pathlib
 import tomllib
 import typing
-import os
+
 from kitsunekko_tools.common import KitsuException
 from kitsunekko_tools.consts import *
 
 DEFAULT_HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:108.0) Gecko/20100101 Firefox/108.0",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
     "Accept-Charset": "ISO-8859-1,utf-8;q=0.7,*;q=0.3",
@@ -95,18 +96,18 @@
     return datetime.timedelta(**{time_unit: int(period)})
 
 
 @dataclasses.dataclass(frozen=True)
 class KitsuConfig:
     destination: pathlib.Path = pathlib.Path.home() / "kitsunekko"
     proxy: str | None = "socks5://127.0.0.1:9050"
-    download_root: str = "https://kitsunekko.net/dirlist.php?dir=subtitles/japanese/"
+    download_root: str = "https://kitsunekko.net/dirlist.php?dir=subtitles/japanese/"  # scrap target
     timeout: int = 120
     skip_older: datetime.timedelta = datetime.timedelta(days=30)  # 30 days
-    api_url: str = ""  # URL of a subtitle server's API. Normally looks like 'https://example.com/api'.
+    api_url: str = "https://kitsunekko.net"  # URL of a subtitle server. Normally looks like 'https://example.com'.
     api_key: str = ""  # API key of the subtitle server
     allowed_file_types: frozenset[str] = dataclasses.field(
         default_factory=lambda: frozenset(["ssa", "ass", "srt", "zip", "rar", "7z"])
     )
     headers: dict[str, str] = dataclasses.field(default_factory=lambda: DEFAULT_HEADERS.copy())
 
     @classmethod
```

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/file_downloader.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/file_downloader.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/ignore.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/ignore.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/mega_upload.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/mega_upload.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/download.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         return self.remote_dir.name
 
     @classmethod
     def from_remote(cls, remote_dir: ApiDirectoryEntry, config: KitsuConfig):
         return cls(
             remote_dir=remote_dir,
             meta_file_path=pathlib.Path(config.destination / remote_dir.name / ".kitsuinfo.json"),
-            dir_listing_url=f"{config.api_url}/entries/{remote_dir.entry_id}/files",
+            dir_listing_url=f"{config.api_url}/api/entries/{remote_dir.entry_id}/files",
         )
 
     def should_visit_directory(self) -> bool:
         return not self.meta_file_path.is_file() or self.is_remote_newer()
 
     def is_remote_newer(self) -> bool:
         with open(self.meta_file_path) as f:
@@ -188,15 +188,15 @@
     def _construct_search_args_str(self, is_anime: bool) -> str:
         args: dict[str, object] = {"anime": is_anime}
         if not self._full_sync:
             args["after"] = (self._now - self._config.skip_older).strftime("%s")
         return "&".join(f"{key}={str(value).lower()}" for key, value in args.items())
 
     def get_search_url(self, is_anime: bool) -> str:
-        return f"{self._config.api_url}/entries/search?{self._construct_search_args_str(is_anime)}"
+        return f"{self._config.api_url}/api/entries/search?{self._construct_search_args_str(is_anime)}"
 
     async def _run_tasks(self) -> None:
         while self._tasks:
             print(f"Running task.")
             try:
                 await self._tasks.popleft()
             except (KitsuConnectionError, ApiBadStatusError) as e:
```

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/file_entry.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/file_entry.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/rate_limit.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/rate_limit.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/root_directory.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/api_access/root_directory.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/download.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/download.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/parse.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/parse.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/types.py` & `kitsunekko_tools-24.5.3.1/kitsunekko_tools/scrapper/types.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/tests/test_directory.py` & `kitsunekko_tools-24.5.3.1/tests/test_directory.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 def test_shows_in_root_dir(search_response_json: Sequence[ApiDirectoryDict]) -> None:
     dirs: list[ApiDirectoryEntry] = [*iter_catalog_directories(search_response_json)]
     assert len(dirs) > 0
     assert all(dir_.entry_id > 0 for dir_ in dirs)
     assert all(dir_.name for dir_ in dirs)
     date_threshold = datetime.datetime.fromisoformat("2012-07-15 20:21:54+00:00")
-    assert all(datetime.datetime.fromisoformat(dir_.last_modified) > date_threshold for dir_ in dirs)
+    assert all(dir_.last_modified > date_threshold for dir_ in dirs)
```

### Comparing `kitsunekko_tools-24.5.3.0/tests/test_parser.py` & `kitsunekko_tools-24.5.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/tests/data/entries_search_anime_response.json` & `kitsunekko_tools-24.5.3.1/tests/data/entries_search_anime_response.json`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/tests/data/entries_search_dramas_response.json` & `kitsunekko_tools-24.5.3.1/tests/data/entries_search_dramas_response.json`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/tests/data/main_dir_page.html` & `kitsunekko_tools-24.5.3.1/tests/data/main_dir_page.html`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/tests/data/subs_page.html` & `kitsunekko_tools-24.5.3.1/tests/data/subs_page.html`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/LICENSE` & `kitsunekko_tools-24.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/README.md` & `kitsunekko_tools-24.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/pyproject.toml` & `kitsunekko_tools-24.5.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.5.3.0/PKG-INFO` & `kitsunekko_tools-24.5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitsunekko-tools
-Version: 24.5.3.0
+Version: 24.5.3.1
 Summary: A set of scripts for creating a local kitsunekko mirror.
 Author-email: Ren Tatsumoto <tatsu@autistici.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

