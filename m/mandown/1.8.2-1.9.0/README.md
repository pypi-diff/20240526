# Comparing `tmp/mandown-1.8.2.tar.gz` & `tmp/mandown-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.8.2.tar", max compression
+gzip compressed data, was "mandown-1.9.0.tar", max compression
```

## Comparing `mandown-1.8.2.tar` & `mandown-1.9.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.8.2/LICENSE
--rw-r--r--   0        0        0     3885 2024-05-12 17:51:49.558004 mandown-1.8.2/README.md
--rw-r--r--   0        0        0      542 2024-05-14 15:31:23.242152 mandown-1.8.2/mandown/__init__.py
--rw-r--r--   0        0        0    11781 2024-05-13 20:08:43.671607 mandown-1.8.2/mandown/api.py
--rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.8.2/mandown/base.py
--rw-r--r--   0        0        0    17083 2024-05-14 15:30:30.062508 mandown-1.8.2/mandown/cli.py
--rw-r--r--   0        0        0     2562 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/comic.py
--rw-r--r--   0        0        0      705 2024-05-13 20:10:08.695482 mandown-1.8.2/mandown/convert_utils.py
--rw-r--r--   0        0        0     5543 2024-03-08 17:11:50.450985 mandown-1.8.2/mandown/io.py
--rw-r--r--   0        0        0     5095 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4064 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/processor/ops.py
--rw-r--r--   0        0        0     1597 2024-03-08 17:11:50.448985 mandown-1.8.2/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1505 2024-05-12 17:51:49.558004 mandown-1.8.2/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2016 2024-03-08 17:11:50.448985 mandown-1.8.2/mandown/sources/base_source.py
--rw-r--r--   0        0        0     3301 2024-05-12 16:09:43.070512 mandown-1.8.2/mandown/sources/source_blogtruyenmoi.py
--rw-r--r--   0        0        0     4476 2024-05-12 17:51:49.558004 mandown-1.8.2/mandown/sources/source_kuaikanmanhua.py
--rw-r--r--   0        0        0     5045 2024-03-08 17:11:50.450985 mandown-1.8.2/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2535 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2641 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3658 2024-03-08 17:11:50.450985 mandown-1.8.2/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3044 2024-03-08 17:11:50.451985 mandown-1.8.2/mandown/sources/source_manhuaes.py
--rw-r--r--   0        0        0     3567 2023-07-14 02:43:47.054901 mandown-1.8.2/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     5154 2024-03-08 17:11:50.451985 mandown-1.8.2/mandown/sources/source_thecomicseries.py
--rw-r--r--   0        0        0     4059 2024-03-08 17:11:50.449985 mandown-1.8.2/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.8.2/mandown/ui/form.ui
--rw-r--r--   0        0        0     7060 2024-03-08 17:14:31.384962 mandown-1.8.2/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.8.2/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     6954 2024-03-08 17:14:31.383962 mandown-1.8.2/mandown/ui/ui.py
--rw-r--r--   0        0        0     1603 2024-05-14 15:31:19.435178 mandown-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.9.0/LICENSE
+-rw-r--r--   0        0        0     3885 2024-05-12 17:51:49.558004 mandown-1.9.0/README.md
+-rw-r--r--   0        0        0      542 2024-05-26 17:00:36.483789 mandown-1.9.0/mandown/__init__.py
+-rw-r--r--   0        0        0    12267 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/api.py
+-rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.9.0/mandown/base.py
+-rw-r--r--   0        0        0    17379 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/cli.py
+-rw-r--r--   0        0        0     2562 2024-03-08 17:11:50.449985 mandown-1.9.0/mandown/comic.py
+-rw-r--r--   0        0        0      705 2024-05-13 20:10:08.695482 mandown-1.9.0/mandown/convert_utils.py
+-rw-r--r--   0        0        0      142 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/errors.py
+-rw-r--r--   0        0        0     5694 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/io.py
+-rw-r--r--   0        0        0     5095 2024-03-08 17:11:50.449985 mandown-1.9.0/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4064 2024-03-08 17:11:50.449985 mandown-1.9.0/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1597 2024-03-08 17:11:50.448985 mandown-1.9.0/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1528 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2016 2024-03-08 17:11:50.448985 mandown-1.9.0/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     3301 2024-05-12 16:09:43.070512 mandown-1.9.0/mandown/sources/source_blogtruyenmoi.py
+-rw-r--r--   0        0        0     2716 2024-05-26 16:57:29.367141 mandown-1.9.0/mandown/sources/source_comixextra.py
+-rw-r--r--   0        0        0     4476 2024-05-12 17:51:49.558004 mandown-1.9.0/mandown/sources/source_kuaikanmanhua.py
+-rw-r--r--   0        0        0     5045 2024-03-08 17:11:50.450985 mandown-1.9.0/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2535 2024-03-08 17:11:50.449985 mandown-1.9.0/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2738 2024-05-15 17:38:08.510260 mandown-1.9.0/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3658 2024-03-08 17:11:50.450985 mandown-1.9.0/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3044 2024-03-08 17:11:50.451985 mandown-1.9.0/mandown/sources/source_manhuaes.py
+-rw-r--r--   0        0        0     3842 2024-05-15 17:35:57.085096 mandown-1.9.0/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     5154 2024-03-08 17:11:50.451985 mandown-1.9.0/mandown/sources/source_thecomicseries.py
+-rw-r--r--   0        0        0     4059 2024-03-08 17:11:50.449985 mandown-1.9.0/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.9.0/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7060 2024-03-08 17:14:31.384962 mandown-1.9.0/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.9.0/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     6954 2024-03-08 17:14:31.383962 mandown-1.9.0/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1603 2024-05-26 17:00:29.471877 mandown-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.9.0/PKG-INFO
```

### Comparing `mandown-1.8.2/LICENSE` & `mandown-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/README.md` & `mandown-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/__init__.py` & `mandown-1.9.0/mandown/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     ProcessConfig,
     ProcessOps,
     ProcessOptionMismatchError,
     Processor,
 )
 from .processor.profiles import SupportedProfiles, all_profiles
 
-__version__ = (1, 8, 2)
+__version__ = (1, 9, 0)
 __version_str__ = ".".join(map(str, __version__))
```

### Comparing `mandown-1.8.2/mandown/api.py` & `mandown-1.9.0/mandown/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Iterator
 
 import comicon
 
 from . import io, sources
 from .comic import BaseComic
 from .convert_utils import ConvertFormats, convert_one
+from .errors import ImageDownloadError
 from .processor import ProcessConfig, ProcessOps, Processor
 
 
 def query(url: str) -> BaseComic:
     """
     Attempt to query for a comic given a URL.
     :param `url`: An internet URL to search for
@@ -228,14 +229,15 @@
     comic: BaseComic | str,
     path: Path | str = ".",
     *,
     start: int | None = None,
     end: int | None = None,
     threads: int = 4,
     only_download_missing: bool = True,
+    raise_on_failed_download: bool = True,
 ) -> Iterator[str]:
     """
     Download comic or comic URL `comic` to `path` using `threads` threads.
 
     :param `comic`: A comic or URL to download
     :param `path`: A folder to download the comic to
     :param `start`: The first chapter to download (zero-indexed, inclusive)
@@ -309,23 +311,33 @@
             chapter_path,
             headers=comic.source.headers,
             filestems=filestems,
             threads=threads,
         ):
             pass
 
+        # check if every image was downloaded
+        if count := len([f for f in chapter_path.iterdir() if f.is_file()]) != len(
+            processed_image_urls
+        ):
+            if raise_on_failed_download:
+                raise ImageDownloadError(
+                    f"Failed to download {len(processed_image_urls) - count} images"
+                )
+
 
 def download(
     comic: BaseComic | str,
     path: Path | str = ".",
     *,
     start: int | None = None,
     end: int | None = None,
     threads: int = 4,
     only_download_missing: bool = True,
+    raise_on_failed_download: bool = True,
 ) -> None:
     """
     Download comic or comic URL `comic` to `path` using `threads` threads.
 
     :param `comic`: A comic or URL to download
     :param `path`: A folder to download the comic to
     :param `start`: The first chapter to download (one-indexed, inclusive)
```

### Comparing `mandown-1.8.2/mandown/base.py` & `mandown-1.9.0/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/cli.py` & `mandown-1.9.0/mandown/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ProcessOptionMismatchError,
     SupportedProfiles,
     __version_str__,
     all_profiles,
     api,
     sources,
 )
+from .errors import ImageDownloadError
 
 app = typer.Typer()
 
 
 def cli_init_metadata_interactive() -> None:
     path: Path = typer.prompt("Folder path", default=Path.cwd(), type=Path).expanduser().resolve()
 
@@ -415,20 +416,26 @@
     # zero-index
     start_chapter -= 1
 
     comic.set_chapter_range(start=start_chapter, end=end_chapter)
 
     # download
     typer.echo(f"Downloading {end_chapter - start_chapter} chapter(s)...")
-    with typer.progressbar(
-        api.download_progress(comic, dest, threads=maxthreads),
-        length=len(comic.chapters),
-    ) as progress:
-        for title in progress:
-            progress.label = title
+    try:
+        with typer.progressbar(
+            api.download_progress(comic, dest, threads=maxthreads),
+            length=len(comic.chapters),
+        ) as progress:
+            for title in progress:
+                progress.label = title
+    except ImageDownloadError as err:
+        typer.secho(
+            "Some image links on the host site were broken, ignoring...", fg=typer.colors.ORANGE
+        )
+        typer.secho(f"Error: {err}", fg=typer.colors.RED)
 
     full_dest_folder = dest.absolute() / comic.metadata.title_slug
     typer.secho(
         f"Successfully downloaded {end_chapter - start_chapter} chapter(s) to {full_dest_folder}.",
         fg=typer.colors.GREEN,
     )
```

### Comparing `mandown-1.8.2/mandown/comic.py` & `mandown-1.9.0/mandown/comic.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/convert_utils.py` & `mandown-1.9.0/mandown/convert_utils.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/io.py` & `mandown-1.9.0/mandown/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 from .base import BaseChapter, BaseMetadata
 from .comic import BaseComic
 
 NUM_LEFT_PAD_DIGITS = 5
 FILE_PADDING = f"0{NUM_LEFT_PAD_DIGITS}"
 MD_METADATA_FILE = "md-metadata.json"
 
+AsyncDownloadImageInput = tuple[str, Path | str, str | None, dict[str, str] | None]
 
-def async_download_image(data: tuple[str, Path | str, str | None, dict[str, str] | None]) -> None:
+
+def async_download_image(data: AsyncDownloadImageInput) -> None:
     """
     Download an image from a URL to a destination folder, fixing the file extension if necessary.
 
     :param `data`: A tuple of the url, destination folder, filename, and headers.
     """
     url, dest_folder, filename, headers = data
     dest_folder = Path(dest_folder)
 
     name = filename or url.split("/")[-1]
     dest_file = dest_folder / name
 
     res = requests.get(url, headers=headers, timeout=5)
-    res.raise_for_status()
+
+    if res.status_code != 200:
+        # there is no clean way to raise an error in a pool
+        # so we just return early and check it later
+        return
+
     with open(dest_file, "wb") as file:
         file.write(res.content)
 
     # if the file extension is lying
     # rename it so epubcheck doesn't yell at us
     ext = filetype.guess(dest_file)
     if ext is not None and ext.extension in ["jpg", "png", "gif"]:
@@ -62,15 +69,15 @@
     """
     dest_folder = Path(dest_folder)
 
     # attempt to create
     dest_folder.mkdir(exist_ok=True)
 
     # args to async_download
-    map_pool: list[tuple[str, Path | str, str | None, dict[str, str] | None]] = []
+    map_pool: list[AsyncDownloadImageInput] = []
 
     if filestems is None:
         filestems = [f"{i+1:FILE_PADDING}" for i in range(len(urls))]
 
     for url, stem in zip(urls, filestems, strict=True):
         _, ext = os.path.splitext(urllib.parse.urlparse(url).path)
         map_pool.append((url, dest_folder, f"{stem}{ext}", headers))
```

### Comparing `mandown-1.8.2/mandown/processor/__init__.py` & `mandown-1.9.0/mandown/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/processor/ops.py` & `mandown-1.9.0/mandown/processor/ops.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/processor/profiles.py` & `mandown-1.9.0/mandown/processor/profiles.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/__init__.py` & `mandown-1.9.0/mandown/sources/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import sys
 import types
 
 from . import (
     source_blogtruyenmoi,
+    source_comixextra,
     source_kuaikanmanhua,
     source_mangadex,
     source_mangakakalot,
     source_manganato,
     source_mangasee,
     source_manhuaes,
     source_readcomiconline,
```

### Comparing `mandown-1.8.2/mandown/sources/base_source.py` & `mandown-1.9.0/mandown/sources/base_source.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_blogtruyenmoi.py` & `mandown-1.9.0/mandown/sources/source_blogtruyenmoi.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_kuaikanmanhua.py` & `mandown-1.9.0/mandown/sources/source_kuaikanmanhua.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_mangadex.py` & `mandown-1.9.0/mandown/sources/source_mangadex.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_mangakakalot.py` & `mandown-1.9.0/mandown/sources/source_mangakakalot.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_manganato.py` & `mandown-1.9.0/mandown/sources/source_manganato.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class MangaNatoSource(BaseSource):
     name = "MangaNato"
     domains = [
         "https://manganato.com",
         "https://readmanganato.com",
         "https://chapmanganato.com",
+        "https://chapmanganato.to",
     ]
     headers = {"Referer": "https://readmanganato.com/"}
 
     def __init__(self, url: str) -> None:
         super().__init__(url)
         self.id = self.url_to_id(url)
         self._scripts: str | None = None
@@ -72,12 +73,13 @@
         return last_item
 
     @staticmethod
     def check_url(url: str) -> bool:
         return bool(
             re.match(r"https://readmanganato.com/.*", url)
             or re.match(r"https://chapmanganato.com/.*", url)
+            or re.match(r"https://chapmanganato.to/.*", url)
         )
 
 
 def get_class() -> type[BaseSource]:
     return MangaNatoSource
```

### Comparing `mandown-1.8.2/mandown/sources/source_mangasee.py` & `mandown-1.9.0/mandown/sources/source_mangasee.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_manhuaes.py` & `mandown-1.9.0/mandown/sources/source_manhuaes.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_readcomiconline.py` & `mandown-1.9.0/mandown/sources/source_readcomiconline.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import binascii
 import re
 
 import requests
 from bs4 import BeautifulSoup
 
 from ..base import BaseChapter, BaseMetadata
+from ..errors import NoImagesFoundError
 from .base_source import BaseSource
 
 
 class ReadComicOnlineSource(BaseSource):
     name = "ReadComicOnline"
     domains = ["https://readcomiconline.li"]
 
@@ -65,14 +66,19 @@
         images: list[str] = []
         start = 0
         while (index := text.find("lstImages.push(", start)) != -1:
             s_index = index + len("lstImages.push(") + 1
             e_index = text.find(");", s_index) - 1  # could be single or double quotes
             images.append(self.beau(text[s_index:e_index]))
             start = e_index
+        if not images:
+            raise NoImagesFoundError(
+                "No images found in the current chapter. Try visiting the URL in your browser "
+                "and solving any CAPTCHAs before trying again."
+            )
         return images
 
     @classmethod
     def url_to_id(cls, url: str) -> str:
         segments = url.split("/")
         for i, s in enumerate(segments):
             if s == "Comic":
```

### Comparing `mandown-1.8.2/mandown/sources/source_thecomicseries.py` & `mandown-1.9.0/mandown/sources/source_thecomicseries.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/sources/source_webtoons.py` & `mandown-1.9.0/mandown/sources/source_webtoons.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/ui/form.ui` & `mandown-1.9.0/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/ui/mainwin.py` & `mandown-1.9.0/mandown/ui/mainwin.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/mandown/ui/ui.py` & `mandown-1.9.0/mandown/ui/ui.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.2/pyproject.toml` & `mandown-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mandown"
-version = "1.8.2"
+version = "1.9.0"
 description = "Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter"
 authors = ["potatoeggy <eggyrules@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
@@ -14,25 +14,25 @@
 mandown-gui = "mandown.ui.ui:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 typer = "^0.7.0"
 feedparser = "^6.0.11"
 beautifulsoup4 = "^4.12.2"
-requests = "^2.31.0"
+requests = "^2.32.2"
 lxml = "^5.1.0"
 pillow = "^10.2.0"
 python-slugify = "^8.0.1"
 PySide6 = { version = "^6.6.1", optional = true }
 natsort = "^8.4.0"
 filetype = "^1.2.0"
-comicon = "^1.0.1"
+comicon = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
-types-requests = "^2.31.0.20240106"
+types-requests = "^2.32.0.20240523"
 types-lxml = "^2023.10.21"
 pytest-xdist = "^3.5.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
```

### Comparing `mandown-1.8.2/PKG-INFO` & `mandown-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.8.2
+Version: 1.9.0
 Summary: Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
 Author: potatoeggy
 Author-email: eggyrules@gmail.com
 Requires-Python: >=3.10,<3.13
@@ -12,22 +12,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: gui
 Requires-Dist: PySide6 (>=6.6.1,<7.0.0) ; extra == "gui"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: comicon (>=1.0.1,<2.0.0)
+Requires-Dist: comicon (>=1.2.0,<2.0.0)
 Requires-Dist: feedparser (>=6.0.11,<7.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: natsort (>=8.4.0,<9.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://github.com/potatoeggy/mandown
 Project-URL: Repository, https://github.com/potatoeggy/mandown
 Description-Content-Type: text/markdown
 
 # mandown
```

