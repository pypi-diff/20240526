# Comparing `tmp/nudebomb-0.3.6.tar.gz` & `tmp/nudebomb-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudebomb-0.3.6.tar", max compression
+gzip compressed data, was "nudebomb-0.3.7.tar", max compression
```

## Comparing `nudebomb-0.3.6.tar` & `nudebomb-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2024-02-19 01:01:44.140076 nudebomb-0.3.6/LICENSE
--rw-r--r--   0        0        0     1283 2024-02-19 01:01:44.140076 nudebomb-0.3.6/NEWS.md
--rw-r--r--   0        0        0     2255 2024-02-19 01:01:44.140076 nudebomb-0.3.6/README.md
--rw-r--r--   0        0        0       16 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/__init__.py
--rw-r--r--   0        0        0     4448 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/cli.py
--rw-r--r--   0        0        0     3920 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/config.py
--rw-r--r--   0        0        0      290 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/config_default.yaml
--rw-r--r--   0        0        0     2598 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/langfiles.py
--rw-r--r--   0        0        0     7078 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/mkv.py
--rw-r--r--   0        0        0      442 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/track.py
--rw-r--r--   0        0        0      344 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/version.py
--rw-r--r--   0        0        0     4526 2024-02-19 01:01:44.140076 nudebomb-0.3.6/nudebomb/walk.py
--rw-r--r--   0        0        0     3941 2024-02-19 01:01:44.144075 nudebomb-0.3.6/pyproject.toml
--rw-r--r--   0        0        0       13 2024-02-19 01:01:44.144075 nudebomb-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     2396 2024-02-19 01:01:44.144075 nudebomb-0.3.6/tests/mockdata/clean-tracks.json
--rw-r--r--   0        0        0  5100034 2024-02-19 01:01:44.152075 nudebomb-0.3.6/tests/test_files/test5.mkv
--rw-r--r--   0        0        0     1908 2024-02-19 01:01:44.152075 nudebomb-0.3.6/tests/test_integrated.py
--rw-r--r--   0        0        0     2335 2024-02-19 01:01:44.152075 nudebomb-0.3.6/tests/test_mkv.py
--rw-r--r--   0        0        0      810 2024-02-19 01:01:44.152075 nudebomb-0.3.6/tests/test_track.py
--rw-r--r--   0        0        0      622 2024-02-19 01:01:44.152075 nudebomb-0.3.6/tests/util.py
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 nudebomb-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-26 21:21:36.730395 nudebomb-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1326 2024-05-26 21:21:36.730395 nudebomb-0.3.7/NEWS.md
+-rw-r--r--   0        0        0     2255 2024-05-26 21:21:36.730395 nudebomb-0.3.7/README.md
+-rw-r--r--   0        0        0       16 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/__init__.py
+-rw-r--r--   0        0        0     5058 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/cli.py
+-rw-r--r--   0        0        0     3921 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/config.py
+-rw-r--r--   0        0        0      290 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/config_default.yaml
+-rw-r--r--   0        0        0     2599 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/langfiles.py
+-rw-r--r--   0        0        0     7108 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/mkv.py
+-rw-r--r--   0        0        0      442 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/track.py
+-rw-r--r--   0        0        0      344 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/version.py
+-rw-r--r--   0        0        0     4527 2024-05-26 21:21:36.730395 nudebomb-0.3.7/nudebomb/walk.py
+-rw-r--r--   0        0        0     3941 2024-05-26 21:21:36.734395 nudebomb-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-26 21:21:36.734395 nudebomb-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-26 21:21:36.734395 nudebomb-0.3.7/tests/mockdata/clean-tracks.json
+-rw-r--r--   0        0        0  5100034 2024-05-26 21:21:36.738395 nudebomb-0.3.7/tests/test_files/test5.mkv
+-rw-r--r--   0        0        0     1909 2024-05-26 21:21:36.738395 nudebomb-0.3.7/tests/test_integrated.py
+-rw-r--r--   0        0        0     2336 2024-05-26 21:21:36.738395 nudebomb-0.3.7/tests/test_mkv.py
+-rw-r--r--   0        0        0      811 2024-05-26 21:21:36.738395 nudebomb-0.3.7/tests/test_track.py
+-rw-r--r--   0        0        0      623 2024-05-26 21:21:36.738395 nudebomb-0.3.7/tests/util.py
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 nudebomb-0.3.7/PKG-INFO
```

### Comparing `nudebomb-0.3.6/LICENSE` & `nudebomb-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.6/NEWS.md` & `nudebomb-0.3.7/NEWS.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # 📰 Nudebomb News
 
+## v0.3.7
+
+- Add a dot color key to help.
+
 ## v0.3.6
 
 - Fix treestamps wal file bug with illegal characters in filename.
 
 ## v0.3.5
 
 - Require python 3.10
```

### Comparing `nudebomb-0.3.6/README.md` & `nudebomb-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.6/nudebomb/cli.py` & `nudebomb-0.3.7/nudebomb/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Command line interface for nudebomb."""
-from argparse import Action, ArgumentParser, Namespace
+
+from argparse import Action, ArgumentParser, Namespace, RawDescriptionHelpFormatter
+
+from termcolor import colored
 
 from nudebomb.config import get_config
 from nudebomb.version import VERSION
 from nudebomb.walk import Walk
 
 
 class CommaListAction(Action):
@@ -16,15 +19,34 @@
         items = values.strip().split(self.DELINEATOR)
         setattr(namespace, self.dest, items)
 
 
 def get_arguments(params=None):
     """Command line interface."""
     description = "Strips unnecessary tracks from MKV files."
-    parser = ArgumentParser(description=description)
+    epilog = (
+        "Dot color key:\n"
+        + colored("\tMKV ignored", "white", attrs=["dark"])
+        + "\n"
+        + colored("\tMKV timestamp unchanged", "cyan")
+        + "\n"
+        + colored("\tMKV already stripped", "green")
+        + "\n"
+        + colored("\tMKV not remuxed on dry run", "black", attrs=["bold"])
+        + "\n"
+        + colored("\tWarning", "yellow")
+        + "\n"
+        + colored("\tError", "red")
+        + "\n"
+    )
+    parser = ArgumentParser(
+        description=description,
+        epilog=epilog,
+        formatter_class=RawDescriptionHelpFormatter,
+    )
     parser.add_argument(
         "-d",
         "--dry-run",
         action="store_true",
         help="Enable mkvmerge dry run for testing.",
     )
     parser.add_argument(
```

### Comparing `nudebomb-0.3.6/nudebomb/config.py` & `nudebomb-0.3.7/nudebomb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Confuse config for comicbox."""
+
 import os
 import sys
 from argparse import Namespace
 from platform import system
 from time import mktime
 
 from confuse import Configuration
```

### Comparing `nudebomb-0.3.6/nudebomb/langfiles.py` & `nudebomb-0.3.7/nudebomb/langfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for reading lang files."""
+
 import pycountry
 from termcolor import cprint
 
 LANGS_FNS = ("lang", "langs", ".lang", ".langs")
 
 
 def lang_to_alpha3(lang):
```

### Comparing `nudebomb-0.3.6/nudebomb/mkv.py` & `nudebomb-0.3.7/nudebomb/mkv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MKV file operations."""
+
 import json
 import subprocess
 import sys
 import time
 from pathlib import Path
 
 from termcolor import cprint
@@ -186,22 +187,22 @@
             output, command, num_remove_ids = self._extend_track_command(
                 track_type, output, command, num_remove_ids
             )
         command += [(str(self.path))]
 
         if not num_remove_ids:
             if self._config.verbose:
-                cprint(f"\tNot remuxing {self.path}", "green", attrs=["dark"])
+                cprint(f"\tAlready stripped {self.path}", "green", attrs=["dark"])
             else:
                 cprint(".", "green", attrs=["bold"], end="")
             return
 
         try:
             cprint(output, flush=True)
             if self._config.dry_run:
-                cprint("Dry run 100%", "black", attrs=["bold"])
+                cprint("\tNot remuxing on dry run {self.path}", "black", attrs=["bold"])
             else:
                 self._remux_file(command)
                 tmp_path.replace(self.path)
         except Exception as exc:
             cprint(str(exc), "red")
             tmp_path.unlink(missing_ok=True)
```

### Comparing `nudebomb-0.3.6/nudebomb/walk.py` & `nudebomb-0.3.7/nudebomb/walk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Walk directory trees and strip mkvs."""
+
 import os
 from copy import deepcopy
 from pathlib import Path
 
 from termcolor import cprint
 from treestamps import Grovestamps, GrovestampsConfig
 from treestamps.tree import Treestamps
```

### Comparing `nudebomb-0.3.6/pyproject.toml` & `nudebomb-0.3.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nudebomb"
-version = "0.3.6"
+version = "0.3.7"
 description = "Strip unused languages from mkv files en mass"
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/nudebomb"
 documentation = "https://github.com/ajslater/nudebomb"
 keywords = ["mkv", "movie", "video", "srt", "audio", "subtitles"]
@@ -38,18 +38,18 @@
 termcolor = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
 neovim = "^0.3.1"
 pyright = "^1.1.237"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-gitignore = "^1.3"
 radon = { version = "^6.0.1", extras = ["toml"] }
-ruff = "^0.2.1"
+ruff = "^0.4.5"
 types-python-dateutil = "^2.8.0"
 vulture = "^2.1"
 
 [tool.poetry.scripts]
 nudebomb = "nudebomb.cli:main"
 
 [tool.poetry.urls]
```

### Comparing `nudebomb-0.3.6/tests/mockdata/clean-tracks.json` & `nudebomb-0.3.7/tests/mockdata/clean-tracks.json`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.6/tests/test_files/test5.mkv` & `nudebomb-0.3.7/tests/test_files/test5.mkv`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.6/tests/test_integrated.py` & `nudebomb-0.3.7/tests/test_integrated.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """Integration tests."""
+
 import shutil
 from pathlib import Path
 
 from nudebomb.cli import main
 from nudebomb.mkv import MKVFile
 
 from .test_mkv import assert_eng_und_only
```

### Comparing `nudebomb-0.3.6/tests/test_mkv.py` & `nudebomb-0.3.7/tests/test_mkv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test MKVFile object."""
+
 import os
 import shutil
 from pathlib import Path
 
 from nudebomb.config import get_config
 from nudebomb.mkv import MKVFile
```

### Comparing `nudebomb-0.3.6/tests/test_track.py` & `nudebomb-0.3.7/tests/test_track.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test Track class."""
+
 import json
 
 from nudebomb.track import Track
 
 from .util import read
 
 __all__ = ()
```

### Comparing `nudebomb-0.3.6/tests/util.py` & `nudebomb-0.3.7/tests/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common test utilities."""
+
 import json
 import subprocess
 from pathlib import Path
 
 TEST_FN = "test5.mkv"
 SRC_DIR = Path("tests/test_files")
 SRC_PATH = SRC_DIR / TEST_FN
```

### Comparing `nudebomb-0.3.6/PKG-INFO` & `nudebomb-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudebomb
-Version: 0.3.6
+Version: 0.3.7
 Summary: Strip unused languages from mkv files en mass
 Home-page: https://github.com/ajslater/nudebomb
 License: GPL-3.0-only
 Keywords: mkv,movie,video,srt,audio,subtitles
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.10,<4.0
```

