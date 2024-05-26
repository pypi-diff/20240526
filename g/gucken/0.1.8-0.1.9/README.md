# Comparing `tmp/gucken-0.1.8.tar.gz` & `tmp/gucken-0.1.9.tar.gz`

## Comparing `gucken-0.1.8.tar` & `gucken-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/__main__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0    32797 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/rome.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/settings.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/update.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/_hosters.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/_players.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/android.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/common.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/mpv.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/resources/default_settings.toml
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/resources/gucken.css
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/resources/mpv_skip.lua
--rwxr-xr-x   0        0        0     3912 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/resources/vlc_skip.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.8/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.8/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 gucken-0.1.8/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 gucken-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/__main__.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0    32575 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/rome.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/settings.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/update.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/_hosters.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/_players.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/android.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/common.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/resources/default_settings.toml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/resources/gucken.css
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/resources/mpv_gucken.lua
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/resources/vlc_gucken.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.9/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 gucken-0.1.9/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 gucken-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 gucken-0.1.9/PKG-INFO
```

### Comparing `gucken-0.1.8/src/gucken/custom_widgets.py` & `gucken-0.1.9/src/gucken/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/gucken.py` & `gucken-0.1.9/src/gucken/gucken.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import warnings
+warnings.filterwarnings('ignore', message='Using slow pure-python SequenceMatcher. Install python-Levenshtein to remove this warning')
+
 import argparse
 import logging
 from asyncio import gather
 from atexit import register as register_atexit
 from os import remove, name as os_name
 from os.path import join
 from pathlib import Path
@@ -21,33 +24,29 @@
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual.widgets import (
     Button,
     Checkbox,
     Collapsible,
     DataTable,
-    Footer,
     Header,
     Input,
     Label,
     ListItem,
     ListView,
     Markdown,
     RadioButton,
     Select,
     TabbedContent,
     TabPane,
 )
 
 from .aniskip import (
     generate_chapters_file,
-    get_chapters_file_mpv_option,
-    get_timings_from_search,
-    opening_timings_to_mpv_option,
-    ending_timings_to_mpv_option
+    get_timings_from_search
 )
 from .custom_widgets import SortableTable
 from .hoster._hosters import hoster
 from .hoster.common import DirectLink, Hoster
 from .player._players import all_players_keys, available_players_keys, player_map
 from .player.mpv import MPVPlayer
 from .player.vlc import VLCPlayer
@@ -477,14 +476,15 @@
         final_results = []
         for l in results:
             if l is not None:
                 for e in l:
                     final_results.append(e)
 
         # TODO: Sort final_results with fuzzy-sort
+        # from fuzzywuzzy import process process.extract()
         if len(final_results) > 0:
             self.current = final_results
             for series in final_results:
                 # TODO: show provider
                 await results_list_view.append(
                     ClickableListItem(
                         Markdown(
@@ -677,76 +677,64 @@
         if isinstance(_player, MPVPlayer) or isinstance(_player, VLCPlayer):
             ani_skip_opening = self.query_one("#ani_skip_opening", RadioButton).value
             ani_skip_ending = self.query_one("#ani_skip_ending", RadioButton).value
             ani_skip_chapters = self.query_one("#ani_skip_chapters", RadioButton).value
 
             if ani_skip_opening or ani_skip_ending or ani_skip_chapters:
                 timings = await get_timings_from_search(
-                    series_search_result.name, index + 1
+                    series_search_result.name + " " + str(episode.season), episode.episode_number
                 )
                 if timings:
                     if isinstance(_player, MPVPlayer):
                         if ani_skip_chapters:
                             chapters_file = generate_chapters_file(timings)
 
                             def delete_chapters_file():
                                 try:
                                     remove(chapters_file.name)
                                 except FileNotFoundError:
                                     pass
 
                             register_atexit(delete_chapters_file)
+                            args.append(f"--chapters-file={chapters_file.name}")
 
-                            args.append(get_chapters_file_mpv_option(chapters_file.name))
-
+                        script_opts = []
                         if ani_skip_opening:
-                            args.append(opening_timings_to_mpv_option(timings))
-
+                            script_opts.append(f"skip-op_start={timings.op_start}")
+                            script_opts.append(f"skip-op_end={timings.op_end}")
                         if ani_skip_ending:
-                            args.append(ending_timings_to_mpv_option(timings))
+                            script_opts.append(f"skip-ed_start={timings.ed_start}")
+                            script_opts.append(f"skip-ed_end={timings.ed_end}")
+                        if len(script_opts) > 0:
+                            args.append(f"--script-opts={','.join(script_opts)}")
 
-                        args.append("--script=" + str(Path(__file__).parent.joinpath("resources", "mpv_skip.lua")))
+                        args.append("--scripts-append=" + str(Path(__file__).parent.joinpath("resources", "mpv_gucken.lua")))
 
                     if isinstance(_player, VLCPlayer):
-                        # cant use --lua-config because it would override syncplay cfg
-                        # cant use --extraintf and --lua-intf because it is already used by syncplay
-                        """
-                            args = [
-                                "vlc",
-                                "--extraintf=luaintf",
-                                "--lua-intf=skip",
-                                "--lua-config=skip={" + f"op_start={op_start},op_end={op_end},ed_start={ed_start},ed_end={ed_end}" +"}",
-                                url
-                            ]
-                        """
-                        prepend_data = ["-- Generated"]
-
+                        prepend_data = []
                         if ani_skip_opening:
-                            prepend_data.append(set_default_vlc_interface_cfg("op_start", timings["op_start_time"]))
-                            prepend_data.append(set_default_vlc_interface_cfg("op_end", timings["op_end_time"]))
-
+                            prepend_data.append(set_default_vlc_interface_cfg("op_start", timings.op_start))
+                            prepend_data.append(set_default_vlc_interface_cfg("op_end", timings.op_end))
                         if ani_skip_ending:
-                            prepend_data.append(set_default_vlc_interface_cfg("ed_start", timings["ed_start_time"]))
-                            prepend_data.append(set_default_vlc_interface_cfg("ed_end", timings["ed_end_time"]))
-
-                        prepend_data.append("-- Generated\n")
+                            prepend_data.append(set_default_vlc_interface_cfg("ed_start", timings.ed_start))
+                            prepend_data.append(set_default_vlc_interface_cfg("ed_end", timings.ed_end))
 
                         vlc_intf_user_path = get_vlc_intf_user_path(_player.executable).vlc_intf_user_path
                         Path(vlc_intf_user_path).mkdir(mode=0o755, parents=True, exist_ok=True)
 
-                        vlc_skip_plugin = Path(__file__).parent.joinpath("resources", "vlc_skip.lua")
-                        copyTo = join(vlc_intf_user_path, "vlc_skip.lua")
+                        vlc_skip_plugin = Path(__file__).parent.joinpath("resources", "vlc_gucken.lua")
+                        copy_to = join(vlc_intf_user_path, "vlc_gucken.lua")
 
                         with open(vlc_skip_plugin, 'r') as f:
                             original_content = f.read()
 
-                        with open(copyTo, 'w') as f:
+                        with open(copy_to, 'w') as f:
                             f.write("\n".join(prepend_data) + original_content)
 
-                        args.append("--control=luaintf{intf=vlc_skip}")
+                        args.append("--control=luaintf{intf=vlc_gucken}")
 
         if syncplay:
             # TODO: make work with flatpak
             # TODO: make work with android
             syncplay_path = None
             if which("syncplay"):
                 syncplay_path = "syncplay"
@@ -767,14 +755,15 @@
                     url = args[1]
                     args.pop(0)
                     args.pop(0)
                     args = [
                                syncplay_path,
                                "--player-path",
                                player_path,
+                               # "--debug",
                                url,
                                "--",
                            ] + args
                 else:
                     self.notify(
                         "Your player is not supported by Syncplay",
                         title="Player not supported",
```

### Comparing `gucken-0.1.8/src/gucken/rome.py` & `gucken-0.1.9/src/gucken/rome.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/settings.py` & `gucken-0.1.9/src/gucken/settings.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/update.py` & `gucken-0.1.9/src/gucken/update.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/utils.py` & `gucken-0.1.9/src/gucken/utils.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/hoster/common.py` & `gucken-0.1.9/src/gucken/hoster/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/hoster/doodstream.py` & `gucken-0.1.9/src/gucken/hoster/doodstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/hoster/streamtape.py` & `gucken-0.1.9/src/gucken/hoster/streamtape.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/hoster/veo.py` & `gucken-0.1.9/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/hoster/vidoza.py` & `gucken-0.1.9/src/gucken/hoster/vidoza.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/_players.py` & `gucken-0.1.9/src/gucken/player/_players.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/android.py` & `gucken-0.1.9/src/gucken/player/android.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/common.py` & `gucken-0.1.9/src/gucken/player/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/ffplay.py` & `gucken-0.1.9/src/gucken/player/ffplay.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/flatpak.py` & `gucken-0.1.9/src/gucken/player/flatpak.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/mpv.py` & `gucken-0.1.9/src/gucken/player/mpv.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/vlc.py` & `gucken-0.1.9/src/gucken/player/vlc.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/player/wmplayer.py` & `gucken-0.1.9/src/gucken/player/wmplayer.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/provider/aniworld.py` & `gucken-0.1.9/src/gucken/provider/aniworld.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/provider/common.py` & `gucken-0.1.9/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/provider/serienstream.py` & `gucken-0.1.9/src/gucken/provider/serienstream.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/resources/default_settings.toml` & `gucken-0.1.9/src/gucken/resources/default_settings.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/src/gucken/resources/gucken.css` & `gucken-0.1.9/src/gucken/resources/gucken.css`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 #input {
     margin: 1 0;
 }
 
 #markdown {
     margin: 0 0;
-    margin-top: -1;
+    margin-top: -2;
 }
 
 /*TODO: make height 100 of what the table needs, so there is only one scroll*/
 #season_list {
     margin: 1 0;
     margin-top: 0;
     margin-bottom: 0;
@@ -63,8 +63,12 @@
 #footer {
     background: $accent;
     color: $text;
     dock: bottom;
     height: 1;
 }
 
+SortableTable {
+    width: auto;
+}
+
 /*$accent: lime;*/
```

### Comparing `gucken-0.1.8/src/gucken/resources/mpv_skip.lua` & `gucken-0.1.9/src/gucken/resources/mpv_gucken.lua`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 local mpv_utils = require("mp.utils")
 
 -- Stop script if skip.lua is inside scripts folder
 local scripts_dir = mp.find_config_file("scripts")
-if mpv_utils.file_info(mpv_utils.join_path(scripts_dir, "skip.lua")) ~= nil then
+if scripts_dir ~= nil and mpv_utils.file_info(mpv_utils.join_path(scripts_dir, "skip.lua")) ~= nil then
 	mp.msg.info("Disabling, another skip.lua is already present in scripts dir")
 	return
 end
 
 local mpv_options = require("mp.options")
 
 local options = {
```

### Comparing `gucken-0.1.8/src/gucken/tracker/anilist.py` & `gucken-0.1.9/src/gucken/tracker/anilist.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/LICENSE.txt` & `gucken-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.8/README.md` & `gucken-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 - [x] Language priority list
 - [x] Hoster priority list
 - [x] Automatically use working hoster
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
-  - [x] Discord Presence **WIP**
+  - [x] Discord Presence **Very WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support (almost out of WIP)
     - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
@@ -201,15 +201,14 @@
 - [ ] CI Testing (Windows, Linux)
 - [ ] CD pip
 - [ ] [Anime4k] options
 - [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
-- [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
 - [ ] Image preview (Kitty protocol, iterm protocol, Sixel, textual-web)
 - [ ] Support textual-web
 - [ ] Blacklist detection & bypass
 - [ ] Mac support
 - [ ] IOS support
 - [ ] Update checker option to perform update
```

### Comparing `gucken-0.1.8/pyproject.toml` & `gucken-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 dynamic = ["version"]
 description = "Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style."
 authors = [{name="Commandcracker"}]
 maintainers = [{name="Commandcracker"}]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 dependencies = [
-  "textual>=0.62.0",
+  "textual>=0.63.3",
   "beautifulsoup4>=4.12.3",
   "httpx>=0.27.0",
   "pypresence>=4.3.0",
   "packaging>=24.0",
   "platformdirs>=4.2.2",
-  "toml>=0.10.2"
+  "toml>=0.10.2",
+  "fuzzywuzzy>=0.18.0",
+  "levenshtein>=0.25.1"
   #"yt-dlp>=2024.4.9",
   #"mpv>=1.0.6",
   #"httpx[socks]",
 ]
 keywords = [
   "gucken",
   "anime",
```

### Comparing `gucken-0.1.8/PKG-INFO` & `gucken-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
@@ -41,19 +41,21 @@
 Classifier: Programming Language :: Lua
 Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: fuzzywuzzy>=0.18.0
 Requires-Dist: httpx>=0.27.0
+Requires-Dist: levenshtein>=0.25.1
 Requires-Dist: packaging>=24.0
 Requires-Dist: platformdirs>=4.2.2
 Requires-Dist: pypresence>=4.3.0
-Requires-Dist: textual>=0.62.0
+Requires-Dist: textual>=0.63.3
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
 
 # Gucken
 
 Project state: **Pre-Alpha**
 
@@ -141,17 +143,17 @@
 - [x] Language priority list
 - [x] Hoster priority list
 - [x] Automatically use working hoster
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
-  - [x] Discord Presence **WIP**
+  - [x] Discord Presence **Very WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support (almost out of WIP)
     - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
@@ -256,15 +258,14 @@
 - [ ] CI Testing (Windows, Linux)
 - [ ] CD pip
 - [ ] [Anime4k] options
 - [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
-- [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
 - [ ] Image preview (Kitty protocol, iterm protocol, Sixel, textual-web)
 - [ ] Support textual-web
 - [ ] Blacklist detection & bypass
 - [ ] Mac support
 - [ ] IOS support
 - [ ] Update checker option to perform update
```

