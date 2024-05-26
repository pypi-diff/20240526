# Comparing `tmp/beets-xtractor-0.4.1.tar.gz` & `tmp/beets_xtractor-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets-xtractor-0.4.1.tar", last modified: Mon Apr  3 05:56:45 2023, max compression
+gzip compressed data, was "beets_xtractor-0.4.2.tar", last modified: Sun May 26 19:58:47 2024, max compression
```

## Comparing `beets-xtractor-0.4.1.tar` & `beets_xtractor-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:56:45.384871 beets-xtractor-0.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-03 05:56:45.384871 beets-xtractor-0.4.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9487 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:56:45.384871 beets-xtractor-0.4.1/beets_xtractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-03 05:56:45.000000 beets-xtractor-0.4.1/beets_xtractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-03 05:56:45.000000 beets-xtractor-0.4.1/beets_xtractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 05:56:45.000000 beets-xtractor-0.4.1/beets_xtractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-03 05:56:45.000000 beets-xtractor-0.4.1/beets_xtractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 05:56:45.000000 beets-xtractor-0.4.1/beets_xtractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:56:45.380871 beets-xtractor-0.4.1/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:56:45.384871 beets-xtractor-0.4.1/beetsplug/xtractor/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2619 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/beetsplug/xtractor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/beetsplug/xtractor/about.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13101 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/beetsplug/xtractor/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/beetsplug/xtractor/config_default.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2466 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/beetsplug/xtractor/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-04-03 05:56:45.384871 beets-xtractor-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1622 2023-04-03 05:56:35.000000 beets-xtractor-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:58:47.972017 beets_xtractor-0.4.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-05-26 19:58:47.972017 beets_xtractor-0.4.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9121 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:58:47.972017 beets_xtractor-0.4.2/beets_xtractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-05-26 19:58:47.000000 beets_xtractor-0.4.2/beets_xtractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-26 19:58:47.000000 beets_xtractor-0.4.2/beets_xtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:58:47.000000 beets_xtractor-0.4.2/beets_xtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 19:58:47.000000 beets_xtractor-0.4.2/beets_xtractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 19:58:47.000000 beets_xtractor-0.4.2/beets_xtractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:58:47.968017 beets_xtractor-0.4.2/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:58:47.972017 beets_xtractor-0.4.2/beetsplug/xtractor/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2619 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/beetsplug/xtractor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/beetsplug/xtractor/about.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13102 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/beetsplug/xtractor/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/beetsplug/xtractor/config_default.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2466 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/beetsplug/xtractor/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-26 19:58:47.972017 beets_xtractor-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1725 2024-05-26 19:58:39.000000 beets_xtractor-0.4.2/setup.py
```

### Comparing `beets-xtractor-0.4.1/LICENSE.txt` & `beets_xtractor-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-xtractor-0.4.1/PKG-INFO` & `beets_xtractor-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,122 +1,123 @@
 Metadata-Version: 2.1
 Name: beets-xtractor
-Version: 0.4.1
+Version: 0.4.2
 Summary: ('A beets plugin that extracts music descriptors from your audio files',)
 Home-page: https://github.com/adamjakab/BeetsPluginXtractor
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
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
-Provides-Extra: tests
 License-File: LICENSE.txt
+Requires-Dist: beets>=1.4.9
+Requires-Dist: pyyaml
+Provides-Extra: tests
 
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginXtractor/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginXtractor?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # Xtractor (Beets Plugin)
 
-The *beets-xtractor* plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
+The _beets-xtractor_ plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
 to obtain low and high level musical information from your songs.
 
 Currently, the following attributes are extracted for each library item:
-`bpm`, `danceability`, `beats_count`, `average_loudness`,  `danceable`, `gender`, `is_male`, `is_female`,
+`bpm`, `danceability`, `beats_count`, `average_loudness`, `danceable`, `gender`, `is_male`, `is_female`,
 `genre_rosamerica`, `voice_instrumental`, `is_voice`, `is_instrumental`, `mood_acoustic`,
 `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_sad`, `mood_party`, `mood_relaxed`, `mood_mirex`,
 `mood_mirex_cluster_1`, `mood_mirex_cluster_2`, `mood_mirex_cluster_3`, `mood_mirex_cluster_4`, `mood_mirex_cluster_5`
 
 ## Installation
+
 The plugin can be installed via:
 
 ```shell script
-$ pip install beets-xtractor
+pip install beets-xtractor
 ```
+
 and activated the usual way by adding `xtractor` to the list of plugins in your configuration:
 
 ```yaml
 plugins:
-    - xtractor
+  - xtractor
 ```
 
 ### Install the Essentia extractors
 
-You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits). You will need
-to compile this extractor yourself.
-The [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
-is somewhat complex but with some cross searching on the internet you will make it. If you are stuck you can use
-the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). Make sure you compile it with Gaia
-support (`--with-gaia`) otherwise will not be able to use the high level models.
+You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits).
+Please refer to the [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
+for the installation procedure for your OS. If you are stuck you can use
+the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). If you are compiling Essentia from source,
+make sure you compile it with Gaia support (`--with-gaia`) otherwise will not be able to use the high level models.
 
 ### Download the SVM models
 
-The second extractor uses prebuilt trained models for prediction. You need to download these from
-here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the more recent beta5 version.
+For computing the high-level descriptors you will need the prebuilt trained models for prediction. You need to download these from
+here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the most recent beta5 version.
 This means that your binaries must match this version. Put the downloaded models in any folder from which they can be
 accessed.
 
-### Precompiled packages
-
-If you happen to use Linux to run beets, the MusicPlayerPlus project provides pre-compiled packages that were split out from the main project and can be downloaded separately here: https://github.com/doctorfree/mpplus-essentia/releases.
-
-The package contains a precompiled extractor binary as well as the fitting SVM models (as of writing 2.1 beta5).
-
-`mpplus-essentia` provides the files you need for your beets configuration as `/usr/bin/essentia_streaming_extractor_music` and `/usr/share/mpplus-essentia/svm_models/*.history`
-
 ## Configuration
+
 All your configuration will need to go under the `xtractor` key. This is what your configuration should look like:
 
 ```yaml
 xtractor:
-    auto: no
-    dry-run: no
-    write: yes
-    threads: 1
-    force: no
-    quiet: no
-    keep_output: yes
-    keep_profiles: no
-    output_path: /mnt/data/xtraction_data
-    essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
-    extractor_profile:
-        highlevel:
-            svm_models:
-                - /mnt/data/extractors/beta5/svm_models/danceability.history
-                - /mnt/data/extractors/beta5/svm_models/gender.history
-                - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
-                - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
-                - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_happy.history
-                - /mnt/data/extractors/beta5/svm_models/mood_sad.history
-                - /mnt/data/extractors/beta5/svm_models/mood_party.history
-                - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
-                - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
-                - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
+  auto: no
+  dry-run: no
+  write: yes
+  threads: 1
+  force: no
+  quiet: no
+  keep_output: yes
+  keep_profiles: no
+  output_path: /mnt/data/xtraction_data
+  essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
+  extractor_profile:
+    highlevel:
+      svm_models:
+        - /mnt/data/extractors/beta5/svm_models/danceability.history
+        - /mnt/data/extractors/beta5/svm_models/gender.history
+        - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
+        - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
+        - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_happy.history
+        - /mnt/data/extractors/beta5/svm_models/mood_sad.history
+        - /mnt/data/extractors/beta5/svm_models/mood_party.history
+        - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
+        - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
+        - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
 ```
 
 First of all, you will need adjust all paths. Put the path of the extractor binary in `essentia_extractor` and
 substitute the location of the SVM models with your local path under the `svm_models` section. Finally, set
 the `output_path` to indicate where the extracted data files will be stored. If you do not set this, a temporary path
 will be used.
+will be used.
 
-**Note on shell tilde expansion**:  Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
+**Note on shell tilde expansion**: Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
 The entire section of `extractor_profile` is passed as-is to the essentia extractor binary and it will not do tilde expansion on your paths.
 The rest of the path keys such as `essentia_extractor` and `output_path` are used by the plugin itself and it will take
 care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
+care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
 
 By default both `keep_output` and `keep_profile` options are set to `no`. This means that after extraction (and the
 storage of the important information) the profile files used to pass to the extractors, and the json files created by
 the extractors will be deleted. There are various reasons you might want to keep these files. One is for debugging
 purposes. Another is to see what else is in these files (there is a lot) and maybe to use them with some other projects
 of yours. Lastly, you might want to keep these because the plugin only extracts data if these files are not present. If
 you store them, on a successive extraction, the plugin will skip the extraction and use these files (they are named
@@ -130,30 +131,28 @@
 
 The `write` option instructs the plugin to write the extracted attributes to the media file right away. Note that only `bpm` is actually written to the media file, all the other attributes are flex attributes and are only stored in the database.
 
 The `dry-run` option shows what would be done without actually doing it.
 
 **NOTE**: Please note that the `auto` option is not yet implemented. For now you will have to call the xtractor plugin manually.
 
-
 ## Usage
 
 Invoke the plugin as:
 
     $ beet xtractor [options] [QUERY...]
-    
+
 For a more verbose reporting use the `-v` flag on `beet`:
 
     $ beet -v xtractor [options] [QUERY...]
-    
+
 The plugin has also got a shorthand `xt` so you can also invoke it like this:
 
     $ beet xt [options] [QUERY...]
 
-
 The following command line options are available:
 
 **--dry-run [-d]**: Only show what would be done - displays the extracted values but does not store them in the library.
 
 **--write [-w]**: Write the values (bpm only) to the media files.
 
 **--threads=THREADS [-t THREADS]**: The number of concurrently running executions.
@@ -164,41 +163,39 @@
 
 **--quiet [-q]**: Run without any output.
 
 **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
 
 These command line options will override those specified in the configuration file.
 
-
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
 ## Credits
-Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
+Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
 ## References
+
 - [Essentia](https://essentia.upf.edu/index.html)
 - [SVM Models](https://essentia.upf.edu/svm_models/)
 - [Essentia Licensing](https://essentia.upf.edu/licensing_information.html)
 - [MTG Github - Music Technology Group](https://github.com/MTG)
 - [Acousticbrainz Downloads](https://acousticbrainz.org/download)
 
-
 ## Final Remarks
-Enjoy!
 
+Enjoy!
```

### Comparing `beets-xtractor-0.4.1/README.md` & `beets_xtractor-0.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,98 @@
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginXtractor/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginXtractor?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # Xtractor (Beets Plugin)
 
-The *beets-xtractor* plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
+The _beets-xtractor_ plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
 to obtain low and high level musical information from your songs.
 
 Currently, the following attributes are extracted for each library item:
-`bpm`, `danceability`, `beats_count`, `average_loudness`,  `danceable`, `gender`, `is_male`, `is_female`,
+`bpm`, `danceability`, `beats_count`, `average_loudness`, `danceable`, `gender`, `is_male`, `is_female`,
 `genre_rosamerica`, `voice_instrumental`, `is_voice`, `is_instrumental`, `mood_acoustic`,
 `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_sad`, `mood_party`, `mood_relaxed`, `mood_mirex`,
 `mood_mirex_cluster_1`, `mood_mirex_cluster_2`, `mood_mirex_cluster_3`, `mood_mirex_cluster_4`, `mood_mirex_cluster_5`
 
 ## Installation
+
 The plugin can be installed via:
 
 ```shell script
-$ pip install beets-xtractor
+pip install beets-xtractor
 ```
+
 and activated the usual way by adding `xtractor` to the list of plugins in your configuration:
 
 ```yaml
 plugins:
-    - xtractor
+  - xtractor
 ```
 
 ### Install the Essentia extractors
 
-You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits). You will need
-to compile this extractor yourself.
-The [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
-is somewhat complex but with some cross searching on the internet you will make it. If you are stuck you can use
-the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). Make sure you compile it with Gaia
-support (`--with-gaia`) otherwise will not be able to use the high level models.
+You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits).
+Please refer to the [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
+for the installation procedure for your OS. If you are stuck you can use
+the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). If you are compiling Essentia from source,
+make sure you compile it with Gaia support (`--with-gaia`) otherwise will not be able to use the high level models.
 
 ### Download the SVM models
 
-The second extractor uses prebuilt trained models for prediction. You need to download these from
-here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the more recent beta5 version.
+For computing the high-level descriptors you will need the prebuilt trained models for prediction. You need to download these from
+here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the most recent beta5 version.
 This means that your binaries must match this version. Put the downloaded models in any folder from which they can be
 accessed.
 
-### Precompiled packages
-
-If you happen to use Linux to run beets, the MusicPlayerPlus project provides pre-compiled packages that were split out from the main project and can be downloaded separately here: https://github.com/doctorfree/mpplus-essentia/releases.
-
-The package contains a precompiled extractor binary as well as the fitting SVM models (as of writing 2.1 beta5).
-
-`mpplus-essentia` provides the files you need for your beets configuration as `/usr/bin/essentia_streaming_extractor_music` and `/usr/share/mpplus-essentia/svm_models/*.history`
-
 ## Configuration
+
 All your configuration will need to go under the `xtractor` key. This is what your configuration should look like:
 
 ```yaml
 xtractor:
-    auto: no
-    dry-run: no
-    write: yes
-    threads: 1
-    force: no
-    quiet: no
-    keep_output: yes
-    keep_profiles: no
-    output_path: /mnt/data/xtraction_data
-    essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
-    extractor_profile:
-        highlevel:
-            svm_models:
-                - /mnt/data/extractors/beta5/svm_models/danceability.history
-                - /mnt/data/extractors/beta5/svm_models/gender.history
-                - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
-                - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
-                - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_happy.history
-                - /mnt/data/extractors/beta5/svm_models/mood_sad.history
-                - /mnt/data/extractors/beta5/svm_models/mood_party.history
-                - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
-                - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
-                - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
+  auto: no
+  dry-run: no
+  write: yes
+  threads: 1
+  force: no
+  quiet: no
+  keep_output: yes
+  keep_profiles: no
+  output_path: /mnt/data/xtraction_data
+  essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
+  extractor_profile:
+    highlevel:
+      svm_models:
+        - /mnt/data/extractors/beta5/svm_models/danceability.history
+        - /mnt/data/extractors/beta5/svm_models/gender.history
+        - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
+        - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
+        - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_happy.history
+        - /mnt/data/extractors/beta5/svm_models/mood_sad.history
+        - /mnt/data/extractors/beta5/svm_models/mood_party.history
+        - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
+        - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
+        - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
 ```
 
 First of all, you will need adjust all paths. Put the path of the extractor binary in `essentia_extractor` and
 substitute the location of the SVM models with your local path under the `svm_models` section. Finally, set
 the `output_path` to indicate where the extracted data files will be stored. If you do not set this, a temporary path
 will be used.
+will be used.
 
-**Note on shell tilde expansion**:  Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
+**Note on shell tilde expansion**: Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
 The entire section of `extractor_profile` is passed as-is to the essentia extractor binary and it will not do tilde expansion on your paths.
 The rest of the path keys such as `essentia_extractor` and `output_path` are used by the plugin itself and it will take
 care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
+care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
 
 By default both `keep_output` and `keep_profile` options are set to `no`. This means that after extraction (and the
 storage of the important information) the profile files used to pass to the extractors, and the json files created by
 the extractors will be deleted. There are various reasons you might want to keep these files. One is for debugging
 purposes. Another is to see what else is in these files (there is a lot) and maybe to use them with some other projects
 of yours. Lastly, you might want to keep these because the plugin only extracts data if these files are not present. If
 you store them, on a successive extraction, the plugin will skip the extraction and use these files (they are named
@@ -109,30 +106,28 @@
 
 The `write` option instructs the plugin to write the extracted attributes to the media file right away. Note that only `bpm` is actually written to the media file, all the other attributes are flex attributes and are only stored in the database.
 
 The `dry-run` option shows what would be done without actually doing it.
 
 **NOTE**: Please note that the `auto` option is not yet implemented. For now you will have to call the xtractor plugin manually.
 
-
 ## Usage
 
 Invoke the plugin as:
 
     $ beet xtractor [options] [QUERY...]
-    
+
 For a more verbose reporting use the `-v` flag on `beet`:
 
     $ beet -v xtractor [options] [QUERY...]
-    
+
 The plugin has also got a shorthand `xt` so you can also invoke it like this:
 
     $ beet xt [options] [QUERY...]
 
-
 The following command line options are available:
 
 **--dry-run [-d]**: Only show what would be done - displays the extracted values but does not store them in the library.
 
 **--write [-w]**: Write the values (bpm only) to the media files.
 
 **--threads=THREADS [-t THREADS]**: The number of concurrently running executions.
@@ -143,41 +138,39 @@
 
 **--quiet [-q]**: Run without any output.
 
 **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
 
 These command line options will override those specified in the configuration file.
 
-
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
 ## Credits
-Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
+Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
 ## References
+
 - [Essentia](https://essentia.upf.edu/index.html)
 - [SVM Models](https://essentia.upf.edu/svm_models/)
 - [Essentia Licensing](https://essentia.upf.edu/licensing_information.html)
 - [MTG Github - Music Technology Group](https://github.com/MTG)
 - [Acousticbrainz Downloads](https://acousticbrainz.org/download)
 
-
 ## Final Remarks
-Enjoy!
 
+Enjoy!
```

### Comparing `beets-xtractor-0.4.1/beets_xtractor.egg-info/PKG-INFO` & `beets_xtractor-0.4.2/beets_xtractor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,122 +1,123 @@
 Metadata-Version: 2.1
 Name: beets-xtractor
-Version: 0.4.1
+Version: 0.4.2
 Summary: ('A beets plugin that extracts music descriptors from your audio files',)
 Home-page: https://github.com/adamjakab/BeetsPluginXtractor
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
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
-Provides-Extra: tests
 License-File: LICENSE.txt
+Requires-Dist: beets>=1.4.9
+Requires-Dist: pyyaml
+Provides-Extra: tests
 
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginXtractor/actions/workflows/test_release_deploy.yml)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginXtractor/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginXtractor?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-xtractor.svg)](https://pypi.org/project/beets-xtractor/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # Xtractor (Beets Plugin)
 
-The *beets-xtractor* plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
+The _beets-xtractor_ plugin lets you, through the use of the [Essentia](https://essentia.upf.edu/index.html) extractors,
 to obtain low and high level musical information from your songs.
 
 Currently, the following attributes are extracted for each library item:
-`bpm`, `danceability`, `beats_count`, `average_loudness`,  `danceable`, `gender`, `is_male`, `is_female`,
+`bpm`, `danceability`, `beats_count`, `average_loudness`, `danceable`, `gender`, `is_male`, `is_female`,
 `genre_rosamerica`, `voice_instrumental`, `is_voice`, `is_instrumental`, `mood_acoustic`,
 `mood_aggressive`, `mood_electronic`, `mood_happy`, `mood_sad`, `mood_party`, `mood_relaxed`, `mood_mirex`,
 `mood_mirex_cluster_1`, `mood_mirex_cluster_2`, `mood_mirex_cluster_3`, `mood_mirex_cluster_4`, `mood_mirex_cluster_5`
 
 ## Installation
+
 The plugin can be installed via:
 
 ```shell script
-$ pip install beets-xtractor
+pip install beets-xtractor
 ```
+
 and activated the usual way by adding `xtractor` to the list of plugins in your configuration:
 
 ```yaml
 plugins:
-    - xtractor
+  - xtractor
 ```
 
 ### Install the Essentia extractors
 
-You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits). You will need
-to compile this extractor yourself.
-The [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
-is somewhat complex but with some cross searching on the internet you will make it. If you are stuck you can use
-the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). Make sure you compile it with Gaia
-support (`--with-gaia`) otherwise will not be able to use the high level models.
+You will also need the `streaming_extractor_music` binary extractor from the [Essentia project](#credits).
+Please refer to the [official installation documentation](https://essentia.upf.edu/installing.html#compiling-essentia-from-source)
+for the installation procedure for your OS. If you are stuck you can use
+the [Issue tracker](https://github.com/adamjakab/BeetsPluginXtractor/issues). If you are compiling Essentia from source,
+make sure you compile it with Gaia support (`--with-gaia`) otherwise will not be able to use the high level models.
 
 ### Download the SVM models
 
-The second extractor uses prebuilt trained models for prediction. You need to download these from
-here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the more recent beta5 version.
+For computing the high-level descriptors you will need the prebuilt trained models for prediction. You need to download these from
+here: [SVM Models](https://essentia.upf.edu/svm_models/). I suggest that you download the most recent beta5 version.
 This means that your binaries must match this version. Put the downloaded models in any folder from which they can be
 accessed.
 
-### Precompiled packages
-
-If you happen to use Linux to run beets, the MusicPlayerPlus project provides pre-compiled packages that were split out from the main project and can be downloaded separately here: https://github.com/doctorfree/mpplus-essentia/releases.
-
-The package contains a precompiled extractor binary as well as the fitting SVM models (as of writing 2.1 beta5).
-
-`mpplus-essentia` provides the files you need for your beets configuration as `/usr/bin/essentia_streaming_extractor_music` and `/usr/share/mpplus-essentia/svm_models/*.history`
-
 ## Configuration
+
 All your configuration will need to go under the `xtractor` key. This is what your configuration should look like:
 
 ```yaml
 xtractor:
-    auto: no
-    dry-run: no
-    write: yes
-    threads: 1
-    force: no
-    quiet: no
-    keep_output: yes
-    keep_profiles: no
-    output_path: /mnt/data/xtraction_data
-    essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
-    extractor_profile:
-        highlevel:
-            svm_models:
-                - /mnt/data/extractors/beta5/svm_models/danceability.history
-                - /mnt/data/extractors/beta5/svm_models/gender.history
-                - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
-                - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
-                - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
-                - /mnt/data/extractors/beta5/svm_models/mood_happy.history
-                - /mnt/data/extractors/beta5/svm_models/mood_sad.history
-                - /mnt/data/extractors/beta5/svm_models/mood_party.history
-                - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
-                - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
-                - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
+  auto: no
+  dry-run: no
+  write: yes
+  threads: 1
+  force: no
+  quiet: no
+  keep_output: yes
+  keep_profiles: no
+  output_path: /mnt/data/xtraction_data
+  essentia_extractor: /mnt/data/extractors/beta5/streaming_extractor_music
+  extractor_profile:
+    highlevel:
+      svm_models:
+        - /mnt/data/extractors/beta5/svm_models/danceability.history
+        - /mnt/data/extractors/beta5/svm_models/gender.history
+        - /mnt/data/extractors/beta5/svm_models/genre_rosamerica.history
+        - /mnt/data/extractors/beta5/svm_models/mood_acoustic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_aggressive.history
+        - /mnt/data/extractors/beta5/svm_models/mood_electronic.history
+        - /mnt/data/extractors/beta5/svm_models/mood_happy.history
+        - /mnt/data/extractors/beta5/svm_models/mood_sad.history
+        - /mnt/data/extractors/beta5/svm_models/mood_party.history
+        - /mnt/data/extractors/beta5/svm_models/mood_relaxed.history
+        - /mnt/data/extractors/beta5/svm_models/voice_instrumental.history
+        - /mnt/data/extractors/beta5/svm_models/moods_mirex.history
 ```
 
 First of all, you will need adjust all paths. Put the path of the extractor binary in `essentia_extractor` and
 substitute the location of the SVM models with your local path under the `svm_models` section. Finally, set
 the `output_path` to indicate where the extracted data files will be stored. If you do not set this, a temporary path
 will be used.
+will be used.
 
-**Note on shell tilde expansion**:  Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
+**Note on shell tilde expansion**: Please note that you cannot use shell expansion on the `svm_models` (i.e.: do not use `~` for your home folder).
 The entire section of `extractor_profile` is passed as-is to the essentia extractor binary and it will not do tilde expansion on your paths.
 The rest of the path keys such as `essentia_extractor` and `output_path` are used by the plugin itself and it will take
 care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
+care of expanding the tilde symbol (`~`) to the home directory of the user running the script.
 
 By default both `keep_output` and `keep_profile` options are set to `no`. This means that after extraction (and the
 storage of the important information) the profile files used to pass to the extractors, and the json files created by
 the extractors will be deleted. There are various reasons you might want to keep these files. One is for debugging
 purposes. Another is to see what else is in these files (there is a lot) and maybe to use them with some other projects
 of yours. Lastly, you might want to keep these because the plugin only extracts data if these files are not present. If
 you store them, on a successive extraction, the plugin will skip the extraction and use these files (they are named
@@ -130,30 +131,28 @@
 
 The `write` option instructs the plugin to write the extracted attributes to the media file right away. Note that only `bpm` is actually written to the media file, all the other attributes are flex attributes and are only stored in the database.
 
 The `dry-run` option shows what would be done without actually doing it.
 
 **NOTE**: Please note that the `auto` option is not yet implemented. For now you will have to call the xtractor plugin manually.
 
-
 ## Usage
 
 Invoke the plugin as:
 
     $ beet xtractor [options] [QUERY...]
-    
+
 For a more verbose reporting use the `-v` flag on `beet`:
 
     $ beet -v xtractor [options] [QUERY...]
-    
+
 The plugin has also got a shorthand `xt` so you can also invoke it like this:
 
     $ beet xt [options] [QUERY...]
 
-
 The following command line options are available:
 
 **--dry-run [-d]**: Only show what would be done - displays the extracted values but does not store them in the library.
 
 **--write [-w]**: Write the values (bpm only) to the media files.
 
 **--threads=THREADS [-t THREADS]**: The number of concurrently running executions.
@@ -164,41 +163,39 @@
 
 **--quiet [-q]**: Run without any output.
 
 **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
 
 These command line options will override those specified in the configuration file.
 
-
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
 ## Credits
-Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
+Essentia is an open-source C++ library with Python bindings for audio analysis and audio-based music information retrieval. It is released under the Affero GPLv3 license and is also available under proprietary license upon request. This plugin is just a mere wrapper around this library. [Learn more about the Essentia project](http://essentia.upf.edu)
 
 ## References
+
 - [Essentia](https://essentia.upf.edu/index.html)
 - [SVM Models](https://essentia.upf.edu/svm_models/)
 - [Essentia Licensing](https://essentia.upf.edu/licensing_information.html)
 - [MTG Github - Music Technology Group](https://github.com/MTG)
 - [Acousticbrainz Downloads](https://acousticbrainz.org/download)
 
-
 ## Final Remarks
-Enjoy!
 
+Enjoy!
```

### Comparing `beets-xtractor-0.4.1/beetsplug/xtractor/__init__.py` & `beets_xtractor-0.4.2/beetsplug/xtractor/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-xtractor-0.4.1/beetsplug/xtractor/about.py` & `beets_xtractor-0.4.2/beetsplug/xtractor/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  License: See LICENSE.txt
 
 __author__ = u'Adam Jakab'
 __email__ = u'adam@jakab.pro'
 __copyright__ = u'Copyright (c) 2020, {} <{}>'.format(__author__, __email__)
 __license__ = u'License :: OSI Approved :: MIT License'
-__version__ = u'0.4.1'
+__version__ = u'0.4.2'
 __status__ = u'Building'
 
 __PACKAGE_TITLE__ = u'Xtractor'
 __PACKAGE_NAME__ = u'beets-xtractor'
 __PACKAGE_DESCRIPTION__ = u'A beets plugin that extracts music descriptors ' \
                           u'from your audio files',
 __PACKAGE_URL__ = u'https://github.com/adamjakab/BeetsPluginXtractor'
```

### Comparing `beets-xtractor-0.4.1/beetsplug/xtractor/command.py` & `beets_xtractor-0.4.2/beetsplug/xtractor/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #  Copyright: Copyright (c) 2020., Adam Jakab
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  License: See LICENSE.txt
 
+from concurrent import futures
 import hashlib
 import json
-import os
 import multiprocessing
-import tempfile
-from concurrent import futures
 from optparse import OptionParser
+import os
 from subprocess import Popen, PIPE
+import tempfile
 
 import yaml
+
 from beets import dbcore
 from beets.library import Library, Item, parse_query_string
 from beets.ui import Subcommand, decargs
-from confuse import Subview
 from beetsplug.xtractor import helper
+from confuse import Subview
 
 
 class XtractorCommand(Subcommand):
     config: Subview = None
 
     lib = None
     query = None
```

### Comparing `beets-xtractor-0.4.1/beetsplug/xtractor/config_default.yml` & `beets_xtractor-0.4.2/beetsplug/xtractor/config_default.yml`

 * *Files identical despite different names*

### Comparing `beets-xtractor-0.4.1/beetsplug/xtractor/helper.py` & `beets_xtractor-0.4.2/beetsplug/xtractor/helper.py`

 * *Files identical despite different names*

### Comparing `beets-xtractor-0.4.1/setup.py` & `beets_xtractor-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,34 +33,36 @@
     long_description_content_type='text/markdown',
     platforms='ALL',
 
     include_package_data=True,
     test_suite='test',
     packages=['beetsplug.xtractor'],
 
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 
     install_requires=[
         'beets>=1.4.9',
-        'PyYAML'
+        'pyyaml'
     ],
 
     tests_require=[
         'pytest', 'nose', 'coverage',
-        'mock', 'six', 'yaml',
+        'mock', 'six', 'pyyaml',
     ],
 
     # Extras needed during testing
     extras_require={
         'tests': [],
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

