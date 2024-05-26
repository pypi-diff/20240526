# Comparing `tmp/beets-yearfixer-0.0.4.tar.gz` & `tmp/beets_yearfixer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-yearfixer-0.0.4.tar", last modified: Thu Mar  3 20:50:38 2022, max compression
+gzip compressed data, was "beets_yearfixer-0.0.5.tar", last modified: Sun May 26 20:10:12 2024, max compression
```

## Comparing `beets-yearfixer-0.0.4.tar` & `beets_yearfixer-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beets_yearfixer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     7875 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/common.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/beetsplug/yearfixer/config_default.yml
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-03-03 20:50:38.000000 beets-yearfixer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-03-03 20:50:27.000000 beets-yearfixer-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:10:12.354147 beets_yearfixer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-26 20:10:12.354147 beets_yearfixer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:10:12.354147 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-26 20:10:12.000000 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 20:10:12.000000 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:10:12.000000 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 20:10:12.000000 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 20:10:12.000000 beets_yearfixer-0.0.5/beets_yearfixer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:10:12.350147 beets_yearfixer-0.0.5/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:10:12.354147 beets_yearfixer-0.0.5/beetsplug/yearfixer/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/beetsplug/yearfixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/beetsplug/yearfixer/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/beetsplug/yearfixer/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/beetsplug/yearfixer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/beetsplug/yearfixer/config_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 20:10:12.354147 beets_yearfixer-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-26 20:09:59.000000 beets_yearfixer-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beets-yearfixer-0.0.4/LICENSE.txt` & `beets_yearfixer-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-yearfixer-0.0.4/PKG-INFO` & `beets_yearfixer-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 Metadata-Version: 2.1
 Name: beets-yearfixer
-Version: 0.0.4
+Version: 0.0.5
 Summary: ('A beets plugin for fixing `original_year` and `year` tags on audio items.',)
 Home-page: https://github.com/adamjakab/BeetsPluginYearFixer
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
-Description: [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginYearFixer/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginYearFixer?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        # YearFixer (Beets Plugin)
-        
-        The *beets-yearfixer* plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried. 
-        
-        
-        ## Installation
-        The plugin can be installed via:
-        
-        
-            $pip install beets-yearfixer
-        
-        
-        Activate the plugin in your configuration file by adding `yearfixer` to the plugins section:
-        
-        ```yaml
-        plugins:
-            - yearfixer
-        ```
-        
-        ## Usage
-        
-        Invoke the plugin as:
-        
-            $ beet yearfixer [options] [QUERY...]
-        
-        
-        The following command line options are available:
-        
-        **--force [-f]**: Force setting the values on items even if the value has been previously set.
-        
-        **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
-        
-        
-        ## Configuration
-        The `force` options can also be set through the configuration like this: 
-        
-        ```yaml
-        force: yes
-        ```
-        
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
+Requires-Dist: requests
 Provides-Extra: tests
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginYearFixer/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginYearFixer?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# YearFixer (Beets Plugin)
+
+The _beets-yearfixer_ plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried.
+
+## Installation
+
+The plugin can be installed via:
+
+    $pip install beets-yearfixer
+
+Activate the plugin in your configuration file by adding `yearfixer` to the plugins section:
+
+```yaml
+plugins:
+  - yearfixer
+```
+
+## Usage
+
+Invoke the plugin as:
+
+    $ beet yearfixer [options] [QUERY...]
+
+The following command line options are available:
+
+**--force [-f]**: Force setting the values on items even if the value has been previously set.
+
+**--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
+
+## Configuration
+
+The `force` options can also be set through the configuration like this:
+
+```yaml
+force: yes
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

### Comparing `beets-yearfixer-0.0.4/README.md` & `beets_yearfixer-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,63 @@
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml)
 [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginYearFixer/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginYearFixer?branch=master)
 [![PyPi](https://img.shields.io/pypi/v/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
 
 # YearFixer (Beets Plugin)
 
-The *beets-yearfixer* plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried. 
-
+The _beets-yearfixer_ plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried.
 
 ## Installation
-The plugin can be installed via:
 
+The plugin can be installed via:
 
     $pip install beets-yearfixer
 
-
 Activate the plugin in your configuration file by adding `yearfixer` to the plugins section:
 
 ```yaml
 plugins:
-    - yearfixer
+  - yearfixer
 ```
 
 ## Usage
 
 Invoke the plugin as:
 
     $ beet yearfixer [options] [QUERY...]
 
-
 The following command line options are available:
 
 **--force [-f]**: Force setting the values on items even if the value has been previously set.
 
 **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
 
-
 ## Configuration
-The `force` options can also be set through the configuration like this: 
+
+The `force` options can also be set through the configuration like this:
 
 ```yaml
 force: yes
 ```
 
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
 ## Final Remarks
+
 Enjoy!
```

### Comparing `beets-yearfixer-0.0.4/beets_yearfixer.egg-info/PKG-INFO` & `beets_yearfixer-0.0.5/beets_yearfixer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,88 @@
 Metadata-Version: 2.1
 Name: beets-yearfixer
-Version: 0.0.4
+Version: 0.0.5
 Summary: ('A beets plugin for fixing `original_year` and `year` tags on audio items.',)
 Home-page: https://github.com/adamjakab/BeetsPluginYearFixer
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
-Description: [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginYearFixer/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginYearFixer?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        # YearFixer (Beets Plugin)
-        
-        The *beets-yearfixer* plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried. 
-        
-        
-        ## Installation
-        The plugin can be installed via:
-        
-        
-            $pip install beets-yearfixer
-        
-        
-        Activate the plugin in your configuration file by adding `yearfixer` to the plugins section:
-        
-        ```yaml
-        plugins:
-            - yearfixer
-        ```
-        
-        ## Usage
-        
-        Invoke the plugin as:
-        
-            $ beet yearfixer [options] [QUERY...]
-        
-        
-        The following command line options are available:
-        
-        **--force [-f]**: Force setting the values on items even if the value has been previously set.
-        
-        **--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
-        
-        
-        ## Configuration
-        The `force` options can also be set through the configuration like this: 
-        
-        ```yaml
-        force: yes
-        ```
-        
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
+Requires-Dist: requests
 Provides-Extra: tests
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginYearFixer/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginYearFixer/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginYearFixer?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-yearfixer.svg)](https://pypi.org/project/beets-yearfixer/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# YearFixer (Beets Plugin)
+
+The _beets-yearfixer_ plugin finds the `original_year` for each of your songs by querying the MusicBrainz database and finding the first release date that is associated with it. If the MB database query is unsuccessful, it will then use the other songs in the same album as reference and calculate the mean `original_year` between them. If this does not yield any results then the same will be done for all songs of the artist. For the `year` attribute the same procedure will be used except that the MB database is not queried.
+
+## Installation
+
+The plugin can be installed via:
+
+    $pip install beets-yearfixer
+
+Activate the plugin in your configuration file by adding `yearfixer` to the plugins section:
+
+```yaml
+plugins:
+  - yearfixer
+```
+
+## Usage
+
+Invoke the plugin as:
+
+    $ beet yearfixer [options] [QUERY...]
+
+The following command line options are available:
+
+**--force [-f]**: Force setting the values on items even if the value has been previously set.
+
+**--version [-v]**: Display the version number of the plugin. Useful when you need to report some issue and you have to state the version of the plugin you are using.
+
+## Configuration
+
+The `force` options can also be set through the configuration like this:
+
+```yaml
+force: yes
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

### Comparing `beets-yearfixer-0.0.4/beetsplug/yearfixer/__init__.py` & `beets_yearfixer-0.0.5/beetsplug/yearfixer/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-yearfixer-0.0.4/beetsplug/yearfixer/about.py` & `beets_yearfixer-0.0.5/beetsplug/yearfixer/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  Created: 3/27/20, 3:52 PM
 #  License: See LICENSE.txt
 
 __author__ = u'Adam Jakab'
 __email__ = u'adam@jakab.pro'
 __copyright__ = u'Copyright (c) 2020, {} <{}>'.format(__author__, __email__)
 __license__ = u'License :: OSI Approved :: MIT License'
-__version__ = u'0.0.4'
+__version__ = u'0.0.5'
 __status__ = u'Kickstarted'
 
 __PACKAGE_TITLE__ = u'YearFixer'
 __PACKAGE_NAME__ = u'beets-yearfixer'
 __PACKAGE_DESCRIPTION__ = u'A beets plugin for fixing `original_year` and `year` tags on audio items.',
 __PACKAGE_URL__ = u'https://github.com/adamjakab/BeetsPluginYearFixer'
 __PLUGIN_NAME__ = u'yearfixer'
```

### Comparing `beets-yearfixer-0.0.4/beetsplug/yearfixer/command.py` & `beets_yearfixer-0.0.5/beetsplug/yearfixer/command.py`

 * *Files identical despite different names*

### Comparing `beets-yearfixer-0.0.4/beetsplug/yearfixer/common.py` & `beets_yearfixer-0.0.5/beetsplug/yearfixer/common.py`

 * *Files identical despite different names*

### Comparing `beets-yearfixer-0.0.4/setup.py` & `beets_yearfixer-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     platforms='ALL',
 
     include_package_data=True,
     test_suite='test',
 
     packages=['beetsplug.yearfixer'],
 
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 
     install_requires=[
         'beets>=1.4.9',
         'requests'
     ],
 
     tests_require=[
@@ -56,12 +56,14 @@
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

