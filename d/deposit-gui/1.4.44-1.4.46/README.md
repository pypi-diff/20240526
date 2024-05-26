# Comparing `tmp/deposit_gui-1.4.44.tar.gz` & `tmp/deposit_gui-1.4.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deposit_gui-1.4.44.tar", last modified: Thu Feb 29 14:49:42 2024, max compression
+gzip compressed data, was "deposit_gui-1.4.46.tar", last modified: Sun May 26 18:22:13 2024, max compression
```

## Comparing `deposit_gui-1.4.44.tar` & `deposit_gui-1.4.46.tar`

### file list

```diff
@@ -1,314 +1,314 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:42.049662 deposit_gui-1.4.44/
--rw-rw-rw-   0        0        0    35821 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/LICENSE
--rw-rw-rw-   0        0        0     2900 2024-02-29 14:49:42.049662 deposit_gui-1.4.44/PKG-INFO
--rw-rw-rw-   0        0        0     2117 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/README.md
--rw-rw-rw-   0        0        0       97 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-02-29 14:49:42.065305 deposit_gui-1.4.44/setup.cfg
--rw-rw-rw-   0        0        0     1724 2024-02-29 14:48:41.000000 deposit_gui-1.4.44/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.564080 deposit_gui-1.4.44/src/
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.595322 deposit_gui-1.4.44/src/deposit_gui/
--rw-rw-rw-   0        0        0    35821 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/LICENSE
--rw-rw-rw-   0        0        0      893 2024-02-29 14:48:41.000000 deposit_gui-1.4.44/src/deposit_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.633068 deposit_gui-1.4.44/src/deposit_gui/controller/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/__init__.py
--rw-rw-rw-   0        0        0    15994 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cactions.py
--rw-rw-rw-   0        0        0    18641 2024-02-29 09:51:52.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cdialogs.py
--rw-rw-rw-   0        0        0     9120 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cmdiarea.py
--rw-rw-rw-   0        0        0     3923 2024-02-29 10:02:23.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cmodel.py
--rw-rw-rw-   0        0        0     3891 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cnavigator.py
--rw-rw-rw-   0        0        0     4368 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/controller.py
--rw-rw-rw-   0        0        0      718 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cquerytoolbar.py
--rw-rw-rw-   0        0        0     7601 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cusertools.py
--rw-rw-rw-   0        0        0     2650 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/controller/cview.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.664316 deposit_gui-1.4.44/src/deposit_gui/dgui/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/__init__.py
--rw-rw-rw-   0        0        0      181 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/abstract_subcontroller.py
--rw-rw-rw-   0        0        0      889 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/abstract_subview.py
--rw-rw-rw-   0        0        0     2709 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dcactions.py
--rw-rw-rw-   0        0        0     2895 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dcdialogs.py
--rw-rw-rw-   0        0        0      486 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dclickable_logo.py
--rw-rw-rw-   0        0        0    15038 2024-02-29 09:57:20.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dcmodel.py
--rw-rw-rw-   0        0        0     2925 2024-02-29 10:46:53.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_frame.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.679937 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/__init__.py
--rw-rw-rw-   0        0        0     3349 2024-02-29 12:00:02.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/abstract_tab_file.py
--rw-rw-rw-   0        0        0     8590 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db.py
--rw-rw-rw-   0        0        0      230 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db_rel.py
--rw-rw-rw-   0        0        0      145 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_json.py
--rw-rw-rw-   0        0        0      815 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_memory.py
--rw-rw-rw-   0        0        0      149 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_pickle.py
--rw-rw-rw-   0        0        0     2677 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_recent.py
--rw-rw-rw-   0        0        0     2005 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/ddialog.py
--rw-rw-rw-   0        0        0    29511 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dgraph_view.py
--rw-rw-rw-   0        0        0     3184 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dgraphics_view.py
--rw-rw-rw-   0        0        0     1209 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dlogging.py
--rw-rw-rw-   0        0        0     2663 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dmain_window.py
--rw-rw-rw-   0        0        0     1207 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dmenu_bar.py
--rw-rw-rw-   0        0        0    11285 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dmodel.py
--rw-rw-rw-   0        0        0     2270 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dnotification.py
--rw-rw-rw-   0        0        0     1046 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dprogress.py
--rw-rw-rw-   0        0        0     2264 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dregistry.py
--rw-rw-rw-   0        0        0     1771 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dsave_as_postgres_frame.py
--rw-rw-rw-   0        0        0      290 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dstatus_bar.py
--rw-rw-rw-   0        0        0     4921 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dtool_bar.py
--rw-rw-rw-   0        0        0      857 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dvactions.py
--rw-rw-rw-   0        0        0      815 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dvdialogs.py
--rw-rw-rw-   0        0        0     4228 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/dview.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.795803 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/__init__.py
--rwxrwxrwx   0        0        0    13312 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/acyclic.exe
--rwxrwxrwx   0        0        0    17408 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/bcomps.exe
--rw-rw-rw-   0        0        0  1506816 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cairo.dll
--rwxrwxrwx   0        0        0    23040 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/ccomps.exe
--rw-rw-rw-   0        0        0    24576 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cdt.dll
--rw-rw-rw-   0        0        0    11264 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cgraph++.dll
--rw-rw-rw-   0        0        0    75264 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cgraph.dll
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/circo.exe
--rw-rw-rw-   0        0        0   317216 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/concrt140.dll
--rw-rw-rw-   0        0        0     3057 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/config6
--rwxrwxrwx   0        0        0    16896 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dijkstra.exe
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dot.exe
--rwxrwxrwx   0        0        0    37376 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dot2gxl.exe
--rwxrwxrwx   0        0        0   235008 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/edgepaint.exe
--rw-rw-rw-   0        0        0   184832 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/expat.dll
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/fdp.exe
--rw-rw-rw-   0        0        0   830976 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/fontconfig.dll
--rwxrwxrwx   0        0        0    15872 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gc.exe
--rw-rw-rw-   0        0        0    19968 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/getopt.dll
--rw-rw-rw-   0        0        0  1374208 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/glib-2.dll
--rwxrwxrwx   0        0        0    36864 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gml2gv.exe
--rw-rw-rw-   0        0        0   276480 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gobject-2.dll
--rwxrwxrwx   0        0        0    22016 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/graphml2gv.exe
--rwxrwxrwx   0        0        0    22016 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gv2gml.exe
--rw-rw-rw-   0        0        0    17408 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvc++.dll
--rw-rw-rw-   0        0        0   551424 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvc.dll
--rwxrwxrwx   0        0        0    36864 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvcolor.exe
--rwxrwxrwx   0        0        0    25088 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvgen.exe
--rwxrwxrwx   0        0        0   311808 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvmap.exe
--rw-rw-rw-   0        0        0     2386 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvmap.sh
--rwxrwxrwx   0        0        0    33792 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvpack.exe
--rw-rw-rw-   0        0        0   122368 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_core.dll
--rw-rw-rw-   0        0        0   156160 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_dot_layout.dll
--rw-rw-rw-   0        0        0    31744 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_gdiplus.dll
--rw-rw-rw-   0        0        0   374272 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_neato_layout.dll
--rw-rw-rw-   0        0        0    38912 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_pango.dll
--rw-rw-rw-   0        0        0    43520 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_visio.dll
--rwxrwxrwx   0        0        0   329728 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvpr.exe
--rwxrwxrwx   0        0        0    37376 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gxl2gv.exe
--rw-rw-rw-   0        0        0   922112 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/libharfbuzz-0.dll
--rwxrwxrwx   0        0        0    33792 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/mm2gv.exe
--rw-rw-rw-   0        0        0   590096 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140.dll
--rw-rw-rw-   0        0        0    31528 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_1.dll
--rw-rw-rw-   0        0        0   193312 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_2.dll
--rw-rw-rw-   0        0        0    27424 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_codecvt_ids.dll
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/neato.exe
--rwxrwxrwx   0        0        0    12800 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/nop.exe
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/osage.exe
--rw-rw-rw-   0        0        0   287744 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pango-1.dll
--rw-rw-rw-   0        0        0   612864 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangocairo-1.dll
--rw-rw-rw-   0        0        0   639488 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangoft2-1.dll
--rw-rw-rw-   0        0        0    65536 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangowin32-1.dll
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/patchwork.exe
--rw-rw-rw-   0        0        0    39936 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pathplan.dll
--rw-rw-rw-   0        0        0   578560 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pixman-1.dll
--rwxrwxrwx   0        0        0    17920 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/sccmap.exe
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/sfdp.exe
--rwxrwxrwx   0        0        0    16384 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/tred.exe
--rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/twopi.exe
--rwxrwxrwx   0        0        0    16384 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/unflatten.exe
--rw-rw-rw-   0        0        0   101664 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/vcruntime140.dll
--rw-rw-rw-   0        0        0    44328 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/vcruntime140_1.dll
--rw-rw-rw-   0        0        0    25600 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/xdot.dll
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.811426 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/
--rw-rw-rw-   0        0        0        5 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/INSTALLER
--rw-rw-rw-   0        0        0     1655 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/LICENSE
--rw-rw-rw-   0        0        0     2899 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/METADATA
--rw-rw-rw-   0        0        0      958 2024-02-29 14:13:30.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/__init__.py
--rw-rw-rw-   0        0        0   103424 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/_graphviz.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   217528 2024-02-29 13:56:03.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/_graphviz.cpython-310-darwin.so
--rw-rw-rw-   0        0        0    72375 2024-02-29 14:14:24.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/agraph.py
--rw-rw-rw-   0        0        0     9298 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz.i
--rw-rw-rw-   0        0        0     7202 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz.py
--rw-rw-rw-   0        0        0   194463 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz_wrap.c
--rw-rw-rw-   0        0        0     2861 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/scraper.py
--rw-rw-rw-   0        0        0      609 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/testing.py
--rw-rw-rw-   0        0        0      500 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dgui_main.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.827047 deposit_gui-1.4.44/src/deposit_gui/dialogs/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/__init__.py
--rw-rw-rw-   0        0        0     1384 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_about.py
--rw-rw-rw-   0        0        0     2297 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_add_relation.py
--rw-rw-rw-   0        0        0      907 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_connect.py
--rw-rw-rw-   0        0        0     5158 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_import_external.py
--rw-rw-rw-   0        0        0      264 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_import_source.py
--rw-rw-rw-   0        0        0     1383 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_import_store.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.949422 deposit_gui-1.4.44/src/deposit_gui/res/
--rw-rw-rw-   0        0        0     3997 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/3d_obj.svg
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/__init__.py
--rw-rw-rw-   0        0        0     4468 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add.svg
--rw-rw-rw-   0        0        0     5809 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_class.svg
--rw-rw-rw-   0        0        0     7103 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_descriptor.svg
--rw-rw-rw-   0        0        0     6328 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_form.svg
--rw-rw-rw-   0        0        0     4271 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_object.svg
--rw-rw-rw-   0        0        0     4990 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_query.svg
--rw-rw-rw-   0        0        0     3249 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/add_search.svg
--rw-rw-rw-   0        0        0     5252 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/attributes.svg
--rw-rw-rw-   0        0        0     4497 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/attributes_simple.svg
--rw-rw-rw-   0        0        0     4286 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/bold.svg
--rw-rw-rw-   0        0        0     7721 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/calculator.svg
--rw-rw-rw-   0        0        0     3173 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/check_box.svg
--rw-rw-rw-   0        0        0     4812 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/class.svg
--rw-rw-rw-   0        0        0    24326 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/classes_graph.svg
--rw-rw-rw-   0        0        0     3364 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/column_break.svg
--rw-rw-rw-   0        0        0     4186 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/combo_box.svg
--rw-rw-rw-   0        0        0     5820 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/connect.svg
--rw-rw-rw-   0        0        0     6697 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/copy.svg
--rw-rw-rw-   0        0        0     3691 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/database.svg
--rw-rw-rw-   0        0        0     2805 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/delete.svg
--rw-rw-rw-   0        0        0     3518 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/dep_cube.svg
--rw-rw-rw-   0        0        0    14186 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/dep_installer.svg
--rw-rw-rw-   0        0        0     5443 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/deposit_logo.svg
--rw-rw-rw-   0        0        0     6188 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/descriptor.svg
--rw-rw-rw-   0        0        0     5845 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/disconnect.svg
--rw-rw-rw-   0        0        0     7401 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/dock.svg
--rw-rw-rw-   0        0        0     2293 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/down_small.svg
--rw-rw-rw-   0        0        0     2298 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/down_small_black.svg
--rw-rw-rw-   0        0        0     7023 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/draw_polygon.svg
--rw-rw-rw-   0        0        0     4896 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/edit.svg
--rw-rw-rw-   0        0        0     6722 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/edit_class.svg
--rw-rw-rw-   0        0        0     6378 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/edit_query.svg
--rw-rw-rw-   0        0        0     3862 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/export_deposit.svg
--rw-rw-rw-   0        0        0    12377 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/export_external.svg
--rw-rw-rw-   0        0        0     4772 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/file.svg
--rw-rw-rw-   0        0        0     5462 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/form.svg
--rw-rw-rw-   0        0        0     3916 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/geometry.svg
--rw-rw-rw-   0        0        0     9955 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/georaster.svg
--rw-rw-rw-   0        0        0     3428 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/group_box.svg
--rw-rw-rw-   0        0        0     5920 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/image.svg
--rw-rw-rw-   0        0        0     6133 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/import.svg
--rw-rw-rw-   0        0        0    10021 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/import_deposit.svg
--rw-rw-rw-   0        0        0     7261 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/import_external.svg
--rw-rw-rw-   0        0        0     3920 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/line_edit.svg
--rw-rw-rw-   0        0        0     4589 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/link.svg
--rw-rw-rw-   0        0        0     8564 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/link_class.svg
--rw-rw-rw-   0        0        0     7415 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/link_db.svg
--rw-rw-rw-   0        0        0     5391 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/link_file.svg
--rw-rw-rw-   0        0        0    10641 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/link_server.svg
--rw-rw-rw-   0        0        0    10832 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/load_external.svg
--rw-rw-rw-   0        0        0     8232 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/merge_linked.svg
--rw-rw-rw-   0        0        0    15565 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/merge_objects.svg
--rw-rw-rw-   0        0        0     3922 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/multi_group_box.svg
--rw-rw-rw-   0        0        0     3685 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/new_file.svg
--rw-rw-rw-   0        0        0     2284 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/next_small.svg
--rw-rw-rw-   0        0        0     2382 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/nodes.svg
--rw-rw-rw-   0        0        0      548 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/obj_id.svg
--rw-rw-rw-   0        0        0     4212 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/object.svg
--rw-rw-rw-   0        0        0     4050 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/open.svg
--rw-rw-rw-   0        0        0     3334 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/paste.svg
--rw-rw-rw-   0        0        0     3945 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/plain_text_edit.svg
--rw-rw-rw-   0        0        0     2288 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/previous_small.svg
--rw-rw-rw-   0        0        0     4145 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/query.svg
--rw-rw-rw-   0        0        0     8850 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remote_file.svg
--rw-rw-rw-   0        0        0    12527 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remote_georaster.svg
--rw-rw-rw-   0        0        0     8475 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remote_image.svg
--rw-rw-rw-   0        0        0     5888 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remove_class.svg
--rw-rw-rw-   0        0        0     7182 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remove_descriptor.svg
--rw-rw-rw-   0        0        0    14417 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remove_duplicate_objects.svg
--rw-rw-rw-   0        0        0     4358 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remove_object.svg
--rw-rw-rw-   0        0        0     5394 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/remove_query.svg
--rw-rw-rw-   0        0        0     3812 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/rename.svg
--rw-rw-rw-   0        0        0    10046 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/save.svg
--rw-rw-rw-   0        0        0    13848 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/save_pdf.svg
--rw-rw-rw-   0        0        0     2401 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/search.svg
--rw-rw-rw-   0        0        0     3506 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/select.svg
--rw-rw-rw-   0        0        0     5840 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/shapefile.svg
--rw-rw-rw-   0        0        0      983 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/slider_handle.png
--rw-rw-rw-   0        0        0    27808 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/split_objects.svg
--rw-rw-rw-   0        0        0    10041 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/table.svg
--rw-rw-rw-   0        0        0     3678 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/to_object.svg
--rw-rw-rw-   0        0        0     2665 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/trash.svg
--rw-rw-rw-   0        0        0     2665 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/trash_closed.svg
--rw-rw-rw-   0        0        0     2726 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/trash_open.svg
--rw-rw-rw-   0        0        0     5674 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/unlink.svg
--rw-rw-rw-   0        0        0     2292 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/up_small.svg
--rw-rw-rw-   0        0        0     2298 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/up_small_black.svg
--rw-rw-rw-   0        0        0     4730 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/xlsxfile.svg
--rw-rw-rw-   0        0        0     3088 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/zoom_in.svg
--rw-rw-rw-   0        0        0     2609 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/zoom_out.svg
--rw-rw-rw-   0        0        0     3956 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/res/zoom_reset.svg
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.965042 deposit_gui-1.4.44/src/deposit_gui/utils/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/utils/__init__.py
--rw-rw-rw-   0        0        0     5455 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/utils/fnc_svg.py
--rw-rw-rw-   0        0        0     2971 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/utils/fnc_thumbnails.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.965042 deposit_gui-1.4.44/src/deposit_gui/view/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/__init__.py
--rw-rw-rw-   0        0        0     1859 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/view.py
--rw-rw-rw-   0        0        0     5495 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.980673 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/__init__.py
--rw-rw-rw-   0        0        0      426 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/abstract_mdiarea_frame.py
--rw-rw-rw-   0        0        0      430 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/abstract_outside_frame.py
--rw-rw-rw-   0        0        0     5557 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/class_graph_frame.py
--rw-rw-rw-   0        0        0     7116 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/external_frame.py
--rw-rw-rw-   0        0        0    14153 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.996286 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/__init__.py
--rw-rw-rw-   0        0        0     3491 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_drag_model.py
--rw-rw-rw-   0        0        0      272 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_query_tab.py
--rw-rw-rw-   0        0        0     4669 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_item.py
--rw-rw-rw-   0        0        0     6781 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_graph.py
--rw-rw-rw-   0        0        0    10774 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_images.py
--rw-rw-rw-   0        0        0     9581 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_table.py
--rw-rw-rw-   0        0        0     4272 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/relation_frame.py
--rw-rw-rw-   0        0        0     5280 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.996286 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/__init__.py
--rw-rw-rw-   0        0        0     4924 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/class_list.py
--rw-rw-rw-   0        0        0     4709 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/class_widget.py
--rw-rw-rw-   0        0        0     1182 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/query_list.py
--rw-rw-rw-   0        0        0     2278 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/query_widget.py
--rw-rw-rw-   0        0        0     1509 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vquerytoolbar.py
--rw-rw-rw-   0        0        0     6369 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:41.996286 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:42.011904 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/__init__.py
--rw-rw-rw-   0        0        0      541 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_column.py
--rw-rw-rw-   0        0        0     6121 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_controls.py
--rw-rw-rw-   0        0        0     7531 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_entry_form.py
--rw-rw-rw-   0        0        0     6854 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_form.py
--rw-rw-rw-   0        0        0     1297 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_frame.py
--rw-rw-rw-   0        0        0     4819 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_group.py
--rw-rw-rw-   0        0        0     4112 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_multi_group.py
--rw-rw-rw-   0        0        0     1446 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_search_form.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:42.034037 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/__init__.py
--rw-rw-rw-   0        0        0     5346 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_actions.py
--rw-rw-rw-   0        0        0      451 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_column.py
--rw-rw-rw-   0        0        0     3309 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_controls.py
--rw-rw-rw-   0        0        0    11001 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_form.py
--rw-rw-rw-   0        0        0     2275 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_frame.py
--rw-rw-rw-   0        0        0     4136 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_group.py
--rw-rw-rw-   0        0        0     2005 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_query.py
--rw-rw-rw-   0        0        0     1830 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_select.py
--rw-rw-rw-   0        0        0     1580 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_unique.py
--rw-rw-rw-   0        0        0     7671 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/manager.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:42.049662 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/
--rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/__init__.py
--rw-rw-rw-   0        0        0      242 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/column_break.py
--rw-rw-rw-   0        0        0      485 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/entry_form.py
--rw-rw-rw-   0        0        0     1054 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/query.py
--rw-rw-rw-   0        0        0      490 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/search_form.py
--rw-rw-rw-   0        0        0     2210 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_controls.py
--rw-rw-rw-   0        0        0      153 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_element.py
--rw-rw-rw-   0        0        0      510 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_element_list.py
--rw-rw-rw-   0        0        0      741 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_groups.py
--rw-rw-rw-   0        0        0      411 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_labeled_element.py
--rw-rw-rw-   0        0        0      408 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_select.py
--rw-rw-rw-   0        0        0      628 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_tool.py
--rw-rw-rw-   0        0        0      330 2024-02-29 11:43:21.000000 deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_unique.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:49:42.049662 deposit_gui-1.4.44/src/deposit_gui.egg-info/
--rw-rw-rw-   0        0        0     2900 2024-02-29 14:49:41.000000 deposit_gui-1.4.44/src/deposit_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12634 2024-02-29 14:49:41.000000 deposit_gui-1.4.44/src/deposit_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 14:49:41.000000 deposit_gui-1.4.44/src/deposit_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-02-29 14:49:41.000000 deposit_gui-1.4.44/src/deposit_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-29 14:49:41.000000 deposit_gui-1.4.44/src/deposit_gui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:13.023412 deposit_gui-1.4.46/
+-rw-rw-rw-   0        0        0    35821 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/LICENSE
+-rw-rw-rw-   0        0        0     2900 2024-05-26 18:22:13.023412 deposit_gui-1.4.46/PKG-INFO
+-rw-rw-rw-   0        0        0     2117 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/README.md
+-rw-rw-rw-   0        0        0       97 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-26 18:22:13.039044 deposit_gui-1.4.46/setup.cfg
+-rw-rw-rw-   0        0        0     2073 2024-05-26 18:21:56.000000 deposit_gui-1.4.46/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.453170 deposit_gui-1.4.46/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.522161 deposit_gui-1.4.46/src/deposit_gui/
+-rw-rw-rw-   0        0        0    35821 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/LICENSE
+-rw-rw-rw-   0        0        0      893 2024-05-26 18:19:01.000000 deposit_gui-1.4.46/src/deposit_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.569039 deposit_gui-1.4.46/src/deposit_gui/controller/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/__init__.py
+-rw-rw-rw-   0        0        0    15701 2024-05-15 07:09:24.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cactions.py
+-rw-rw-rw-   0        0        0    18641 2024-02-29 09:51:52.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cdialogs.py
+-rw-rw-rw-   0        0        0     9110 2024-05-26 17:57:12.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cmdiarea.py
+-rw-rw-rw-   0        0        0     3923 2024-02-29 10:02:23.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cmodel.py
+-rw-rw-rw-   0        0        0     3891 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cnavigator.py
+-rw-rw-rw-   0        0        0     4368 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/controller.py
+-rw-rw-rw-   0        0        0      718 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cquerytoolbar.py
+-rw-rw-rw-   0        0        0     7601 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cusertools.py
+-rw-rw-rw-   0        0        0     2650 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/controller/cview.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.615906 deposit_gui-1.4.46/src/deposit_gui/dgui/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/__init__.py
+-rw-rw-rw-   0        0        0      181 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/abstract_subcontroller.py
+-rw-rw-rw-   0        0        0      889 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/abstract_subview.py
+-rw-rw-rw-   0        0        0     2709 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dcactions.py
+-rw-rw-rw-   0        0        0     2895 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dcdialogs.py
+-rw-rw-rw-   0        0        0      486 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dclickable_logo.py
+-rw-rw-rw-   0        0        0    15038 2024-02-29 09:57:20.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dcmodel.py
+-rw-rw-rw-   0        0        0     2925 2024-02-29 10:46:53.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_frame.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.622414 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/__init__.py
+-rw-rw-rw-   0        0        0     3349 2024-02-29 12:00:02.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/abstract_tab_file.py
+-rw-rw-rw-   0        0        0     8590 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db.py
+-rw-rw-rw-   0        0        0      230 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db_rel.py
+-rw-rw-rw-   0        0        0      145 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_json.py
+-rw-rw-rw-   0        0        0      815 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_memory.py
+-rw-rw-rw-   0        0        0      149 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_pickle.py
+-rw-rw-rw-   0        0        0     2677 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_recent.py
+-rw-rw-rw-   0        0        0     2005 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/ddialog.py
+-rw-rw-rw-   0        0        0    29511 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dgraph_view.py
+-rw-rw-rw-   0        0        0     3184 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dgraphics_view.py
+-rw-rw-rw-   0        0        0     1209 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dlogging.py
+-rw-rw-rw-   0        0        0     2663 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dmain_window.py
+-rw-rw-rw-   0        0        0     1207 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dmenu_bar.py
+-rw-rw-rw-   0        0        0    11285 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dmodel.py
+-rw-rw-rw-   0        0        0     2270 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dnotification.py
+-rw-rw-rw-   0        0        0     1046 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dprogress.py
+-rw-rw-rw-   0        0        0     2264 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dregistry.py
+-rw-rw-rw-   0        0        0     1771 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dsave_as_postgres_frame.py
+-rw-rw-rw-   0        0        0      290 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dstatus_bar.py
+-rw-rw-rw-   0        0        0     4921 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dtool_bar.py
+-rw-rw-rw-   0        0        0      857 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dvactions.py
+-rw-rw-rw-   0        0        0      815 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dvdialogs.py
+-rw-rw-rw-   0        0        0     4228 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/dview.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.753952 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/__init__.py
+-rwxrwxrwx   0        0        0    13312 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/acyclic.exe
+-rwxrwxrwx   0        0        0    17408 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/bcomps.exe
+-rw-rw-rw-   0        0        0  1506816 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cairo.dll
+-rwxrwxrwx   0        0        0    23040 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/ccomps.exe
+-rw-rw-rw-   0        0        0    24576 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cdt.dll
+-rw-rw-rw-   0        0        0    11264 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cgraph++.dll
+-rw-rw-rw-   0        0        0    75264 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cgraph.dll
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/circo.exe
+-rw-rw-rw-   0        0        0   317216 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/concrt140.dll
+-rw-rw-rw-   0        0        0     3057 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/config6
+-rwxrwxrwx   0        0        0    16896 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dijkstra.exe
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dot.exe
+-rwxrwxrwx   0        0        0    37376 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dot2gxl.exe
+-rwxrwxrwx   0        0        0   235008 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/edgepaint.exe
+-rw-rw-rw-   0        0        0   184832 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/expat.dll
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/fdp.exe
+-rw-rw-rw-   0        0        0   830976 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/fontconfig.dll
+-rwxrwxrwx   0        0        0    15872 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gc.exe
+-rw-rw-rw-   0        0        0    19968 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/getopt.dll
+-rw-rw-rw-   0        0        0  1374208 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/glib-2.dll
+-rwxrwxrwx   0        0        0    36864 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gml2gv.exe
+-rw-rw-rw-   0        0        0   276480 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gobject-2.dll
+-rwxrwxrwx   0        0        0    22016 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/graphml2gv.exe
+-rwxrwxrwx   0        0        0    22016 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gv2gml.exe
+-rw-rw-rw-   0        0        0    17408 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvc++.dll
+-rw-rw-rw-   0        0        0   551424 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvc.dll
+-rwxrwxrwx   0        0        0    36864 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvcolor.exe
+-rwxrwxrwx   0        0        0    25088 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvgen.exe
+-rwxrwxrwx   0        0        0   311808 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvmap.exe
+-rw-rw-rw-   0        0        0     2386 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvmap.sh
+-rwxrwxrwx   0        0        0    33792 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvpack.exe
+-rw-rw-rw-   0        0        0   122368 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_core.dll
+-rw-rw-rw-   0        0        0   156160 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_dot_layout.dll
+-rw-rw-rw-   0        0        0    31744 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_gdiplus.dll
+-rw-rw-rw-   0        0        0   374272 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_neato_layout.dll
+-rw-rw-rw-   0        0        0    38912 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_pango.dll
+-rw-rw-rw-   0        0        0    43520 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_visio.dll
+-rwxrwxrwx   0        0        0   329728 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvpr.exe
+-rwxrwxrwx   0        0        0    37376 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gxl2gv.exe
+-rw-rw-rw-   0        0        0   922112 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/libharfbuzz-0.dll
+-rwxrwxrwx   0        0        0    33792 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/mm2gv.exe
+-rw-rw-rw-   0        0        0   590096 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140.dll
+-rw-rw-rw-   0        0        0    31528 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_1.dll
+-rw-rw-rw-   0        0        0   193312 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_2.dll
+-rw-rw-rw-   0        0        0    27424 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_codecvt_ids.dll
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/neato.exe
+-rwxrwxrwx   0        0        0    12800 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/nop.exe
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/osage.exe
+-rw-rw-rw-   0        0        0   287744 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pango-1.dll
+-rw-rw-rw-   0        0        0   612864 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangocairo-1.dll
+-rw-rw-rw-   0        0        0   639488 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangoft2-1.dll
+-rw-rw-rw-   0        0        0    65536 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangowin32-1.dll
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/patchwork.exe
+-rw-rw-rw-   0        0        0    39936 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pathplan.dll
+-rw-rw-rw-   0        0        0   578560 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pixman-1.dll
+-rwxrwxrwx   0        0        0    17920 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/sccmap.exe
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/sfdp.exe
+-rwxrwxrwx   0        0        0    16384 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/tred.exe
+-rwxrwxrwx   0        0        0    10752 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/twopi.exe
+-rwxrwxrwx   0        0        0    16384 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/unflatten.exe
+-rw-rw-rw-   0        0        0   101664 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/vcruntime140.dll
+-rw-rw-rw-   0        0        0    44328 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/vcruntime140_1.dll
+-rw-rw-rw-   0        0        0    25600 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/xdot.dll
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.769541 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/
+-rw-rw-rw-   0        0        0        5 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/INSTALLER
+-rw-rw-rw-   0        0        0     1655 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/LICENSE
+-rw-rw-rw-   0        0        0     2899 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/METADATA
+-rw-rw-rw-   0        0        0      958 2024-02-29 14:13:30.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/__init__.py
+-rw-rw-rw-   0        0        0   103424 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/_graphviz.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   217528 2024-02-29 13:56:03.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/_graphviz.cpython-310-darwin.so
+-rw-rw-rw-   0        0        0    72375 2024-02-29 14:14:24.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/agraph.py
+-rw-rw-rw-   0        0        0     9298 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz.i
+-rw-rw-rw-   0        0        0     7202 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz.py
+-rw-rw-rw-   0        0        0   194463 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz_wrap.c
+-rw-rw-rw-   0        0        0     2861 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/scraper.py
+-rw-rw-rw-   0        0        0      609 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/testing.py
+-rw-rw-rw-   0        0        0      500 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dgui_main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.785165 deposit_gui-1.4.46/src/deposit_gui/dialogs/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/__init__.py
+-rw-rw-rw-   0        0        0     1384 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_about.py
+-rw-rw-rw-   0        0        0     2297 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_add_relation.py
+-rw-rw-rw-   0        0        0      907 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_connect.py
+-rw-rw-rw-   0        0        0     5158 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_import_external.py
+-rw-rw-rw-   0        0        0      264 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_import_source.py
+-rw-rw-rw-   0        0        0     1383 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_import_store.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.923174 deposit_gui-1.4.46/src/deposit_gui/res/
+-rw-rw-rw-   0        0        0     3997 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/3d_obj.svg
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/__init__.py
+-rw-rw-rw-   0        0        0     4468 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add.svg
+-rw-rw-rw-   0        0        0     5809 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_class.svg
+-rw-rw-rw-   0        0        0     7103 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_descriptor.svg
+-rw-rw-rw-   0        0        0     6328 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_form.svg
+-rw-rw-rw-   0        0        0     4271 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_object.svg
+-rw-rw-rw-   0        0        0     4990 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_query.svg
+-rw-rw-rw-   0        0        0     3249 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/add_search.svg
+-rw-rw-rw-   0        0        0     5252 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/attributes.svg
+-rw-rw-rw-   0        0        0     4497 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/attributes_simple.svg
+-rw-rw-rw-   0        0        0     4286 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/bold.svg
+-rw-rw-rw-   0        0        0     7721 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/calculator.svg
+-rw-rw-rw-   0        0        0     3173 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/check_box.svg
+-rw-rw-rw-   0        0        0     4812 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/class.svg
+-rw-rw-rw-   0        0        0    24326 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/classes_graph.svg
+-rw-rw-rw-   0        0        0     3364 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/column_break.svg
+-rw-rw-rw-   0        0        0     4186 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/combo_box.svg
+-rw-rw-rw-   0        0        0     5820 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/connect.svg
+-rw-rw-rw-   0        0        0     6697 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/copy.svg
+-rw-rw-rw-   0        0        0     3691 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/database.svg
+-rw-rw-rw-   0        0        0     2805 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/delete.svg
+-rw-rw-rw-   0        0        0     3518 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/dep_cube.svg
+-rw-rw-rw-   0        0        0    14186 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/dep_installer.svg
+-rw-rw-rw-   0        0        0     5443 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/deposit_logo.svg
+-rw-rw-rw-   0        0        0     6188 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/descriptor.svg
+-rw-rw-rw-   0        0        0     5845 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/disconnect.svg
+-rw-rw-rw-   0        0        0     7401 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/dock.svg
+-rw-rw-rw-   0        0        0     2293 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/down_small.svg
+-rw-rw-rw-   0        0        0     2298 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/down_small_black.svg
+-rw-rw-rw-   0        0        0     7023 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/draw_polygon.svg
+-rw-rw-rw-   0        0        0     4896 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/edit.svg
+-rw-rw-rw-   0        0        0     6722 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/edit_class.svg
+-rw-rw-rw-   0        0        0     6378 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/edit_query.svg
+-rw-rw-rw-   0        0        0     3862 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/export_deposit.svg
+-rw-rw-rw-   0        0        0    12377 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/export_external.svg
+-rw-rw-rw-   0        0        0     4772 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/file.svg
+-rw-rw-rw-   0        0        0     5462 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/form.svg
+-rw-rw-rw-   0        0        0     3916 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/geometry.svg
+-rw-rw-rw-   0        0        0     9955 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/georaster.svg
+-rw-rw-rw-   0        0        0     3428 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/group_box.svg
+-rw-rw-rw-   0        0        0     5920 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/image.svg
+-rw-rw-rw-   0        0        0     6133 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/import.svg
+-rw-rw-rw-   0        0        0    10021 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/import_deposit.svg
+-rw-rw-rw-   0        0        0     7261 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/import_external.svg
+-rw-rw-rw-   0        0        0     3920 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/line_edit.svg
+-rw-rw-rw-   0        0        0     4589 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/link.svg
+-rw-rw-rw-   0        0        0     8564 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/link_class.svg
+-rw-rw-rw-   0        0        0     7415 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/link_db.svg
+-rw-rw-rw-   0        0        0     5391 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/link_file.svg
+-rw-rw-rw-   0        0        0    10641 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/link_server.svg
+-rw-rw-rw-   0        0        0    10832 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/load_external.svg
+-rw-rw-rw-   0        0        0     8232 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/merge_linked.svg
+-rw-rw-rw-   0        0        0    15565 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/merge_objects.svg
+-rw-rw-rw-   0        0        0     3922 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/multi_group_box.svg
+-rw-rw-rw-   0        0        0     3685 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/new_file.svg
+-rw-rw-rw-   0        0        0     2284 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/next_small.svg
+-rw-rw-rw-   0        0        0     2382 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/nodes.svg
+-rw-rw-rw-   0        0        0      548 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/obj_id.svg
+-rw-rw-rw-   0        0        0     4212 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/object.svg
+-rw-rw-rw-   0        0        0     4050 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/open.svg
+-rw-rw-rw-   0        0        0     3334 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/paste.svg
+-rw-rw-rw-   0        0        0     3945 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/plain_text_edit.svg
+-rw-rw-rw-   0        0        0     2288 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/previous_small.svg
+-rw-rw-rw-   0        0        0     4145 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/query.svg
+-rw-rw-rw-   0        0        0     8850 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remote_file.svg
+-rw-rw-rw-   0        0        0    12527 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remote_georaster.svg
+-rw-rw-rw-   0        0        0     8475 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remote_image.svg
+-rw-rw-rw-   0        0        0     5888 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remove_class.svg
+-rw-rw-rw-   0        0        0     7182 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remove_descriptor.svg
+-rw-rw-rw-   0        0        0    14417 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remove_duplicate_objects.svg
+-rw-rw-rw-   0        0        0     4358 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remove_object.svg
+-rw-rw-rw-   0        0        0     5394 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/remove_query.svg
+-rw-rw-rw-   0        0        0     3812 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/rename.svg
+-rw-rw-rw-   0        0        0    10046 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/save.svg
+-rw-rw-rw-   0        0        0    13848 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/save_pdf.svg
+-rw-rw-rw-   0        0        0     2401 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/search.svg
+-rw-rw-rw-   0        0        0     3506 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/select.svg
+-rw-rw-rw-   0        0        0     5840 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/shapefile.svg
+-rw-rw-rw-   0        0        0      983 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/slider_handle.png
+-rw-rw-rw-   0        0        0    27808 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/split_objects.svg
+-rw-rw-rw-   0        0        0    10041 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/table.svg
+-rw-rw-rw-   0        0        0     3678 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/to_object.svg
+-rw-rw-rw-   0        0        0     2665 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/trash.svg
+-rw-rw-rw-   0        0        0     2665 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/trash_closed.svg
+-rw-rw-rw-   0        0        0     2726 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/trash_open.svg
+-rw-rw-rw-   0        0        0     5674 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/unlink.svg
+-rw-rw-rw-   0        0        0     2292 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/up_small.svg
+-rw-rw-rw-   0        0        0     2298 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/up_small_black.svg
+-rw-rw-rw-   0        0        0     4730 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/xlsxfile.svg
+-rw-rw-rw-   0        0        0     3088 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/zoom_in.svg
+-rw-rw-rw-   0        0        0     2609 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/zoom_out.svg
+-rw-rw-rw-   0        0        0     3956 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/res/zoom_reset.svg
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.938804 deposit_gui-1.4.46/src/deposit_gui/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/utils/__init__.py
+-rw-rw-rw-   0        0        0     5455 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/utils/fnc_svg.py
+-rw-rw-rw-   0        0        0     2971 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/utils/fnc_thumbnails.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.938804 deposit_gui-1.4.46/src/deposit_gui/view/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/__init__.py
+-rw-rw-rw-   0        0        0     1859 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/view.py
+-rw-rw-rw-   0        0        0     5495 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.954419 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/__init__.py
+-rw-rw-rw-   0        0        0      426 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/abstract_mdiarea_frame.py
+-rw-rw-rw-   0        0        0      430 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/abstract_outside_frame.py
+-rw-rw-rw-   0        0        0     5557 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/class_graph_frame.py
+-rw-rw-rw-   0        0        0     7116 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/external_frame.py
+-rw-rw-rw-   0        0        0    14465 2024-05-15 07:39:48.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.970042 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/__init__.py
+-rw-rw-rw-   0        0        0     3491 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_drag_model.py
+-rw-rw-rw-   0        0        0      272 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_query_tab.py
+-rw-rw-rw-   0        0        0     4669 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_item.py
+-rw-rw-rw-   0        0        0     6810 2024-05-15 07:25:23.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_graph.py
+-rw-rw-rw-   0        0        0    10774 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_images.py
+-rw-rw-rw-   0        0        0     9763 2024-05-15 07:39:32.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_table.py
+-rw-rw-rw-   0        0        0     4272 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/relation_frame.py
+-rw-rw-rw-   0        0        0     5280 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.970042 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/__init__.py
+-rw-rw-rw-   0        0        0     4924 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/class_list.py
+-rw-rw-rw-   0        0        0     4709 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/class_widget.py
+-rw-rw-rw-   0        0        0     1182 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/query_list.py
+-rw-rw-rw-   0        0        0     2278 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/query_widget.py
+-rw-rw-rw-   0        0        0     1509 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vquerytoolbar.py
+-rw-rw-rw-   0        0        0     6369 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.970042 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:12.985662 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/__init__.py
+-rw-rw-rw-   0        0        0      541 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_column.py
+-rw-rw-rw-   0        0        0     6121 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_controls.py
+-rw-rw-rw-   0        0        0     7531 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_entry_form.py
+-rw-rw-rw-   0        0        0     6854 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_form.py
+-rw-rw-rw-   0        0        0     1297 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_frame.py
+-rw-rw-rw-   0        0        0     4819 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_group.py
+-rw-rw-rw-   0        0        0     4112 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_multi_group.py
+-rw-rw-rw-   0        0        0     1446 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_search_form.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:13.001309 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/__init__.py
+-rw-rw-rw-   0        0        0     5346 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_actions.py
+-rw-rw-rw-   0        0        0      451 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_column.py
+-rw-rw-rw-   0        0        0     3309 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_controls.py
+-rw-rw-rw-   0        0        0    11001 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_form.py
+-rw-rw-rw-   0        0        0     2275 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_frame.py
+-rw-rw-rw-   0        0        0     4136 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_group.py
+-rw-rw-rw-   0        0        0     2005 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_query.py
+-rw-rw-rw-   0        0        0     1830 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_select.py
+-rw-rw-rw-   0        0        0     1580 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_unique.py
+-rw-rw-rw-   0        0        0     7671 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/manager.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:13.023412 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/__init__.py
+-rw-rw-rw-   0        0        0      242 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/column_break.py
+-rw-rw-rw-   0        0        0      485 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/entry_form.py
+-rw-rw-rw-   0        0        0     1054 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/query.py
+-rw-rw-rw-   0        0        0      490 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/search_form.py
+-rw-rw-rw-   0        0        0     2210 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_controls.py
+-rw-rw-rw-   0        0        0      153 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_element.py
+-rw-rw-rw-   0        0        0      510 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_element_list.py
+-rw-rw-rw-   0        0        0      741 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_groups.py
+-rw-rw-rw-   0        0        0      411 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_labeled_element.py
+-rw-rw-rw-   0        0        0      408 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_select.py
+-rw-rw-rw-   0        0        0      628 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_tool.py
+-rw-rw-rw-   0        0        0      330 2024-02-29 11:43:21.000000 deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_unique.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:22:13.023412 deposit_gui-1.4.46/src/deposit_gui.egg-info/
+-rw-rw-rw-   0        0        0     2900 2024-05-26 18:22:12.000000 deposit_gui-1.4.46/src/deposit_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12634 2024-05-26 18:22:12.000000 deposit_gui-1.4.46/src/deposit_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:22:12.000000 deposit_gui-1.4.46/src/deposit_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-26 18:22:12.000000 deposit_gui-1.4.46/src/deposit_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 18:22:12.000000 deposit_gui-1.4.46/src/deposit_gui.egg-info/top_level.txt
```

### Comparing `deposit_gui-1.4.44/LICENSE` & `deposit_gui-1.4.46/LICENSE`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/PKG-INFO` & `deposit_gui-1.4.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: deposit_gui
-Version: 1.4.44
+Version: 1.4.46
 Summary: GUI for Deposit: Graph database focused on scientific data collection
 Home-page: https://github.com/demjanp/deposit_gui
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deposit<1.5,>=1.4.41
+Requires-Dist: deposit<1.5,>=1.4.42
 Requires-Dist: svgelements<2,>=1.8.1
 
 # <img src="dep_cube.svg" width="32">Deposit GUI
 GUI for [Deposit](https://github.com/demjanp/deposit): Graph database focused on scientific data collection.
 
 Created on 29. 4. 2013
```

### Comparing `deposit_gui-1.4.44/README.md` & `deposit_gui-1.4.46/README.md`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/setup.py` & `deposit_gui-1.4.46/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 #!/usr/bin/env python
 #
 
 from setuptools import setup, find_packages
 
 import pathlib
 
+import ast
+import os
+
+def get_version():
+	with open(os.path.join(os.path.dirname(__file__), 'src', 'deposit_gui', '__init__.py')) as f:
+		tree = ast.parse(f.read())
+		for node in tree.body:
+			if isinstance(node, ast.Assign):
+				if node.targets[0].id == 'version_info':
+					return '.'.join(map(str, ast.literal_eval(node.value)))
+
 try:
     from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
     class bdist_wheel(_bdist_wheel):
         def finalize_options(self):
             _bdist_wheel.finalize_options(self)
             self.root_is_pure = False
 except ImportError:
@@ -17,15 +28,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="deposit_gui",
-    version="1.4.44",
+    version=get_version(),
     description="GUI for Deposit: Graph database focused on scientific data collection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/demjanp/deposit_gui",
     author="Peter Demjan",
     author_email="peter.demjan@gmail.com",
     classifiers=[
@@ -53,12 +64,12 @@
 		"*.pyd",
 		"*.so",
 		"*.png",
 		"*.svg",
 	]},
     python_requires=">=3.10, <4",
 	install_requires=[
-		'deposit>=1.4.41, <1.5',
+		'deposit>=1.4.42, <1.5',
 		'svgelements>=1.8.1, <2',
 	],
 	cmdclass={'bdist_wheel': bdist_wheel},
 )
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/LICENSE` & `deposit_gui-1.4.46/src/deposit_gui/LICENSE`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/__init__.py` & `deposit_gui-1.4.46/src/deposit_gui/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-version_info = (1, 4, 44)
+version_info = (1, 4, 46)
 
 __version__ = '.'.join(map(str, version_info))
 __title__ = 'Deposit'
-__date__ = "29.2.2024"
+__date__ = "26.5.2024"
 
 from deposit_gui.dgui_main import DGUIMain
 
 from deposit_gui.dgui.abstract_subcontroller import AbstractSubcontroller
 from deposit_gui.dgui.abstract_subview import AbstractSubview
 from deposit_gui.dgui.dclickable_logo import DClickableLogo
 from deposit_gui.dgui.dconnect_frame import DConnectFrame
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cactions.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,29 +359,21 @@
 		)
 	
 	def on_FieldCalculator(self, state):
 		
 		frame = self.cmain.cmdiarea.get_current_frame()
 		if not isinstance(frame, QueryFrame):
 			return
-		rows = {}
-		for row in range(frame.get_row_count()):
-			obj_id = frame.get_item(row, 0).obj_id_row
-			if obj_id is None:
-				continue
-			rows[obj_id] = {}
-			for col in range(frame.get_column_count()):
-				item = frame.get_item(row, col)
-				rows[obj_id][(item.class_name, item.descriptor_name)] = item.value
+		data = frame.get_data()
 		descriptor_name = None
 		items = self.cmain.get_selected_queryitems()
 		if items:
 			descriptor_name = list(items)[0].descriptor_name
-		if rows:
-			self.cmain.cdialogs.open("FieldCalculator", rows, descriptor_name)
+		if data:
+			self.cmain.cdialogs.open("FieldCalculator", data, descriptor_name)
 	
 	
 	def update_MergeRows(self):
 		
 		items = self.cmain.get_selected_queryitems()
 		objects = set([item.obj_id_row for item in items])
 		return dict(
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cdialogs.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cdialogs.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cmdiarea.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cmdiarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 	def on_class_link(self, name):
 		
 		self.add_query("SELECT [%s].*" % (name))
 	
 	@QtCore.Slot(int, str, str)
 	def on_relation_link(self, obj_id, label, name_tgt):
 		
-		self.add_query("SELECT [%s].*, OBJ(%d).* RELATED OBJ(%d).[%s].[%s]" % (name_tgt, obj_id, obj_id, label, name_tgt))
+		self.add_query("SELECT [%s].* WHERE RELATED(OBJ(%d), [%s], '%s')" % (name_tgt, obj_id, name_tgt, label))
 	
 	@QtCore.Slot(int, str, str)
 	def on_relation_unlink(self, obj_id, label, name_tgt):
 		
 		obj = self.cmain.cmodel.get_object(obj_id)
 		to_del = []
 		for obj_tgt, label_ in obj.get_relations():
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cmodel.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cmodel.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cnavigator.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cnavigator.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/controller.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/controller.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cquerytoolbar.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cquerytoolbar.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cusertools.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cusertools.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/controller/cview.py` & `deposit_gui-1.4.46/src/deposit_gui/controller/cview.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/abstract_subview.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/abstract_subview.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dcactions.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dcactions.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dcdialogs.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dcdialogs.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dcmodel.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dcmodel.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/abstract_tab_file.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/abstract_tab_file.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_db.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_memory.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_memory.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_recent.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dconnect_tabs/dconnect_tab_recent.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/ddialog.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/ddialog.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dgraph_view.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dgraph_view.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dgraphics_view.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dgraphics_view.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dlogging.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dlogging.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dmain_window.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dmain_window.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dmenu_bar.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dmenu_bar.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dmodel.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dmodel.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dnotification.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dnotification.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dprogress.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dprogress.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dregistry.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dregistry.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dsave_as_postgres_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dsave_as_postgres_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dtool_bar.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dtool_bar.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dvactions.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dvactions.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dvdialogs.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dvdialogs.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/dview.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/dview.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/acyclic.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/acyclic.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/bcomps.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/bcomps.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cairo.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cairo.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/ccomps.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/ccomps.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cdt.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cdt.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cgraph++.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cgraph++.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/cgraph.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/cgraph.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/circo.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/circo.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/concrt140.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/concrt140.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/config6` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/config6`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dijkstra.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dijkstra.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dot.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dot.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/dot2gxl.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/dot2gxl.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/edgepaint.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/edgepaint.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/expat.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/expat.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/fdp.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/fdp.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/fontconfig.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/fontconfig.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gc.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gc.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/getopt.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/getopt.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/glib-2.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/glib-2.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gml2gv.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gml2gv.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gobject-2.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gobject-2.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/graphml2gv.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/graphml2gv.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gv2gml.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gv2gml.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvc++.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvc++.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvc.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvc.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvcolor.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvcolor.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvgen.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvgen.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvmap.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvmap.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvmap.sh` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvmap.sh`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvpack.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvpack.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_core.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_core.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_dot_layout.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_dot_layout.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_gdiplus.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_gdiplus.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_neato_layout.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_neato_layout.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_pango.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_pango.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvplugin_visio.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvplugin_visio.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gvpr.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gvpr.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/gxl2gv.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/gxl2gv.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/libharfbuzz-0.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/libharfbuzz-0.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/mm2gv.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/mm2gv.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_2.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_2.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/msvcp140_codecvt_ids.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/msvcp140_codecvt_ids.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/neato.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/neato.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/nop.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/nop.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/osage.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/osage.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pango-1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pango-1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangocairo-1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangocairo-1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangoft2-1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangoft2-1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pangowin32-1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pangowin32-1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/patchwork.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/patchwork.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pathplan.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pathplan.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/pixman-1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/pixman-1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/sccmap.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/sccmap.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/sfdp.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/sfdp.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/tred.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/tred.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/twopi.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/twopi.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/unflatten.exe` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/unflatten.exe`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/vcruntime140.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/vcruntime140_1.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/vcruntime140_1.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/graphviz/xdot.dll` & `deposit_gui-1.4.46/src/deposit_gui/dgui/graphviz/xdot.dll`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/LICENSE` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/LICENSE`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/METADATA` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/METADATA`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/__init__.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/__init__.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/_graphviz.cpython-310-darwin.so` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/_graphviz.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/agraph.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/agraph.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz.i` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz.i`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/graphviz_wrap.c` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/graphviz_wrap.c`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/scraper.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/scraper.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dgui/pygraphviz/testing.py` & `deposit_gui-1.4.46/src/deposit_gui/dgui/pygraphviz/testing.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_about.py` & `deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_about.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_add_relation.py` & `deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_add_relation.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_connect.py` & `deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_connect.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_import_external.py` & `deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_import_external.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/dialogs/dialog_import_store.py` & `deposit_gui-1.4.46/src/deposit_gui/dialogs/dialog_import_store.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/3d_obj.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/3d_obj.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_class.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_class.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_descriptor.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_descriptor.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_form.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_form.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_object.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_object.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_query.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_query.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/add_search.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/add_search.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/attributes.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/attributes.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/attributes_simple.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/attributes_simple.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/bold.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/bold.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/calculator.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/calculator.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/check_box.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/check_box.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/class.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/class.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/classes_graph.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/classes_graph.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/column_break.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/column_break.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/combo_box.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/combo_box.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/connect.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/connect.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/copy.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/copy.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/database.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/database.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/delete.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/delete.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/dep_cube.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/dep_cube.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/dep_installer.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/dep_installer.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/deposit_logo.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/deposit_logo.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/descriptor.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/descriptor.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/disconnect.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/disconnect.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/dock.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/dock.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/down_small.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/down_small.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/down_small_black.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/down_small_black.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/draw_polygon.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/draw_polygon.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/edit.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/edit.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/edit_class.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/edit_class.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/edit_query.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/edit_query.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/export_deposit.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/export_deposit.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/export_external.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/export_external.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/file.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/file.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/form.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/form.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/geometry.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/geometry.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/georaster.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/georaster.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/group_box.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/group_box.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/image.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/image.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/import.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/import.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/import_deposit.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/import_deposit.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/import_external.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/import_external.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/line_edit.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/line_edit.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/link.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/link.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/link_class.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/link_class.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/link_db.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/link_db.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/link_file.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/link_file.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/link_server.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/link_server.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/load_external.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/load_external.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/merge_linked.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/merge_linked.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/merge_objects.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/merge_objects.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/multi_group_box.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/multi_group_box.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/new_file.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/new_file.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/next_small.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/next_small.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/nodes.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/nodes.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/obj_id.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/obj_id.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/object.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/object.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/open.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/open.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/paste.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/paste.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/plain_text_edit.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/plain_text_edit.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/previous_small.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/previous_small.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/query.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/query.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remote_file.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remote_file.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remote_georaster.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remote_georaster.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remote_image.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remote_image.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remove_class.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remove_class.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remove_descriptor.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remove_descriptor.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remove_duplicate_objects.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remove_duplicate_objects.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remove_object.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remove_object.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/remove_query.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/remove_query.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/rename.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/rename.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/save.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/save.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/save_pdf.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/save_pdf.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/search.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/search.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/select.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/select.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/shapefile.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/shapefile.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/slider_handle.png` & `deposit_gui-1.4.46/src/deposit_gui/res/slider_handle.png`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/split_objects.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/split_objects.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/table.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/table.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/to_object.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/to_object.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/trash.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/trash.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/trash_closed.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/trash_closed.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/trash_open.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/trash_open.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/unlink.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/unlink.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/up_small.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/up_small.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/up_small_black.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/up_small_black.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/xlsxfile.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/xlsxfile.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/zoom_in.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/zoom_in.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/zoom_out.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/zoom_out.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/res/zoom_reset.svg` & `deposit_gui-1.4.46/src/deposit_gui/res/zoom_reset.svg`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/utils/fnc_svg.py` & `deposit_gui-1.4.46/src/deposit_gui/utils/fnc_svg.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/utils/fnc_thumbnails.py` & `deposit_gui-1.4.46/src/deposit_gui/utils/fnc_thumbnails.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/view.py` & `deposit_gui-1.4.46/src/deposit_gui/view/view.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/class_graph_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/class_graph_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/external_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/external_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 		self.tabs.setCurrentIndex(1)
 		self.tabs.blockSignals(False)
 	
 	def populate_tab_graph(self):
 		
 		if isinstance(self.tab_graph, QueryTabGraph):
 			return
-		self.tab_graph = QueryTabGraph(self, set([self._cmodel.get_object(obj_id) for obj_id in self.tab_table.get_obj_ids()]))
+		self.tab_graph = QueryTabGraph(self)
 		self.tabs.blockSignals(True)
 		self.tabs.insertTab(2, self.tab_graph, "Graph")
 		self.tabs.removeTab(3)
 		self.tabs.setCurrentIndex(2)
 		self.tabs.blockSignals(False)
 	
 	def get_current_tab(self):
@@ -169,24 +169,42 @@
 		# pass to deposit.AbstractExternalsource to provide header data from QueryTabTable
 		
 		return self.tab_table._table_model.headerData(col, QtCore.Qt.Horizontal, QtCore.Qt.UserRole if user_role else QtCore.Qt.DisplayRole)
 	
 	def get_item(self, row, col):
 		# pass to deposit.AbstractExternalsource to provide data from QueryTabTable
 		
-		return self.tab_table._table_model.index(row, col).data(QtCore.Qt.UserRole)
+		return self.tab_table.get_item(row, col)
 	
 	def get_row_count(self):
 		
 		return self.tab_table.get_row_count()
 	
 	def get_column_count(self):
 		
 		return self.tab_table.get_column_count()
 	
+	def get_object(self, obj_id):
+		
+		return self._cmodel.get_object(obj_id)
+	
+	def get_data(self):
+		# returns data = {obj_id: {(class, descriptor): value, ...}, ...}
+		
+		data = {}
+		for row in range(self.get_row_count()):
+			obj_id = self.get_item(row, 0).obj_id_row
+			if obj_id is None:
+				continue
+			data[obj_id] = {}
+			for col in range(self.get_column_count()):
+				item = self.get_item(row, col)
+				data[obj_id][(item.class_name, item.descriptor_name)] = item.value
+		return data
+		
 	@QtCore.Slot(int)
 	def on_tab_changed(self, index):
 		
 		if index == 1:
 			self.populate_tab_images()
 		elif index == 2:
 			self.populate_tab_graph()
@@ -207,15 +225,15 @@
 	@QtCore.Slot()
 	def on_filter_timer(self):
 		
 		self.tab_table.apply_filter(self.footer.get_filter_text())
 		if isinstance(self.tab_images, QueryTabImages):
 			self.tab_images.apply_filter(self.tab_table.get_item_order())
 		if isinstance(self.tab_graph, QueryTabGraph):
-			self.tab_graph.apply_filter(set([self._cmodel.get_object(obj_id) for obj_id in self.tab_table.get_obj_ids()]))
+			self.tab_graph.apply_filter()
 		self.update_count()
 	
 	@QtCore.Slot()
 	def on_sorted(self):
 		
 		self.tab_images.sort(self.tab_table.get_item_order())
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_drag_model.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/abstract_drag_model.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_item.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_item.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_graph.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,25 +21,24 @@
 	
 	def deselect_all(self):
 		
 		pass
 	
 class QueryTabGraph(AbstractQueryTab, QtWidgets.QMainWindow):
 	
-	def __init__(self, queryframe, objects):
+	def __init__(self, queryframe):
 		
 		QtWidgets.QMainWindow.__init__(self)
 		
 		self._queryframe = queryframe
 		self._query = queryframe._query
 		
 		self._actions = {} # {name: QAction, ...}
 		self._positions = {}  # {node_id: (x, y), ...}
 		self._show_attributes = 1  # 0 = show nodes only; 1 = show descriptor values; 2 = show descriptor names and values
-		self._objects = objects
 		
 		self._graph_view = DGraphView()
 		self._graph_view.signal_node_activated.connect(self.on_activated)
 		self._graph_view.signal_selected.connect(self.on_graph_selected)
 		
 		central_widget = QtWidgets.QWidget(self)
 		central_widget.setLayout(QtWidgets.QVBoxLayout())
@@ -84,57 +83,58 @@
 		
 		self.populate_graph()
 	
 	def populate_graph(self):
 		
 		self._graph_view.clear()
 		
-		if self._objects is None:
+		data = self._queryframe.get_data()
+		if data is None:
 			return
 		
 		self._queryframe._cview.progress.show("Drawing Tree")
 		
 		nodes = []  # [AbstractNode, ...]
 		edges = []  # [[source_id, target_id, label], ...]
-		for obj in self._objects:
-			
+		
+		for obj_id in data:
 			descriptors = []
 			if self._show_attributes > 0:
-				for descr in obj.get_descriptors():
-					value = obj.get_descriptor(descr)
+				for cls_name, descr_name in data[obj_id]:
+					value = data[obj_id][(cls_name, descr_name)]
 					if value.__class__.__name__ == "DDateTime":
 						value = value.isoformat
 					elif value.__class__.__name__ == "DGeometry":
 						value = value.geometry_type
 					elif value.__class__.__name__ == "DResource":
 						value = value.filename
 					else:
 						value = str(value)
-					descriptors.append([descr.name, value])
+					descriptors.append([".".join([cls_name, descr_name]), value])
 			
 			if self._show_attributes == 0:
-				nodes.append(Node(obj.id, str(obj.id)))
+				nodes.append(Node(obj_id, str(obj_id)))
 			elif self._show_attributes == 1:
-				nodes.append(NodeWithSimpleAttributes(obj.id, str(obj.id), descriptors))
+				nodes.append(NodeWithSimpleAttributes(obj_id, str(obj_id), descriptors))
 			elif self._show_attributes == 2:
-				nodes.append(NodeWithAttributes(obj.id, str(obj.id), descriptors))
+				nodes.append(NodeWithAttributes(obj_id, str(obj_id), descriptors))
 			
+			obj = self._queryframe.get_object(obj_id)
 			for obj_tgt, label in obj.get_relations():
 				if label.startswith("~"):
 					continue
-				if obj_tgt in self._objects:
-					edges.append([obj.id, obj_tgt.id, label])
+				if obj_tgt.id in data:
+					edges.append([obj_id, obj_tgt.id, label])
 		
 		self._graph_view.populate(nodes = nodes, edges = edges, positions = self._positions, progress = self._queryframe._cview.progress)
 		
 		self._queryframe._cview.progress.stop()
 	
-	def apply_filter(self, objects):
+	def apply_filter(self):
 		
-		self._objects = objects
 		if self.isVisible():
 			self.populate_graph()
 	
 	def show(self):
 		
 		QtWidgets.QMainWindow.show(self)
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_images.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_images.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_table.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/query_tab_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,19 @@
 	def select_object(self, obj_id):
 		
 		for row in range(self._table_model._proxy_model.rowCount()):
 			if self._table_model._proxy_model.index(row, 0).data(QtCore.Qt.UserRole).obj_id_row == obj_id:
 				self.selectRow(row)
 				return
 	
+	def get_item(self, row, col):
+		
+		index = self._table_model._proxy_model.index(row, col)
+		return self._table_model._proxy_model.mapToSource(index).data(QtCore.Qt.UserRole)
+	
 	def set_query_item(self, row, column, value):
 		
 		self._table_model._proxy_model.setData(self._table_model._proxy_model.index(row, column), value)
 	
 	def get_row_count(self):
 		
 		return self._table_model._proxy_model.rowCount()
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/relation_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vmdiarea_frames/query_frame_elements/relation_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vnavigator.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vnavigator.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/class_list.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/class_list.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/class_widget.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/class_widget.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/query_list.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/query_list.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vnavigator_elements/query_widget.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vnavigator_elements/query_widget.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vquerytoolbar.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vquerytoolbar.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_column.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_column.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_controls.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_controls.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_entry_form.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_entry_form.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_form.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_form.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_group.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_group.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_multi_group.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_multi_group.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/dialog/dialog_search_form.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/dialog/dialog_search_form.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_actions.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_actions.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_controls.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_controls.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_form.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_form.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_frame.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_frame.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_group.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_group.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_query.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_query.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_select.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_select.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/editor/editor_unique.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/editor/editor_unique.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/manager.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/manager.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/query.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/query.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_controls.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_controls.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_groups.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_groups.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui/view/vusertools_elements/user_elements/user_tool.py` & `deposit_gui-1.4.46/src/deposit_gui/view/vusertools_elements/user_elements/user_tool.py`

 * *Files identical despite different names*

### Comparing `deposit_gui-1.4.44/src/deposit_gui.egg-info/PKG-INFO` & `deposit_gui-1.4.46/src/deposit_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: deposit_gui
-Version: 1.4.44
+Version: 1.4.46
 Summary: GUI for Deposit: Graph database focused on scientific data collection
 Home-page: https://github.com/demjanp/deposit_gui
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: database,graph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deposit<1.5,>=1.4.41
+Requires-Dist: deposit<1.5,>=1.4.42
 Requires-Dist: svgelements<2,>=1.8.1
 
 # <img src="dep_cube.svg" width="32">Deposit GUI
 GUI for [Deposit](https://github.com/demjanp/deposit): Graph database focused on scientific data collection.
 
 Created on 29. 4. 2013
```

### Comparing `deposit_gui-1.4.44/src/deposit_gui.egg-info/SOURCES.txt` & `deposit_gui-1.4.46/src/deposit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

