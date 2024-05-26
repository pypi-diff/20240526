# Comparing `tmp/beets-bpmanalyser-1.5.8.tar.gz` & `tmp/beets_bpmanalyser-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/BeetsPluginBpmAnalyser/BeetsPluginBpmAnalyser/dist/.tmp-4y_uhvlm/beets-bpmanalyser-1.5.8.tar", last modified: Sat May 11 17:51:50 2024, max compression
+gzip compressed data, was "beets_bpmanalyser-1.5.9.tar", last modified: Sun May 26 14:55:02 2024, max compression
```

## Comparing `beets-bpmanalyser-1.5.8.tar` & `beets_bpmanalyser-1.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     5915 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/analyser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7425 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-11 17:51:50.000000 beets-bpmanalyser-1.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-11 17:51:37.000000 beets-bpmanalyser-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:55:02.837258 beets_bpmanalyser-1.5.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-26 14:55:02.837258 beets_bpmanalyser-1.5.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6043 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:55:02.837258 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-26 14:55:02.000000 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-26 14:55:02.000000 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:55:02.000000 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 14:55:02.000000 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 14:55:02.000000 beets_bpmanalyser-1.5.9/beets_bpmanalyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:55:02.833258 beets_bpmanalyser-1.5.9/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:55:02.837258 beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/analyser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7425 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-26 14:55:02.837258 beets_bpmanalyser-1.5.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1725 2024-05-26 14:54:53.000000 beets_bpmanalyser-1.5.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beets-bpmanalyser-1.5.8/LICENSE.txt` & `beets_bpmanalyser-1.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.8/PKG-INFO` & `beets_bpmanalyser-1.5.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: beets-bpmanalyser
-Version: 1.5.8
-Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
-Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
-Author: Adam Jakab
-Author-email: adam@jakab.pro
-License: MIT
-Platform: ALL
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
 The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
 
 This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
```

### Comparing `beets-bpmanalyser-1.5.8/beets_bpmanalyser.egg-info/PKG-INFO` & `beets_bpmanalyser-1.5.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 Metadata-Version: 2.1
 Name: beets-bpmanalyser
-Version: 1.5.8
+Version: 1.5.9
 Summary: A beets plugin for analysing tempo of songs and storing it in the bpm tag.
 Home-page: https://github.com/adamjakab/BeetsPluginBpmAnalyser
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: beets>=1.4.9
+Requires-Dist: aubio
+Requires-Dist: numpy
+Requires-Dist: pydub
 
 [![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginBpmAnalyser/actions/workflows/test_release_deploy.yml)
 [![PyPi](https://img.shields.io/pypi/v/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-bpmanalyser.svg)](https://pypi.org/project/beets-bpmanalyser/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # BPM Analyser (Beets Plugin)
 
 The _beets-bpmanalyser_ plugin lets you analyse the tempo of the songs you have in your library and write the bpm information on the bpm tag of your media files.
 
 This plugin has a more powerful big brother which does much more than just extracting bpm: [beets-xtractor plugin](https://github.com/adamjakab/BeetsPluginXtractor).
```

### Comparing `beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/__init__.py` & `beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/analyser.py` & `beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/analyser.py`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.8/beetsplug/bpmanalyser/command.py` & `beets_bpmanalyser-1.5.9/beetsplug/bpmanalyser/command.py`

 * *Files identical despite different names*

### Comparing `beets-bpmanalyser-1.5.8/setup.py` & `beets_bpmanalyser-1.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     long_description=README,
     long_description_content_type='text/markdown',
     platforms='ALL',
     test_suite='test',
     
     include_package_data=True,
     packages=['beetsplug.bpmanalyser'],
+    
+    python_requires='>=3.8',
 
     install_requires=[
         'beets>=1.4.9',
         'aubio',
         'numpy',
         'pydub'
     ],
@@ -49,10 +51,14 @@
     ],
 
     classifiers=[
         'Topic :: Multimedia :: Sound/Audio',
         'License :: OSI Approved :: MIT License',
         'Environment :: Console',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

