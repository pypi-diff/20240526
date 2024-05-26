# Comparing `tmp/beets-autofix-0.1.3.tar.gz` & `tmp/beets_autofix-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-autofix-0.1.3.tar", last modified: Fri Mar  4 21:48:18 2022, max compression
+gzip compressed data, was "beets_autofix-0.1.5.tar", last modified: Sun May 26 14:17:18 2024, max compression
```

## Comparing `beets-autofix-0.1.3.tar` & `beets_autofix-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1067 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      132 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beets_autofix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beetsplug/autofix/
--rwxr-xr-x   0 runner    (1001) docker     (121)      760 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      736 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/about.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7610 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/command.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1008 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      256 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/config_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/beetsplug/autofix/task/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1468 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4789 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/ab_data_fetcher.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2328 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/audio_conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2396 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/genre_finder.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      759 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/missing_file_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1720 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/tag_cleaner.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1618 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/xtractor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1641 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/beetsplug/autofix/task/year_fixer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      214 2022-03-04 21:48:18.000000 beets-autofix-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1654 2022-03-04 21:48:09.000000 beets-autofix-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:17:18.270405 beets_autofix-0.1.5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-26 14:17:18.270405 beets_autofix-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:17:18.270405 beets_autofix-0.1.5/beets_autofix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-26 14:17:18.000000 beets_autofix-0.1.5/beets_autofix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-26 14:17:18.000000 beets_autofix-0.1.5/beets_autofix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:17:18.000000 beets_autofix-0.1.5/beets_autofix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-26 14:17:18.000000 beets_autofix-0.1.5/beets_autofix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 14:17:18.000000 beets_autofix-0.1.5/beets_autofix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:17:18.266405 beets_autofix-0.1.5/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:17:18.266405 beets_autofix-0.1.5/beetsplug/autofix/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      760 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/about.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7610 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1008 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      256 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/config_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:17:18.270405 beets_autofix-0.1.5/beetsplug/autofix/task/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1468 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/ab_data_fetcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2328 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/audio_conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2396 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/genre_finder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      759 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/missing_file_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/tag_cleaner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1618 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/xtractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1641 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/beetsplug/autofix/task/year_fixer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      214 2024-05-26 14:17:18.270405 beets_autofix-0.1.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-26 14:17:06.000000 beets_autofix-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beets-autofix-0.1.3/LICENSE.txt` & `beets_autofix-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/PKG-INFO` & `beets_autofix-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,154 @@
 Metadata-Version: 2.1
 Name: beets-autofix
-Version: 0.1.3
+Version: 0.1.5
 Summary: ('A beets plugin to execute repetitive tasks in one go.',)
 Home-page: https://github.com/adamjakab/BeetsPluginAutofix
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
-Description: [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginAutofix/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginAutofix?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        # Autofix (Beets Plugin)
-        
-        The *beets-autofix* plugin helps you to automate the tasks that you keep repeating to maintain your library. 
-        
-        The plugin is a wrapper around the plugins that you already have in beets. It iterates through the items you have in your library and calls the individual plugins to execute their jobs as they are configured by you.
-        
-        
-        ## Installation
-        The plugin can be installed via:
-        
-        ```shell script
-        $ pip install beets-autofix
-        ```
-        
-        
-        ## Usage
-        
-        Invoke the plugin as:
-        
-            $ beet autofix [options] [QUERY...]
-        
-        
-        The following command line options are available:
-        
-        **--max_exec_time=MAX_EXEC_TIME [-m MAX_EXEC_TIME]**: Interrupt the execution after this number of seconds.
-        
-        **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
-        
-        
-        ## Configuration
-        By default all tasks are disabled:
-        
-        ```yaml
-        max_exec_time: 0
-        tasks:
-          missing_file_checker:
-            enabled: no
-          year_fixer:
-            enabled: no
-          audio_conversion:
-            enabled: no
-          tag_cleaner:
-            enabled: no
-          ab_data_fetcher:
-            enabled: no
-          xtractor:
-            enabled: no
-          genre_finder:
-            enabled: no
-        ```
-        
-        You need to override the default configuration and enable the tasks you want to run.
-        
-        The `max_exec_time` allows you to interrupt the execution after a certain number of seconds. For no limit set it to 0.
-        
-        
-        ## Tasks
-        The following tasks are available:
-        
-        ### Missing File Checker (task name: missing_file_checker) [related plugin: None]
-        This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
-        
-        
-        ### Year Fixer (task name: year_fixer) [related plugin: [yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)]
-        The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
-        
-        
-        ### Conversion (task name: audio_conversion) [related plugin: [convert](https://beets.readthedocs.io/en/stable/plugins/convert.html)]
-        This plugin is based on the `convert` plugin and triggers the conversion in two cases:
-        
-        - if the format of the item is does not correspond to the `format` specified in the `convert` plugin configuration
-        - if the bitrate of the item is greater than the `bitrate` specified in the `convert` plugin configuration
-        
-        In both cases the audio file will be converted according to the `convert` plugin configuration. The converted audio file will be attached to the library item whilst the original audio file will be deleted.
-        
-        ### Tag Cleaner (task name: tag_cleaner) [related plugin: [zero](https://beets.readthedocs.io/en/stable/plugins/zero.html)]
-        This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing. 
-        
-        
-        ### AcousticBrainz Data Fetcher (task name: ab_data_fetcher) [related plugin: [acousticbrainz](https://beets.readthedocs.io/en/stable/plugins/acousticbrainz.html)]
-        This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set. 
-        
-        The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
-        
-        
-        ### Xtractor(task name: xtractor) [related plugin: [xtractor](https://github.com/adamjakab/BeetsPluginXtractor)]
-        This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files. 
-        
-        
-        ### Genre Finder (task name: genre_finder) [related plugin: [lastgenre](https://beets.readthedocs.io/en/stable/plugins/lastgenre.html)]
-        This task will call the `lastgenre` plugin to find out the genre of a specific song. If that fails, it will fall back to the `genre_rosamerica` attribute estimated by the Essentia high level extractor and map the genre based on this table:
-        
-        ```text
-            "cla" -> "classical"
-            "dan" -> "dance"
-            "hip" -> "hip-hop"
-            "jaz" -> "jazz"
-            "pop" -> "pop"
-            "rhy" -> "rhythm and blues"
-            "roc" -> "rock"
-            "spe" -> "speech"
-        ```
-        
-        ## Issues
-        - If something is not working as expected please use the Issue tracker.
-        - If the documentation is not clear please use the Issue tracker.
-        - If you have a feature request please use the Issue tracker.
-        - In any other situation please use the Issue tracker.
-        
-        
-        ## Other plugins by the same author
-        
-        - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
-        - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
-        - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
-        - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
-        - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
-        - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
-        - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
-        
-        
-        ## Final Remarks
-        Enjoy!
-        
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: beets>=1.4.9
+Requires-Dist: alive-progress
 Provides-Extra: tests
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginAutofix/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginAutofix?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# Autofix (Beets Plugin)
+
+The _beets-autofix_ plugin helps you to automate the tasks that you keep repeating to maintain your library.
+
+The plugin is a wrapper around the plugins that you already have in beets. It iterates through the items you have in your library and calls the individual plugins to execute their jobs as they are configured by you.
+
+## Installation
+
+The plugin can be installed via:
+
+```shell script
+$ pip install beets-autofix
+```
+
+## Usage
+
+Invoke the plugin as:
+
+    $ beet autofix [options] [QUERY...]
+
+The following command line options are available:
+
+**--max_exec_time=MAX_EXEC_TIME [-m MAX_EXEC_TIME]**: Interrupt the execution after this number of seconds.
+
+**--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
+
+## Configuration
+
+By default all tasks are disabled:
+
+```yaml
+max_exec_time: 0
+tasks:
+  missing_file_checker:
+    enabled: no
+  year_fixer:
+    enabled: no
+  audio_conversion:
+    enabled: no
+  tag_cleaner:
+    enabled: no
+  ab_data_fetcher:
+    enabled: no
+  xtractor:
+    enabled: no
+  genre_finder:
+    enabled: no
+```
+
+You need to override the default configuration and enable the tasks you want to run.
+
+The `max_exec_time` allows you to interrupt the execution after a certain number of seconds. For no limit set it to 0.
+
+## Tasks
+
+The following tasks are available:
+
+### Missing File Checker (task name: missing_file_checker) [related plugin: None]
+
+This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
+
+### Year Fixer (task name: year_fixer) [related plugin: [yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)]
+
+The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
+
+### Conversion (task name: audio_conversion) [related plugin: [convert](https://beets.readthedocs.io/en/stable/plugins/convert.html)]
+
+This plugin is based on the `convert` plugin and triggers the conversion in two cases:
+
+- if the format of the item is does not correspond to the `format` specified in the `convert` plugin configuration
+- if the bitrate of the item is greater than the `bitrate` specified in the `convert` plugin configuration
+
+In both cases the audio file will be converted according to the `convert` plugin configuration. The converted audio file will be attached to the library item whilst the original audio file will be deleted.
+
+### Tag Cleaner (task name: tag_cleaner) [related plugin: [zero](https://beets.readthedocs.io/en/stable/plugins/zero.html)]
+
+This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing.
+
+### AcousticBrainz Data Fetcher (task name: ab_data_fetcher) [related plugin: [acousticbrainz](https://beets.readthedocs.io/en/stable/plugins/acousticbrainz.html)]
+
+This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set.
+
+The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
+
+### Xtractor(task name: xtractor) [related plugin: [xtractor](https://github.com/adamjakab/BeetsPluginXtractor)]
+
+This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files.
+
+### Genre Finder (task name: genre_finder) [related plugin: [lastgenre](https://beets.readthedocs.io/en/stable/plugins/lastgenre.html)]
+
+This task will call the `lastgenre` plugin to find out the genre of a specific song. If that fails, it will fall back to the `genre_rosamerica` attribute estimated by the Essentia high level extractor and map the genre based on this table:
+
+```text
+    "cla" -> "classical"
+    "dan" -> "dance"
+    "hip" -> "hip-hop"
+    "jaz" -> "jazz"
+    "pop" -> "pop"
+    "rhy" -> "rhythm and blues"
+    "roc" -> "rock"
+    "spe" -> "speech"
+```
+
+## Issues
+
+- If something is not working as expected please use the Issue tracker.
+- If the documentation is not clear please use the Issue tracker.
+- If you have a feature request please use the Issue tracker.
+- In any other situation please use the Issue tracker.
+
+## Other plugins by the same author
+
+- [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
+- [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
+- [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
+- [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
+- [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
+- [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
+- [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
+
+## Final Remarks
+
+Enjoy!
```

### Comparing `beets-autofix-0.1.3/README.md` & `beets_autofix-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,41 @@
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginAutofix/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginAutofix?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # Autofix (Beets Plugin)
 
-The *beets-autofix* plugin helps you to automate the tasks that you keep repeating to maintain your library. 
+The _beets-autofix_ plugin helps you to automate the tasks that you keep repeating to maintain your library.
 
 The plugin is a wrapper around the plugins that you already have in beets. It iterates through the items you have in your library and calls the individual plugins to execute their jobs as they are configured by you.
 
-
 ## Installation
+
 The plugin can be installed via:
 
 ```shell script
 $ pip install beets-autofix
 ```
 
-
 ## Usage
 
 Invoke the plugin as:
 
     $ beet autofix [options] [QUERY...]
 
-
 The following command line options are available:
 
 **--max_exec_time=MAX_EXEC_TIME [-m MAX_EXEC_TIME]**: Interrupt the execution after this number of seconds.
 
 **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
 
-
 ## Configuration
+
 By default all tasks are disabled:
 
 ```yaml
 max_exec_time: 0
 tasks:
   missing_file_checker:
     enabled: no
@@ -54,75 +53,77 @@
     enabled: no
 ```
 
 You need to override the default configuration and enable the tasks you want to run.
 
 The `max_exec_time` allows you to interrupt the execution after a certain number of seconds. For no limit set it to 0.
 
-
 ## Tasks
+
 The following tasks are available:
 
 ### Missing File Checker (task name: missing_file_checker) [related plugin: None]
-This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
 
+This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
 
 ### Year Fixer (task name: year_fixer) [related plugin: [yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)]
-The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
 
+The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
 
 ### Conversion (task name: audio_conversion) [related plugin: [convert](https://beets.readthedocs.io/en/stable/plugins/convert.html)]
+
 This plugin is based on the `convert` plugin and triggers the conversion in two cases:
 
 - if the format of the item is does not correspond to the `format` specified in the `convert` plugin configuration
 - if the bitrate of the item is greater than the `bitrate` specified in the `convert` plugin configuration
 
 In both cases the audio file will be converted according to the `convert` plugin configuration. The converted audio file will be attached to the library item whilst the original audio file will be deleted.
 
 ### Tag Cleaner (task name: tag_cleaner) [related plugin: [zero](https://beets.readthedocs.io/en/stable/plugins/zero.html)]
-This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing. 
 
+This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing.
 
 ### AcousticBrainz Data Fetcher (task name: ab_data_fetcher) [related plugin: [acousticbrainz](https://beets.readthedocs.io/en/stable/plugins/acousticbrainz.html)]
-This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set. 
 
-The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
+This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set.
 
+The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
 
 ### Xtractor(task name: xtractor) [related plugin: [xtractor](https://github.com/adamjakab/BeetsPluginXtractor)]
-This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files. 
 
+This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files.
 
 ### Genre Finder (task name: genre_finder) [related plugin: [lastgenre](https://beets.readthedocs.io/en/stable/plugins/lastgenre.html)]
+
 This task will call the `lastgenre` plugin to find out the genre of a specific song. If that fails, it will fall back to the `genre_rosamerica` attribute estimated by the Essentia high level extractor and map the genre based on this table:
 
 ```text
     "cla" -> "classical"
     "dan" -> "dance"
     "hip" -> "hip-hop"
     "jaz" -> "jazz"
     "pop" -> "pop"
     "rhy" -> "rhythm and blues"
     "roc" -> "rock"
     "spe" -> "speech"
 ```
 
 ## Issues
+
 - If something is not working as expected please use the Issue tracker.
 - If the documentation is not clear please use the Issue tracker.
 - If you have a feature request please use the Issue tracker.
 - In any other situation please use the Issue tracker.
 
-
 ## Other plugins by the same author
 
 - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
 - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
 - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
 - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
 - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
 - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
 - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
 
-
 ## Final Remarks
+
 Enjoy!
```

### Comparing `beets-autofix-0.1.3/beets_autofix.egg-info/PKG-INFO` & `beets_autofix-0.1.5/beets_autofix.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,154 @@
 Metadata-Version: 2.1
 Name: beets-autofix
-Version: 0.1.3
+Version: 0.1.5
 Summary: ('A beets plugin to execute repetitive tasks in one go.',)
 Home-page: https://github.com/adamjakab/BeetsPluginAutofix
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
-Description: [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginAutofix/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginAutofix?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        # Autofix (Beets Plugin)
-        
-        The *beets-autofix* plugin helps you to automate the tasks that you keep repeating to maintain your library. 
-        
-        The plugin is a wrapper around the plugins that you already have in beets. It iterates through the items you have in your library and calls the individual plugins to execute their jobs as they are configured by you.
-        
-        
-        ## Installation
-        The plugin can be installed via:
-        
-        ```shell script
-        $ pip install beets-autofix
-        ```
-        
-        
-        ## Usage
-        
-        Invoke the plugin as:
-        
-            $ beet autofix [options] [QUERY...]
-        
-        
-        The following command line options are available:
-        
-        **--max_exec_time=MAX_EXEC_TIME [-m MAX_EXEC_TIME]**: Interrupt the execution after this number of seconds.
-        
-        **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
-        
-        
-        ## Configuration
-        By default all tasks are disabled:
-        
-        ```yaml
-        max_exec_time: 0
-        tasks:
-          missing_file_checker:
-            enabled: no
-          year_fixer:
-            enabled: no
-          audio_conversion:
-            enabled: no
-          tag_cleaner:
-            enabled: no
-          ab_data_fetcher:
-            enabled: no
-          xtractor:
-            enabled: no
-          genre_finder:
-            enabled: no
-        ```
-        
-        You need to override the default configuration and enable the tasks you want to run.
-        
-        The `max_exec_time` allows you to interrupt the execution after a certain number of seconds. For no limit set it to 0.
-        
-        
-        ## Tasks
-        The following tasks are available:
-        
-        ### Missing File Checker (task name: missing_file_checker) [related plugin: None]
-        This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
-        
-        
-        ### Year Fixer (task name: year_fixer) [related plugin: [yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)]
-        The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
-        
-        
-        ### Conversion (task name: audio_conversion) [related plugin: [convert](https://beets.readthedocs.io/en/stable/plugins/convert.html)]
-        This plugin is based on the `convert` plugin and triggers the conversion in two cases:
-        
-        - if the format of the item is does not correspond to the `format` specified in the `convert` plugin configuration
-        - if the bitrate of the item is greater than the `bitrate` specified in the `convert` plugin configuration
-        
-        In both cases the audio file will be converted according to the `convert` plugin configuration. The converted audio file will be attached to the library item whilst the original audio file will be deleted.
-        
-        ### Tag Cleaner (task name: tag_cleaner) [related plugin: [zero](https://beets.readthedocs.io/en/stable/plugins/zero.html)]
-        This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing. 
-        
-        
-        ### AcousticBrainz Data Fetcher (task name: ab_data_fetcher) [related plugin: [acousticbrainz](https://beets.readthedocs.io/en/stable/plugins/acousticbrainz.html)]
-        This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set. 
-        
-        The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
-        
-        
-        ### Xtractor(task name: xtractor) [related plugin: [xtractor](https://github.com/adamjakab/BeetsPluginXtractor)]
-        This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files. 
-        
-        
-        ### Genre Finder (task name: genre_finder) [related plugin: [lastgenre](https://beets.readthedocs.io/en/stable/plugins/lastgenre.html)]
-        This task will call the `lastgenre` plugin to find out the genre of a specific song. If that fails, it will fall back to the `genre_rosamerica` attribute estimated by the Essentia high level extractor and map the genre based on this table:
-        
-        ```text
-            "cla" -> "classical"
-            "dan" -> "dance"
-            "hip" -> "hip-hop"
-            "jaz" -> "jazz"
-            "pop" -> "pop"
-            "rhy" -> "rhythm and blues"
-            "roc" -> "rock"
-            "spe" -> "speech"
-        ```
-        
-        ## Issues
-        - If something is not working as expected please use the Issue tracker.
-        - If the documentation is not clear please use the Issue tracker.
-        - If you have a feature request please use the Issue tracker.
-        - In any other situation please use the Issue tracker.
-        
-        
-        ## Other plugins by the same author
-        
-        - [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
-        - [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
-        - [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
-        - [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
-        - [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
-        - [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
-        - [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
-        
-        
-        ## Final Remarks
-        Enjoy!
-        
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: beets>=1.4.9
+Requires-Dist: alive-progress
 Provides-Extra: tests
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginAutofix/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginAutofix/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginAutofix?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-autofix.svg)](https://pypi.org/project/beets-autofix/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# Autofix (Beets Plugin)
+
+The _beets-autofix_ plugin helps you to automate the tasks that you keep repeating to maintain your library.
+
+The plugin is a wrapper around the plugins that you already have in beets. It iterates through the items you have in your library and calls the individual plugins to execute their jobs as they are configured by you.
+
+## Installation
+
+The plugin can be installed via:
+
+```shell script
+$ pip install beets-autofix
+```
+
+## Usage
+
+Invoke the plugin as:
+
+    $ beet autofix [options] [QUERY...]
+
+The following command line options are available:
+
+**--max_exec_time=MAX_EXEC_TIME [-m MAX_EXEC_TIME]**: Interrupt the execution after this number of seconds.
+
+**--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
+
+## Configuration
+
+By default all tasks are disabled:
+
+```yaml
+max_exec_time: 0
+tasks:
+  missing_file_checker:
+    enabled: no
+  year_fixer:
+    enabled: no
+  audio_conversion:
+    enabled: no
+  tag_cleaner:
+    enabled: no
+  ab_data_fetcher:
+    enabled: no
+  xtractor:
+    enabled: no
+  genre_finder:
+    enabled: no
+```
+
+You need to override the default configuration and enable the tasks you want to run.
+
+The `max_exec_time` allows you to interrupt the execution after a certain number of seconds. For no limit set it to 0.
+
+## Tasks
+
+The following tasks are available:
+
+### Missing File Checker (task name: missing_file_checker) [related plugin: None]
+
+This task is not related to any plugin. It will iterate through all library items and check if the file indicated by the `path` attribute exists. If it does not exist, it deletes the library item.
+
+### Year Fixer (task name: year_fixer) [related plugin: [yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)]
+
+The YearFixer plugin will attempt to fix items with missing `year` or `original_year` attributes missing. The particularity of the `yearfixer` plugin is that given a specific release, to look for the `original_year` attribute, it will search for all recordings of the same title (by the same artist) in the MB database and chose the earliest year that song has been released.
+
+### Conversion (task name: audio_conversion) [related plugin: [convert](https://beets.readthedocs.io/en/stable/plugins/convert.html)]
+
+This plugin is based on the `convert` plugin and triggers the conversion in two cases:
+
+- if the format of the item is does not correspond to the `format` specified in the `convert` plugin configuration
+- if the bitrate of the item is greater than the `bitrate` specified in the `convert` plugin configuration
+
+In both cases the audio file will be converted according to the `convert` plugin configuration. The converted audio file will be attached to the library item whilst the original audio file will be deleted.
+
+### Tag Cleaner (task name: tag_cleaner) [related plugin: [zero](https://beets.readthedocs.io/en/stable/plugins/zero.html)]
+
+This task works with the `zero` plugin and triggers only if in the configuration you use the `fields` configuration option (it does not work with the `keep_fields` option for now). If any of those fields are found to be non-empty, the item will be passed to the `zero` plugin for processing.
+
+### AcousticBrainz Data Fetcher (task name: ab_data_fetcher) [related plugin: [acousticbrainz](https://beets.readthedocs.io/en/stable/plugins/acousticbrainz.html)]
+
+This task will check if any of the following attributes are missing from the library item and will call the acousticbrainz plugin to fetch such data from the acousticbrainz database. The task will then set the values for the missing attributes. If the `force` configuration option is set to `yes` in the configuration of the `acousticbrainz` plugin then all attributes will be set.
+
+The attributes checked and set are: `average_loudness`, `bpm`, `danceable`, `gender`, `genre_rosamerica`, `voice_instrumental`, `mood_acoustic`, `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_party`, `mood_relaxed`, `mood_sad` (some more to come soon)
+
+### Xtractor(task name: xtractor) [related plugin: [xtractor](https://github.com/adamjakab/BeetsPluginXtractor)]
+
+This task and the related plugin works on exactly the same attributes as the ones listed in the AcousticBrainz Data Fetcher task. The difference is that the `xtractor` plugin does not rely on external databases but uses the Essentia extractor binaries to extract such data from your audio files.
+
+### Genre Finder (task name: genre_finder) [related plugin: [lastgenre](https://beets.readthedocs.io/en/stable/plugins/lastgenre.html)]
+
+This task will call the `lastgenre` plugin to find out the genre of a specific song. If that fails, it will fall back to the `genre_rosamerica` attribute estimated by the Essentia high level extractor and map the genre based on this table:
+
+```text
+    "cla" -> "classical"
+    "dan" -> "dance"
+    "hip" -> "hip-hop"
+    "jaz" -> "jazz"
+    "pop" -> "pop"
+    "rhy" -> "rhythm and blues"
+    "roc" -> "rock"
+    "spe" -> "speech"
+```
+
+## Issues
+
+- If something is not working as expected please use the Issue tracker.
+- If the documentation is not clear please use the Issue tracker.
+- If you have a feature request please use the Issue tracker.
+- In any other situation please use the Issue tracker.
+
+## Other plugins by the same author
+
+- [beets-goingrunning](https://github.com/adamjakab/BeetsPluginGoingRunning)
+- [beets-xtractor](https://github.com/adamjakab/BeetsPluginXtractor)
+- [beets-yearfixer](https://github.com/adamjakab/BeetsPluginYearFixer)
+- [beets-autofix](https://github.com/adamjakab/BeetsPluginAutofix)
+- [beets-describe](https://github.com/adamjakab/BeetsPluginDescribe)
+- [beets-bpmanalyser](https://github.com/adamjakab/BeetsPluginBpmAnalyser)
+- [beets-template](https://github.com/adamjakab/BeetsPluginTemplate)
+
+## Final Remarks
+
+Enjoy!
```

### Comparing `beets-autofix-0.1.3/beets_autofix.egg-info/SOURCES.txt` & `beets_autofix-0.1.5/beets_autofix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/__init__.py` & `beets_autofix-0.1.5/beetsplug/autofix/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/about.py` & `beets_autofix-0.1.5/beetsplug/autofix/about.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  Created: 3/27/20, 3:52 PM
 #  License: See LICENSE.txt
 
 __author__ = u'Adam Jakab'
 __email__ = u'adam@jakab.pro'
 __copyright__ = u'Copyright (c) 2020, {} <{}>'.format(__author__, __email__)
 __license__ = u'License :: OSI Approved :: MIT License'
-__version__ = u'0.1.3'
+__version__ = u'0.1.5'
 __status__ = u'Kickstarted'
 
 __PACKAGE_TITLE__ = u'Autofix'
 __PACKAGE_NAME__ = u'beets-autofix'
 __PACKAGE_DESCRIPTION__ = u'A beets plugin to execute repetitive tasks in one go.',
 __PACKAGE_URL__ = u'https://github.com/adamjakab/BeetsPluginAutofix'
 __PLUGIN_NAME__ = u'autofix'
```

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/command.py` & `beets_autofix-0.1.5/beetsplug/autofix/command.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/common.py` & `beets_autofix-0.1.5/beetsplug/autofix/common.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/__init__.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/ab_data_fetcher.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/ab_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/audio_conversion.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/audio_conversion.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/genre_finder.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/genre_finder.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/missing_file_checker.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/missing_file_checker.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/tag_cleaner.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/tag_cleaner.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/xtractor.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/xtractor.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/beetsplug/autofix/task/year_fixer.py` & `beets_autofix-0.1.5/beetsplug/autofix/task/year_fixer.py`

 * *Files identical despite different names*

### Comparing `beets-autofix-0.1.3/setup.py` & `beets_autofix-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_description_content_type='text/markdown',
     platforms='ALL',
 
     include_package_data=True,
     test_suite='test',
     packages=['beetsplug.autofix', 'beetsplug.autofix.task'],
 
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 
     install_requires=[
         'beets>=1.4.9',
         'alive-progress',
     ],
 
     tests_require=[
@@ -54,12 +54,14 @@
     },
 
     classifiers=[
         'Topic :: Multimedia :: Sound/Audio',
         'License :: OSI Approved :: MIT License',
         'Environment :: Console',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

