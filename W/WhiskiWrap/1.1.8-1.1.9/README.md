# Comparing `tmp/WhiskiWrap-1.1.8.tar.gz` & `tmp/WhiskiWrap-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WhiskiWrap-1.1.8.tar", last modified: Tue Feb 27 05:12:41 2024, max compression
+gzip compressed data, was "WhiskiWrap-1.1.9.tar", last modified: Wed Feb 28 20:33:29 2024, max compression
```

## Comparing `WhiskiWrap-1.1.8.tar` & `WhiskiWrap-1.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 05:12:41.081879 WhiskiWrap-1.1.8/
--rw-rw-rw-   0        0        0     1643 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      112 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8617 2024-02-27 05:12:41.080882 WhiskiWrap-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8280 2023-05-04 04:27:18.000000 WhiskiWrap-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 05:12:41.052788 WhiskiWrap-1.1.8/WhiskiWrap/
--rw-rw-rw-   0        0        0     1419 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.8/WhiskiWrap/__init__.py
--rw-rw-rw-   0        0        0    84180 2024-02-27 00:07:54.000000 WhiskiWrap-1.1.8/WhiskiWrap/base.py
--rw-rw-rw-   0        0        0     3487 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.8/WhiskiWrap/default.parameters
--rw-rw-rw-   0        0        0 34781772 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/WhiskiWrap/halfspace.detectorbank
--rw-rw-rw-   0        0        0 34781772 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/WhiskiWrap/line.detectorbank
--rw-rw-rw-   0        0        0    13829 2024-02-27 05:11:33.000000 WhiskiWrap-1.1.8/WhiskiWrap/load_whisker_data.py
--rw-rw-rw-   0        0        0    32697 2023-08-09 14:40:06.000000 WhiskiWrap-1.1.8/WhiskiWrap/mfile_io.py
--rw-rw-rw-   0        0        0     3487 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/WhiskiWrap/sensitive.parameters
--rw-rw-rw-   0        0        0     9264 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/WhiskiWrap/tests.py
--rw-rw-rw-   0        0        0     5025 2024-02-27 03:42:45.000000 WhiskiWrap-1.1.8/WhiskiWrap/utils.py
--rw-rw-rw-   0        0        0     7903 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/WhiskiWrap/video_utils.py
--rw-rw-rw-   0        0        0    16968 2024-02-27 03:42:54.000000 WhiskiWrap-1.1.8/WhiskiWrap/wfile_io.py
-drwxrwxrwx   0        0        0        0 2024-02-27 05:12:41.065781 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/
--rw-rw-rw-   0        0        0     8617 2024-02-27 05:12:40.000000 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-02-27 05:12:40.000000 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 05:12:40.000000 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-02-27 05:12:40.000000 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-02-27 05:12:40.000000 WhiskiWrap-1.1.8/WhiskiWrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-27 05:12:41.081879 WhiskiWrap-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-02-27 05:12:22.000000 WhiskiWrap-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-27 05:12:41.079882 WhiskiWrap-1.1.8/wwutils/
--rw-rw-rw-   0        0        0      315 2024-02-20 17:05:21.000000 WhiskiWrap-1.1.8/wwutils/__init__.py
--rw-rw-rw-   0        0        0    15270 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/wwutils/bootstrap.py
--rw-rw-rw-   0        0        0     8214 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/wwutils/dataload.py
--rw-rw-rw-   0        0        0    59075 2023-05-24 15:29:46.000000 WhiskiWrap-1.1.8/wwutils/misc.py
--rw-rw-rw-   0        0        0    56510 2023-05-24 15:29:46.000000 WhiskiWrap-1.1.8/wwutils/plot.py
--rw-rw-rw-   0        0        0     9449 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.8/wwutils/stats.py
--rw-rw-rw-   0        0        0     1728 2023-08-15 23:05:22.000000 WhiskiWrap-1.1.8/wwutils/test_load_ffmpeg_lib.py
--rw-rw-rw-   0        0        0    29168 2023-05-30 19:50:19.000000 WhiskiWrap-1.1.8/wwutils/video.py
--rw-rw-rw-   0        0        0     1627 2024-02-20 22:06:08.000000 WhiskiWrap-1.1.8/wwutils/whisk_permissions.py
+drwxrwxrwx   0        0        0        0 2024-02-28 20:33:29.190941 WhiskiWrap-1.1.9/
+-rw-rw-rw-   0        0        0     1643 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      112 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8617 2024-02-28 20:33:29.190437 WhiskiWrap-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8280 2023-05-04 04:27:18.000000 WhiskiWrap-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-28 20:33:29.096682 WhiskiWrap-1.1.9/WhiskiWrap/
+-rw-rw-rw-   0        0        0     1419 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.9/WhiskiWrap/__init__.py
+-rw-rw-rw-   0        0        0    86714 2024-02-28 20:31:18.000000 WhiskiWrap-1.1.9/WhiskiWrap/base.py
+-rw-rw-rw-   0        0        0     3487 2023-04-12 17:48:04.000000 WhiskiWrap-1.1.9/WhiskiWrap/default.parameters
+-rw-rw-rw-   0        0        0 34781772 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/WhiskiWrap/halfspace.detectorbank
+-rw-rw-rw-   0        0        0 34781772 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/WhiskiWrap/line.detectorbank
+-rw-rw-rw-   0        0        0    13829 2024-02-27 05:11:33.000000 WhiskiWrap-1.1.9/WhiskiWrap/load_whisker_data.py
+-rw-rw-rw-   0        0        0    32697 2023-08-09 14:40:06.000000 WhiskiWrap-1.1.9/WhiskiWrap/mfile_io.py
+-rw-rw-rw-   0        0        0     3487 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/WhiskiWrap/sensitive.parameters
+-rw-rw-rw-   0        0        0     9264 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/WhiskiWrap/tests.py
+-rw-rw-rw-   0        0        0     5025 2024-02-27 03:42:45.000000 WhiskiWrap-1.1.9/WhiskiWrap/utils.py
+-rw-rw-rw-   0        0        0     7903 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/WhiskiWrap/video_utils.py
+-rw-rw-rw-   0        0        0    16968 2024-02-27 03:42:54.000000 WhiskiWrap-1.1.9/WhiskiWrap/wfile_io.py
+drwxrwxrwx   0        0        0        0 2024-02-28 20:33:29.115682 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/
+-rw-rw-rw-   0        0        0     8617 2024-02-28 20:33:28.000000 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-02-28 20:33:28.000000 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-28 20:33:28.000000 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-02-28 20:33:28.000000 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-02-28 20:33:28.000000 WhiskiWrap-1.1.9/WhiskiWrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-28 20:33:29.190950 WhiskiWrap-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-02-28 20:32:35.000000 WhiskiWrap-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-28 20:33:29.189380 WhiskiWrap-1.1.9/wwutils/
+-rw-rw-rw-   0        0        0      315 2024-02-20 17:05:21.000000 WhiskiWrap-1.1.9/wwutils/__init__.py
+-rw-rw-rw-   0        0        0    15270 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/wwutils/bootstrap.py
+-rw-rw-rw-   0        0        0     8214 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/wwutils/dataload.py
+-rw-rw-rw-   0        0        0    59075 2023-05-24 15:29:46.000000 WhiskiWrap-1.1.9/wwutils/misc.py
+-rw-rw-rw-   0        0        0    56510 2023-05-24 15:29:46.000000 WhiskiWrap-1.1.9/wwutils/plot.py
+-rw-rw-rw-   0        0        0     9449 2023-04-12 17:48:05.000000 WhiskiWrap-1.1.9/wwutils/stats.py
+-rw-rw-rw-   0        0        0     1728 2023-08-15 23:05:22.000000 WhiskiWrap-1.1.9/wwutils/test_load_ffmpeg_lib.py
+-rw-rw-rw-   0        0        0    29168 2023-05-30 19:50:19.000000 WhiskiWrap-1.1.9/wwutils/video.py
+-rw-rw-rw-   0        0        0     1627 2024-02-20 22:06:08.000000 WhiskiWrap-1.1.9/wwutils/whisk_permissions.py
```

### Comparing `WhiskiWrap-1.1.8/LICENSE.txt` & `WhiskiWrap-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/PKG-INFO` & `WhiskiWrap-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhiskiWrap
-Version: 1.1.8
+Version: 1.1.9
 Summary: Whisk package wrapper created by cxrodgers
 Home-page: http://pypi.python.org/pypi/WhiskiWrap/
 Author: Chris Rodgers
 Author-email: 
 Maintainer: cxrodgers, aiporre, vncntprvst
 License: LICENSE.txt
 Description-Content-Type: text/markdown
```

### Comparing `WhiskiWrap-1.1.8/README.md` & `WhiskiWrap-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/__init__.py` & `WhiskiWrap-1.1.9/WhiskiWrap/__init__.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/default.parameters` & `WhiskiWrap-1.1.9/WhiskiWrap/default.parameters`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/halfspace.detectorbank` & `WhiskiWrap-1.1.9/WhiskiWrap/halfspace.detectorbank`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/line.detectorbank` & `WhiskiWrap-1.1.9/WhiskiWrap/line.detectorbank`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/load_whisker_data.py` & `WhiskiWrap-1.1.9/WhiskiWrap/load_whisker_data.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/mfile_io.py` & `WhiskiWrap-1.1.9/WhiskiWrap/mfile_io.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/sensitive.parameters` & `WhiskiWrap-1.1.9/WhiskiWrap/sensitive.parameters`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/tests.py` & `WhiskiWrap-1.1.9/WhiskiWrap/tests.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/utils.py` & `WhiskiWrap-1.1.9/WhiskiWrap/utils.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/video_utils.py` & `WhiskiWrap-1.1.9/WhiskiWrap/video_utils.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap/wfile_io.py` & `WhiskiWrap-1.1.9/WhiskiWrap/wfile_io.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap.egg-info/PKG-INFO` & `WhiskiWrap-1.1.9/WhiskiWrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhiskiWrap
-Version: 1.1.8
+Version: 1.1.9
 Summary: Whisk package wrapper created by cxrodgers
 Home-page: http://pypi.python.org/pypi/WhiskiWrap/
 Author: Chris Rodgers
 Author-email: 
 Maintainer: cxrodgers, aiporre, vncntprvst
 License: LICENSE.txt
 Description-Content-Type: text/markdown
```

### Comparing `WhiskiWrap-1.1.8/WhiskiWrap.egg-info/SOURCES.txt` & `WhiskiWrap-1.1.9/WhiskiWrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/setup.py` & `WhiskiWrap-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup
 
 setup(
    name='WhiskiWrap',
-   version='1.1.8',
+   version='1.1.9',
    author='Chris Rodgers',
    author_email='',
    maintainer=', '.join(['cxrodgers','aiporre','vncntprvst']),
    packages=['WhiskiWrap','wwutils'],
    # scripts=['bin/script1','bin/script2'],
    url='http://pypi.python.org/pypi/WhiskiWrap/',
    license='LICENSE.txt',
```

### Comparing `WhiskiWrap-1.1.8/wwutils/bootstrap.py` & `WhiskiWrap-1.1.9/wwutils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/dataload.py` & `WhiskiWrap-1.1.9/wwutils/dataload.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/misc.py` & `WhiskiWrap-1.1.9/wwutils/misc.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/plot.py` & `WhiskiWrap-1.1.9/wwutils/plot.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/stats.py` & `WhiskiWrap-1.1.9/wwutils/stats.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/test_load_ffmpeg_lib.py` & `WhiskiWrap-1.1.9/wwutils/test_load_ffmpeg_lib.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/video.py` & `WhiskiWrap-1.1.9/wwutils/video.py`

 * *Files identical despite different names*

### Comparing `WhiskiWrap-1.1.8/wwutils/whisk_permissions.py` & `WhiskiWrap-1.1.9/wwutils/whisk_permissions.py`

 * *Files identical despite different names*

