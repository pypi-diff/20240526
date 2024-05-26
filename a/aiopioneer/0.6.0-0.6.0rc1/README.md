# Comparing `tmp/aiopioneer-0.6.0.tar.gz` & `tmp/aiopioneer-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.6.0.tar", last modified: Sun May 26 10:54:58 2024, max compression
+gzip compressed data, was "aiopioneer-0.6.0rc1.tar", last modified: Sun Apr 21 10:58:26 2024, max compression
```

## Comparing `aiopioneer-0.6.0.tar` & `aiopioneer-0.6.0rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2024-05-26 10:54:58.074140 aiopioneer-0.6.0/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0/LICENSE
--rw-rw----   0 root         (0) adm          (4)    29880 2024-05-26 10:54:58.078715 aiopioneer-0.6.0/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    29230 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2024-05-26 10:54:57.854143 aiopioneer-0.6.0/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)    11211 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    13805 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    15128 2024-05-26 10:51:00.000000 aiopioneer-0.6.0/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    18687 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-05-26 10:54:58.044140 aiopioneer-0.6.0/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)     8175 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3419 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)    19209 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    25466 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)      599 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23416 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15910 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     6987 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8405 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    86948 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5266 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2024-05-26 10:54:58.064140 aiopioneer-0.6.0/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    29880 2024-05-26 10:54:57.000000 aiopioneer-0.6.0/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      614 2024-05-26 10:54:57.000000 aiopioneer-0.6.0/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2024-05-26 10:54:57.000000 aiopioneer-0.6.0/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2024-05-26 10:54:57.000000 aiopioneer-0.6.0/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2024-05-26 10:54:57.000000 aiopioneer-0.6.0/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2024-05-26 10:54:58.086874 aiopioneer-0.6.0/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1101 2024-05-23 06:28:23.000000 aiopioneer-0.6.0/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.599502 aiopioneer-0.6.0rc1/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.6.0rc1/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    29883 2024-04-21 10:58:26.603877 aiopioneer-0.6.0rc1/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    29230 2024-04-20 12:22:03.000000 aiopioneer-0.6.0rc1/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.409504 aiopioneer-0.6.0rc1/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2024-03-27 20:16:44.000000 aiopioneer-0.6.0rc1/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    11211 2024-04-20 12:17:48.000000 aiopioneer-0.6.0rc1/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    13805 2024-04-01 19:37:10.000000 aiopioneer-0.6.0rc1/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    15131 2024-04-20 09:58:15.000000 aiopioneer-0.6.0rc1/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    18687 2024-03-27 20:47:07.000000 aiopioneer-0.6.0rc1/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.569502 aiopioneer-0.6.0rc1/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)     8175 2024-04-03 07:47:01.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3419 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)    19209 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    25466 2024-03-31 11:50:52.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)      599 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23416 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    15910 2024-04-03 07:56:23.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     6987 2024-04-03 07:20:56.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8405 2024-03-13 09:14:44.000000 aiopioneer-0.6.0rc1/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    86948 2024-04-20 12:17:45.000000 aiopioneer-0.6.0rc1/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5266 2024-04-05 20:12:40.000000 aiopioneer-0.6.0rc1/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2024-04-21 10:58:26.579502 aiopioneer-0.6.0rc1/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    29883 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      614 2024-04-21 10:58:26.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2024-04-21 10:58:25.000000 aiopioneer-0.6.0rc1/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2024-04-21 10:58:26.610801 aiopioneer-0.6.0rc1/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1101 2024-03-31 08:50:09.000000 aiopioneer-0.6.0rc1/setup.py
```

### Comparing `aiopioneer-0.6.0/LICENSE` & `aiopioneer-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/PKG-INFO` & `aiopioneer-0.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0/README.md` & `aiopioneer-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/cli.py` & `aiopioneer-0.6.0rc1/aiopioneer/cli.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/commands.py` & `aiopioneer-0.6.0rc1/aiopioneer/commands.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/const.py` & `aiopioneer-0.6.0rc1/aiopioneer/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for aiopioneer."""
 
 from enum import StrEnum
 
-VERSION = "0.6.0"
+VERSION = "0.6.0rc1"
 DEFAULT_TIMEOUT = 2
 DEFAULT_SCAN_INTERVAL = 60
 DEFAULT_PORT = 8102
 
 
 class Zones(StrEnum):
     """Valid aiopioneer zones."""
```

### Comparing `aiopioneer-0.6.0/aiopioneer/param.py` & `aiopioneer-0.6.0rc1/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/__init__.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/audio.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/dsp.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/information.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/response.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/settings.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/system.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/system.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/tuner.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/tuner.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/parsers/video.py` & `aiopioneer-0.6.0rc1/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/pioneer_avr.py` & `aiopioneer-0.6.0rc1/aiopioneer/pioneer_avr.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer/util.py` & `aiopioneer-0.6.0rc1/aiopioneer/util.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.6.0rc1/aiopioneer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.6.0
+Version: 0.6.0rc1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopioneer-0.6.0/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.6.0rc1/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.6.0/setup.py` & `aiopioneer-0.6.0rc1/setup.py`

 * *Files identical despite different names*

