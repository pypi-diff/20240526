# Comparing `tmp/jvi-0.1.3.tar.gz` & `tmp/jvi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvi-0.1.3.tar", max compression
+gzip compressed data, was "jvi-0.1.4.tar", max compression
```

## Comparing `jvi-0.1.3.tar` & `jvi-0.1.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       34 2023-11-16 06:02:37.448598 jvi-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-11-16 05:52:20.912471 jvi-0.1.3/jvi/__init__.py
--rwxr-xr-x   0        0        0     2000 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-blur-x.py
--rwxr-xr-x   0        0        0     1418 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-blur.py
--rw-r--r--   0        0        0     1199 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-box.py
--rwxr-xr-x   0        0        0     1568 2023-11-16 16:14:11.027629 jvi-0.1.3/jvi/bin/jvi-cut.py
--rwxr-xr-x   0        0        0     1935 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-ff-remux.py
--rwxr-xr-x   0        0        0      794 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-ff-split.py
--rwxr-xr-x   0        0        0     2185 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/bin/jvi-img2video.py
--rwxr-xr-x   0        0        0      947 2023-11-16 16:14:11.027629 jvi-0.1.3/jvi/bin/jvi-imp.py
--rwxr-xr-x   0        0        0     3337 2023-11-16 16:14:11.027629 jvi-0.1.3/jvi/bin/jvi-infrared.py
--rwxr-xr-x   0        0        0     1415 2023-11-16 16:14:11.027629 jvi-0.1.3/jvi/bin/jvi-letterbox.py
--rwxr-xr-x   0        0        0     1917 2023-11-16 16:14:11.027629 jvi-0.1.3/jvi/bin/jvi-resize.py
--rwxr-xr-x   0        0        0     2412 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-superres.py
--rwxr-xr-x   0        0        0     1127 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/bin/jvi-tile-dir.py
--rwxr-xr-x   0        0        0     2006 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/bin/jvi-tile-match.py
--rwxr-xr-x   0        0        0     1938 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/bin/jvi-tile-viewer.py
--rwxr-xr-x   0        0        0     1891 2023-11-16 05:52:20.928471 jvi-0.1.3/jvi/bin/jvi-tks.py
--rwxr-xr-x   0        0        0     2600 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/bin/jvi-video2img.py
--rw-r--r--   0        0        0      104 2023-11-16 05:52:20.912471 jvi-0.1.3/jvi/common.py
--rw-r--r--   0        0        0        0 2023-11-16 05:52:20.916471 jvi-0.1.3/jvi/drawing/__init__.py
--rw-r--r--   0        0        0    10301 2023-11-16 05:52:20.916471 jvi-0.1.3/jvi/drawing/color.py
--rw-r--r--   0        0        0     3497 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/drawing/shape.py
--rw-r--r--   0        0        0      322 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/__init__.py
--rw-r--r--   0        0        0     1298 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/convert.py
--rw-r--r--   0        0        0     1541 2023-11-16 05:52:20.904471 jvi-0.1.3/jvi/geo/gp.py
--rw-r--r--   0        0        0     1323 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/line_segment.py
--rw-r--r--   0        0        0     5530 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/point2d.py
--rw-r--r--   0        0        0     3749 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/polygon.py
--rw-r--r--   0        0        0      230 2023-11-16 05:52:20.904471 jvi-0.1.3/jvi/geo/protocol.py
--rw-r--r--   0        0        0    11784 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/rectangle.py
--rw-r--r--   0        0        0     6384 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/size2d.py
--rw-r--r--   0        0        0     5944 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/size2d_gp.bak
--rw-r--r--   0        0        0     1230 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/geo/trans.py
--rw-r--r--   0        0        0        0 2023-11-16 05:52:20.936472 jvi-0.1.3/jvi/gui/__init__.py
--rw-r--r--   0        0        0     2668 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/gui/image_viewer.py
--rw-r--r--   0        0        0     5293 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/gui/image_win.py
--rw-r--r--   0        0        0     1475 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/gui/imp_win.py
--rw-r--r--   0        0        0     3003 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/gui/record_viewer.py
--rw-r--r--   0        0        0     2155 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/gui/video_viewer.py
--rw-r--r--   0        0        0        0 2023-11-16 05:52:20.920471 jvi-0.1.3/jvi/image/__init__.py
--rw-r--r--   0        0        0     3226 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/image.py
--rw-r--r--   0        0        0     1200 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/image_factory.py
--rw-r--r--   0        0        0     5632 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/image_nda.py
--rw-r--r--   0        0        0     3123 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/infrared.py
--rw-r--r--   0        0        0     3772 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/io.py
--rw-r--r--   0        0        0     7552 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/proc.py
--rw-r--r--   0        0        0     3827 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/sc3c.py
--rw-r--r--   0        0        0     1913 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/stat.py
--rw-r--r--   0        0        0     4893 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/struct.py
--rw-r--r--   0        0        0     3750 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/tile.py
--rw-r--r--   0        0        0     1869 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/tile_set.py
--rw-r--r--   0        0        0     1263 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/trace.py
--rw-r--r--   0        0        0      616 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/trans.py
--rw-r--r--   0        0        0     2216 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/image/util.py
--rw-r--r--   0        0        0        0 2023-11-16 05:52:20.932471 jvi-0.1.3/jvi/match/__init__.py
--rw-r--r--   0        0        0     4956 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/match/match.py
--rw-r--r--   0        0        0     2578 2023-11-16 16:08:10.173256 jvi-0.1.3/jvi/match/match_template.py
--rw-r--r--   0        0        0        0 2023-11-17 03:53:27.240712 jvi-0.1.3/jvi/py.typed
--rw-r--r--   0        0        0      491 2023-11-17 03:53:44.824812 jvi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 jvi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-11-16 06:02:37.448598 jvi-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-11-16 05:52:20.912471 jvi-0.1.4/jvi/__init__.py
+-rwxr-xr-x   0        0        0     2000 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-blur-x.py
+-rwxr-xr-x   0        0        0     1418 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-blur.py
+-rw-r--r--   0        0        0     1199 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-box.py
+-rwxr-xr-x   0        0        0     1568 2023-11-16 16:14:11.027629 jvi-0.1.4/jvi/bin/jvi-cut.py
+-rwxr-xr-x   0        0        0     1935 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-ff-remux.py
+-rwxr-xr-x   0        0        0      794 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-ff-split.py
+-rwxr-xr-x   0        0        0     2185 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/bin/jvi-img2video.py
+-rwxr-xr-x   0        0        0      947 2023-11-16 16:14:11.027629 jvi-0.1.4/jvi/bin/jvi-imp.py
+-rwxr-xr-x   0        0        0     3337 2023-11-16 16:14:11.027629 jvi-0.1.4/jvi/bin/jvi-infrared.py
+-rwxr-xr-x   0        0        0     1415 2023-11-16 16:14:11.027629 jvi-0.1.4/jvi/bin/jvi-letterbox.py
+-rwxr-xr-x   0        0        0     1917 2023-11-16 16:14:11.027629 jvi-0.1.4/jvi/bin/jvi-resize.py
+-rwxr-xr-x   0        0        0     2412 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-superres.py
+-rwxr-xr-x   0        0        0     1127 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/bin/jvi-tile-dir.py
+-rwxr-xr-x   0        0        0     2006 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/bin/jvi-tile-match.py
+-rwxr-xr-x   0        0        0     1938 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/bin/jvi-tile-viewer.py
+-rwxr-xr-x   0        0        0     1891 2023-11-16 05:52:20.928471 jvi-0.1.4/jvi/bin/jvi-tks.py
+-rwxr-xr-x   0        0        0     2600 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/bin/jvi-video2img.py
+-rw-r--r--   0        0        0      104 2023-11-16 05:52:20.912471 jvi-0.1.4/jvi/common.py
+-rw-r--r--   0        0        0        0 2023-11-16 05:52:20.916471 jvi-0.1.4/jvi/drawing/__init__.py
+-rw-r--r--   0        0        0    10301 2023-11-16 05:52:20.916471 jvi-0.1.4/jvi/drawing/color.py
+-rw-r--r--   0        0        0     3497 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/drawing/shape.py
+-rw-r--r--   0        0        0      372 2024-03-15 09:19:35.357036 jvi-0.1.4/jvi/geo/__init__.py
+-rw-r--r--   0        0        0     1298 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/convert.py
+-rw-r--r--   0        0        0     1541 2023-11-16 05:52:20.904471 jvi-0.1.4/jvi/geo/gp.py
+-rw-r--r--   0        0        0     1323 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/line_segment.py
+-rw-r--r--   0        0        0     5530 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/point2d.py
+-rw-r--r--   0        0        0     3749 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/polygon.py
+-rw-r--r--   0        0        0      230 2023-11-16 05:52:20.904471 jvi-0.1.4/jvi/geo/protocol.py
+-rw-r--r--   0        0        0    11784 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/rectangle.py
+-rw-r--r--   0        0        0     6384 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/size2d.py
+-rw-r--r--   0        0        0     5944 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/size2d_gp.bak
+-rw-r--r--   0        0        0     1230 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/geo/trans.py
+-rw-r--r--   0        0        0        0 2023-11-16 05:52:20.936472 jvi-0.1.4/jvi/gui/__init__.py
+-rw-r--r--   0        0        0     2668 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/gui/image_viewer.py
+-rw-r--r--   0        0        0     5293 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/gui/image_win.py
+-rw-r--r--   0        0        0     1475 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/gui/imp_win.py
+-rw-r--r--   0        0        0     3003 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/gui/record_viewer.py
+-rw-r--r--   0        0        0     2155 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/gui/video_viewer.py
+-rw-r--r--   0        0        0        0 2023-11-16 05:52:20.920471 jvi-0.1.4/jvi/image/__init__.py
+-rw-r--r--   0        0        0     3226 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/image.py
+-rw-r--r--   0        0        0     1200 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/image_factory.py
+-rw-r--r--   0        0        0     5632 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/image_nda.py
+-rw-r--r--   0        0        0     3123 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/infrared.py
+-rw-r--r--   0        0        0     3772 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/io.py
+-rw-r--r--   0        0        0     7552 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/proc.py
+-rw-r--r--   0        0        0     3827 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/sc3c.py
+-rw-r--r--   0        0        0     1913 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/stat.py
+-rw-r--r--   0        0        0     4893 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/struct.py
+-rw-r--r--   0        0        0     3750 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/tile.py
+-rw-r--r--   0        0        0     1869 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/tile_set.py
+-rw-r--r--   0        0        0     1263 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/trace.py
+-rw-r--r--   0        0        0      616 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/trans.py
+-rw-r--r--   0        0        0     2216 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/image/util.py
+-rw-r--r--   0        0        0        0 2023-11-16 05:52:20.932471 jvi-0.1.4/jvi/match/__init__.py
+-rw-r--r--   0        0        0     4956 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/match/match.py
+-rw-r--r--   0        0        0     2578 2023-11-16 16:08:10.173256 jvi-0.1.4/jvi/match/match_template.py
+-rw-r--r--   0        0        0        0 2023-11-17 03:53:27.240712 jvi-0.1.4/jvi/py.typed
+-rw-r--r--   0        0        0      491 2024-05-26 02:19:48.396876 jvi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 jvi-0.1.4/PKG-INFO
```

### Comparing `jvi-0.1.3/jvi/bin/jvi-blur-x.py` & `jvi-0.1.4/jvi/bin/jvi-blur-x.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-blur.py` & `jvi-0.1.4/jvi/bin/jvi-blur.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-box.py` & `jvi-0.1.4/jvi/bin/jvi-box.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-cut.py` & `jvi-0.1.4/jvi/bin/jvi-cut.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-ff-remux.py` & `jvi-0.1.4/jvi/bin/jvi-ff-remux.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-ff-split.py` & `jvi-0.1.4/jvi/bin/jvi-ff-split.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-img2video.py` & `jvi-0.1.4/jvi/bin/jvi-img2video.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-imp.py` & `jvi-0.1.4/jvi/bin/jvi-imp.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-infrared.py` & `jvi-0.1.4/jvi/bin/jvi-infrared.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-letterbox.py` & `jvi-0.1.4/jvi/bin/jvi-letterbox.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-resize.py` & `jvi-0.1.4/jvi/bin/jvi-resize.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-superres.py` & `jvi-0.1.4/jvi/bin/jvi-superres.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-tile-dir.py` & `jvi-0.1.4/jvi/bin/jvi-tile-dir.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-tile-match.py` & `jvi-0.1.4/jvi/bin/jvi-tile-match.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-tile-viewer.py` & `jvi-0.1.4/jvi/bin/jvi-tile-viewer.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-tks.py` & `jvi-0.1.4/jvi/bin/jvi-tks.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/bin/jvi-video2img.py` & `jvi-0.1.4/jvi/bin/jvi-video2img.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/drawing/color.py` & `jvi-0.1.4/jvi/drawing/color.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/drawing/shape.py` & `jvi-0.1.4/jvi/drawing/shape.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/convert.py` & `jvi-0.1.4/jvi/geo/convert.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/gp.py` & `jvi-0.1.4/jvi/geo/gp.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/line_segment.py` & `jvi-0.1.4/jvi/geo/line_segment.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/point2d.py` & `jvi-0.1.4/jvi/geo/point2d.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/polygon.py` & `jvi-0.1.4/jvi/geo/polygon.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/rectangle.py` & `jvi-0.1.4/jvi/geo/rectangle.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/size2d.py` & `jvi-0.1.4/jvi/geo/size2d.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/size2d_gp.bak` & `jvi-0.1.4/jvi/geo/size2d_gp.bak`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/geo/trans.py` & `jvi-0.1.4/jvi/geo/trans.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/gui/image_viewer.py` & `jvi-0.1.4/jvi/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/gui/image_win.py` & `jvi-0.1.4/jvi/gui/image_win.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/gui/imp_win.py` & `jvi-0.1.4/jvi/gui/imp_win.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/gui/record_viewer.py` & `jvi-0.1.4/jvi/gui/record_viewer.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/gui/video_viewer.py` & `jvi-0.1.4/jvi/gui/video_viewer.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/image.py` & `jvi-0.1.4/jvi/image/image.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/image_factory.py` & `jvi-0.1.4/jvi/image/image_factory.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/image_nda.py` & `jvi-0.1.4/jvi/image/image_nda.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/infrared.py` & `jvi-0.1.4/jvi/image/infrared.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/io.py` & `jvi-0.1.4/jvi/image/io.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/proc.py` & `jvi-0.1.4/jvi/image/proc.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/sc3c.py` & `jvi-0.1.4/jvi/image/sc3c.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/stat.py` & `jvi-0.1.4/jvi/image/stat.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/struct.py` & `jvi-0.1.4/jvi/image/struct.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/tile.py` & `jvi-0.1.4/jvi/image/tile.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/tile_set.py` & `jvi-0.1.4/jvi/image/tile_set.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/trace.py` & `jvi-0.1.4/jvi/image/trace.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/trans.py` & `jvi-0.1.4/jvi/image/trans.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/image/util.py` & `jvi-0.1.4/jvi/image/util.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/match/match.py` & `jvi-0.1.4/jvi/match/match.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/jvi/match/match_template.py` & `jvi-0.1.4/jvi/match/match_template.py`

 * *Files identical despite different names*

### Comparing `jvi-0.1.3/PKG-INFO` & `jvi-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jvi
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: dayn9t
 Author-email: dayn9t@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

