# Comparing `tmp/beets-describe-0.0.4.tar.gz` & `tmp/beets_describe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beets-describe-0.0.4.tar", last modified: Fri Feb 25 10:57:06 2022, max compression
+gzip compressed data, was "beets_describe-0.0.5.tar", last modified: Sun May 26 15:39:46 2024, max compression
```

## Comparing `beets-describe-0.0.4.tar` & `beets_describe-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 10:57:06.000000 beets-describe-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-25 10:56:57.000000 beets-describe-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-02-25 10:56:57.000000 beets-describe-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12481 2022-02-25 10:57:06.000000 beets-describe-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10242 2022-02-25 10:56:57.000000 beets-describe-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12481 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beets_describe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beetsplug/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 10:57:06.000000 beets-describe-0.0.4/beetsplug/describe/
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-02-25 10:56:57.000000 beets-describe-0.0.4/beetsplug/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-02-25 10:56:57.000000 beets-describe-0.0.4/beetsplug/describe/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     7625 2022-02-25 10:56:57.000000 beets-describe-0.0.4/beetsplug/describe/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-02-25 10:56:57.000000 beets-describe-0.0.4/beetsplug/describe/common.py
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-25 10:56:57.000000 beets-describe-0.0.4/beetsplug/describe/config_default.yml
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-25 10:57:06.000000 beets-describe-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-02-25 10:56:57.000000 beets-describe-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:39:46.466776 beets_describe-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 15:39:37.000000 beets_describe-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-26 15:39:37.000000 beets_describe-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-26 15:39:46.466776 beets_describe-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-26 15:39:37.000000 beets_describe-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:39:46.466776 beets_describe-0.0.5/beets_describe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-26 15:39:46.000000 beets_describe-0.0.5/beets_describe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-26 15:39:46.000000 beets_describe-0.0.5/beets_describe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:39:46.000000 beets_describe-0.0.5/beets_describe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-26 15:39:46.000000 beets_describe-0.0.5/beets_describe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 15:39:46.000000 beets_describe-0.0.5/beets_describe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:39:46.466776 beets_describe-0.0.5/beetsplug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:39:46.466776 beets_describe-0.0.5/beetsplug/describe/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 15:39:37.000000 beets_describe-0.0.5/beetsplug/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-26 15:39:37.000000 beets_describe-0.0.5/beetsplug/describe/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-26 15:39:37.000000 beets_describe-0.0.5/beetsplug/describe/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-26 15:39:37.000000 beets_describe-0.0.5/beetsplug/describe/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 15:39:37.000000 beets_describe-0.0.5/beetsplug/describe/config_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 15:39:46.466776 beets_describe-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-26 15:39:37.000000 beets_describe-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beets-describe-0.0.4/LICENSE.txt` & `beets_describe-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beets-describe-0.0.4/PKG-INFO` & `beets_describe-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,214 +1,192 @@
-Metadata-Version: 2.1
-Name: beets-describe
-Version: 0.0.4
-Summary: ('A beets plugin that describes attributes in depth',)
-Home-page: https://github.com/adamjakab/BeetsPluginDescribe
-Author: Adam Jakab
-Author-email: adam@jakab.pro
-License: MIT
-Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginDescribe.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginDescribe)
-        [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginDescribe/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginDescribe?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-describe.svg)](https://pypi.org/project/beets-describe/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-describe.svg)](https://pypi.org/project/beets-describe/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        
-        # Describe (Beets Plugin)
-        
-        The *beets-describe* plugin attempts to give you the full picture on a single attribute of your library item.
-        
-        **NOTE: Under heavy development but works!**
-        
-        
-        ## Installation:
-        
-        ```shell script
-        $ pip install beets-describe
-        ```
-        
-        and activate the plugin the usual way
-        ```yaml
-        plugins:
-            - describe
-        ```
-        
-        ## Usage:
-        
-        ```bash
-        beet describe field_name
-        ```
-        
-        You can of course add any queries after the name of the field to describe such as:
-        
-        ```bash
-        beet describe genre albumartist:'Various Artists'
-        ```
-        
-        ## Sample Output
-        
-        `beet describe bpm`
-        
-        ```text
-        ┌────────────────┬────────────────────────────┐
-        │ Name           │                      Value │
-        ╞════════════════╪════════════════════════════╡
-        │ Field name     │                        bpm │
-        ├────────────────┼────────────────────────────┤
-        │ Field type     │ beets.dbcore.types.Integer │
-        ├────────────────┼────────────────────────────┤
-        │ Count          │                       1392 │
-        ├────────────────┼────────────────────────────┤
-        │ Min            │              65.9922409058 │
-        ├────────────────┼────────────────────────────┤
-        │ Max            │                      185.0 │
-        ├────────────────┼────────────────────────────┤
-        │ Mean           │         122.99097545119291 │
-        ├────────────────┼────────────────────────────┤
-        │ Median         │                      122.0 │
-        ├────────────────┼────────────────────────────┤
-        │ Empty          │                          0 │
-        ├────────────────┼────────────────────────────┤
-        │ Unique         │                        649 │
-        ├────────────────┼────────────────────────────┤
-        │ Most frequent  │                  122.0(22) │
-        ├────────────────┼────────────────────────────┤
-        │ Least frequent │           117.853546143(1) │
-        └────────────────┴────────────────────────────┘
-        Distribution(bins=10) histogram
-        66.0 - 77.9    [ 30]  ████▊
-        77.9 - 89.8    [ 73]  ███████████▍
-        89.8 - 101.7   [203]  ███████████████████████████████▊
-        101.7 - 113.6  [221]  ██████████████████████████████████▌
-        113.6 - 125.5  [256]  ████████████████████████████████████████
-        125.5 - 137.4  [208]  ████████████████████████████████▌
-        137.4 - 149.3  [183]  ████████████████████████████▋
-        149.3 - 161.2  [ 87]  █████████████▋
-        161.2 - 173.1  [107]  ████████████████▊
-        173.1 - 185.0  [ 24]  ███▊
-        ```
-        
-        
-        `beet describe genre`
-        
-        ```text
-        ┌────────────────┬───────────────────────────┐
-        │ Name           │                     Value │
-        ╞════════════════╪═══════════════════════════╡
-        │ Field name     │                     genre │
-        ├────────────────┼───────────────────────────┤
-        │ Field type     │ beets.dbcore.types.String │
-        ├────────────────┼───────────────────────────┤
-        │ Count          │                      1392 │
-        ├────────────────┼───────────────────────────┤
-        │ Empty          │                        19 │
-        ├────────────────┼───────────────────────────┤
-        │ Unique         │                        91 │
-        ├────────────────┼───────────────────────────┤
-        │ Most frequent  │               Oldies(202) │
-        ├────────────────┼───────────────────────────┤
-        │ Least frequent │              Post-Punk(1) │
-        └────────────────┴───────────────────────────┘
-        Unique element histogram
-        Oldies                  [202]  ████████████████████████████████████████
-        Classic Rock            [139]  ███████████████████████████▌
-        Soul                    [124]  ████████████████████████▌
-        Blues                   [120]  ███████████████████████▊
-        Rock                    [109]  █████████████████████▋
-        Pop                     [105]  ████████████████████▊
-        Dance                   [ 86]  █████████████████
-        New Wave                [ 48]  █████████▌
-        Reggae                  [ 44]  ████████▊
-        Heavy Metal             [ 33]  ██████▌
-        Trance                  [ 24]  ████▊
-        Blues Rock              [ 20]  ████
-        Jazz                    [ 20]  ████
-                                [ 19]  ███▊
-        Soundtrack              [ 17]  ███▍
-        Ska                     [ 16]  ███▏
-        Synthpop                [ 16]  ███▏
-        Rap                     [ 15]  ███
-        Pop Rock                [ 14]  ██▊
-        Funk                    [ 12]  ██▍
-        Metal                   [ 12]  ██▍
-        Alternative Metal       [ 12]  ██▍
-        Alternative Rock        [ 11]  ██▏
-        Soft Rock               [ 10]  ██
-        Hard Rock               [ 10]  ██
-        Singer-Songwriter       [  9]  █▊
-        Rockabilly              [  8]  █▋
-        Metalcore               [  6]  █▎
-        Electronic              [  6]  █▎
-        Rock And Roll           [  6]  █▎
-        R&B                     [  6]  █▎
-        House                   [  5]  █
-        Disco                   [  5]  █
-        Progressive Rock        [  5]  █
-        Psychedelic Rock        [  5]  █
-        Punk Rock               [  4]  ▊
-        Thrash Metal            [  4]  ▊
-        Progressive Metal       [  4]  ▊
-        Contemporary R&B        [  3]  ▋
-        Nu Metal                [  3]  ▋
-        Symphonic Metal         [  3]  ▋
-        Funk Soul               [  3]  ▋
-        World Music             [  3]  ▋
-        Death Metal             [  3]  ▋
-        Britpop                 [  2]  ▍
-        Industrial Metal        [  2]  ▍
-        Contemporary Classical  [  2]  ▍
-        Post-Grunge             [  2]  ▍
-        Psychedelic             [  2]  ▍
-        Motown                  [  2]  ▍
-        Glam Rock               [  2]  ▍
-        Rock, Hard Rock, Metal  [  2]  ▍
-        Blue-Eyed Soul          [  2]  ▍
-        Black Metal             [  2]  ▍
-        Indie Rock              [  2]  ▍
-        Indie Pop               [  2]  ▍
-        Industrial              [  2]  ▍
-        Pop Punk                [  2]  ▍
-        Surf Rock               [  2]  ▍
-        Hip Hop                 [  1]  ▎
-        Gospel                  [  1]  ▎
-        Ragga                   [  1]  ▎
-        Indie                   [  1]  ▎
-        Speed Metal             [  1]  ▎
-        Gypsy Jazz              [  1]  ▎
-        ```
-        
-        
-        ## Configuration
-        There are no configuration options for this plugin.
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
-Platform: ALL
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: tests
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginDescribe/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginDescribe/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginDescribe/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginDescribe?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-describe.svg)](https://pypi.org/project/beets-describe/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-describe.svg)](https://pypi.org/project/beets-describe/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# Describe (Beets Plugin)
+
+The _beets-describe_ plugin attempts to give you the full picture on a single attribute of your library item.
+
+**NOTE: Under heavy development but works!**
+
+## Installation:
+
+```shell script
+$ pip install beets-describe
+```
+
+and activate the plugin the usual way
+
+```yaml
+plugins:
+  - describe
+```
+
+## Usage:
+
+```bash
+beet describe field_name
+```
+
+You can of course add any queries after the name of the field to describe such as:
+
+```bash
+beet describe genre albumartist:'Various Artists'
+```
+
+## Sample Output
+
+`beet describe bpm`
+
+```text
+┌────────────────┬────────────────────────────┐
+│ Name           │                      Value │
+╞════════════════╪════════════════════════════╡
+│ Field name     │                        bpm │
+├────────────────┼────────────────────────────┤
+│ Field type     │ beets.dbcore.types.Integer │
+├────────────────┼────────────────────────────┤
+│ Count          │                       1392 │
+├────────────────┼────────────────────────────┤
+│ Min            │              65.9922409058 │
+├────────────────┼────────────────────────────┤
+│ Max            │                      185.0 │
+├────────────────┼────────────────────────────┤
+│ Mean           │         122.99097545119291 │
+├────────────────┼────────────────────────────┤
+│ Median         │                      122.0 │
+├────────────────┼────────────────────────────┤
+│ Empty          │                          0 │
+├────────────────┼────────────────────────────┤
+│ Unique         │                        649 │
+├────────────────┼────────────────────────────┤
+│ Most frequent  │                  122.0(22) │
+├────────────────┼────────────────────────────┤
+│ Least frequent │           117.853546143(1) │
+└────────────────┴────────────────────────────┘
+Distribution(bins=10) histogram
+66.0 - 77.9    [ 30]  ████▊
+77.9 - 89.8    [ 73]  ███████████▍
+89.8 - 101.7   [203]  ███████████████████████████████▊
+101.7 - 113.6  [221]  ██████████████████████████████████▌
+113.6 - 125.5  [256]  ████████████████████████████████████████
+125.5 - 137.4  [208]  ████████████████████████████████▌
+137.4 - 149.3  [183]  ████████████████████████████▋
+149.3 - 161.2  [ 87]  █████████████▋
+161.2 - 173.1  [107]  ████████████████▊
+173.1 - 185.0  [ 24]  ███▊
+```
+
+`beet describe genre`
+
+```text
+┌────────────────┬───────────────────────────┐
+│ Name           │                     Value │
+╞════════════════╪═══════════════════════════╡
+│ Field name     │                     genre │
+├────────────────┼───────────────────────────┤
+│ Field type     │ beets.dbcore.types.String │
+├────────────────┼───────────────────────────┤
+│ Count          │                      1392 │
+├────────────────┼───────────────────────────┤
+│ Empty          │                        19 │
+├────────────────┼───────────────────────────┤
+│ Unique         │                        91 │
+├────────────────┼───────────────────────────┤
+│ Most frequent  │               Oldies(202) │
+├────────────────┼───────────────────────────┤
+│ Least frequent │              Post-Punk(1) │
+└────────────────┴───────────────────────────┘
+Unique element histogram
+Oldies                  [202]  ████████████████████████████████████████
+Classic Rock            [139]  ███████████████████████████▌
+Soul                    [124]  ████████████████████████▌
+Blues                   [120]  ███████████████████████▊
+Rock                    [109]  █████████████████████▋
+Pop                     [105]  ████████████████████▊
+Dance                   [ 86]  █████████████████
+New Wave                [ 48]  █████████▌
+Reggae                  [ 44]  ████████▊
+Heavy Metal             [ 33]  ██████▌
+Trance                  [ 24]  ████▊
+Blues Rock              [ 20]  ████
+Jazz                    [ 20]  ████
+                        [ 19]  ███▊
+Soundtrack              [ 17]  ███▍
+Ska                     [ 16]  ███▏
+Synthpop                [ 16]  ███▏
+Rap                     [ 15]  ███
+Pop Rock                [ 14]  ██▊
+Funk                    [ 12]  ██▍
+Metal                   [ 12]  ██▍
+Alternative Metal       [ 12]  ██▍
+Alternative Rock        [ 11]  ██▏
+Soft Rock               [ 10]  ██
+Hard Rock               [ 10]  ██
+Singer-Songwriter       [  9]  █▊
+Rockabilly              [  8]  █▋
+Metalcore               [  6]  █▎
+Electronic              [  6]  █▎
+Rock And Roll           [  6]  █▎
+R&B                     [  6]  █▎
+House                   [  5]  █
+Disco                   [  5]  █
+Progressive Rock        [  5]  █
+Psychedelic Rock        [  5]  █
+Punk Rock               [  4]  ▊
+Thrash Metal            [  4]  ▊
+Progressive Metal       [  4]  ▊
+Contemporary R&B        [  3]  ▋
+Nu Metal                [  3]  ▋
+Symphonic Metal         [  3]  ▋
+Funk Soul               [  3]  ▋
+World Music             [  3]  ▋
+Death Metal             [  3]  ▋
+Britpop                 [  2]  ▍
+Industrial Metal        [  2]  ▍
+Contemporary Classical  [  2]  ▍
+Post-Grunge             [  2]  ▍
+Psychedelic             [  2]  ▍
+Motown                  [  2]  ▍
+Glam Rock               [  2]  ▍
+Rock, Hard Rock, Metal  [  2]  ▍
+Blue-Eyed Soul          [  2]  ▍
+Black Metal             [  2]  ▍
+Indie Rock              [  2]  ▍
+Indie Pop               [  2]  ▍
+Industrial              [  2]  ▍
+Pop Punk                [  2]  ▍
+Surf Rock               [  2]  ▍
+Hip Hop                 [  1]  ▎
+Gospel                  [  1]  ▎
+Ragga                   [  1]  ▎
+Indie                   [  1]  ▎
+Speed Metal             [  1]  ▎
+Gypsy Jazz              [  1]  ▎
+```
+
+## Configuration
+
+There are no configuration options for this plugin.
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

### Comparing `beets-describe-0.0.4/beets_describe.egg-info/PKG-INFO` & `beets_describe-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,220 @@
 Metadata-Version: 2.1
 Name: beets-describe
-Version: 0.0.4
+Version: 0.0.5
 Summary: ('A beets plugin that describes attributes in depth',)
 Home-page: https://github.com/adamjakab/BeetsPluginDescribe
 Author: Adam Jakab
 Author-email: adam@jakab.pro
 License: MIT
-Description: [![Build Status](https://travis-ci.org/adamjakab/BeetsPluginDescribe.svg?branch=master)](https://travis-ci.org/adamjakab/BeetsPluginDescribe)
-        [![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginDescribe/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginDescribe?branch=master)
-        [![PyPi](https://img.shields.io/pypi/v/beets-describe.svg)](https://pypi.org/project/beets-describe/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-describe.svg)](https://pypi.org/project/beets-describe/)
-        [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
-        
-        
-        # Describe (Beets Plugin)
-        
-        The *beets-describe* plugin attempts to give you the full picture on a single attribute of your library item.
-        
-        **NOTE: Under heavy development but works!**
-        
-        
-        ## Installation:
-        
-        ```shell script
-        $ pip install beets-describe
-        ```
-        
-        and activate the plugin the usual way
-        ```yaml
-        plugins:
-            - describe
-        ```
-        
-        ## Usage:
-        
-        ```bash
-        beet describe field_name
-        ```
-        
-        You can of course add any queries after the name of the field to describe such as:
-        
-        ```bash
-        beet describe genre albumartist:'Various Artists'
-        ```
-        
-        ## Sample Output
-        
-        `beet describe bpm`
-        
-        ```text
-        ┌────────────────┬────────────────────────────┐
-        │ Name           │                      Value │
-        ╞════════════════╪════════════════════════════╡
-        │ Field name     │                        bpm │
-        ├────────────────┼────────────────────────────┤
-        │ Field type     │ beets.dbcore.types.Integer │
-        ├────────────────┼────────────────────────────┤
-        │ Count          │                       1392 │
-        ├────────────────┼────────────────────────────┤
-        │ Min            │              65.9922409058 │
-        ├────────────────┼────────────────────────────┤
-        │ Max            │                      185.0 │
-        ├────────────────┼────────────────────────────┤
-        │ Mean           │         122.99097545119291 │
-        ├────────────────┼────────────────────────────┤
-        │ Median         │                      122.0 │
-        ├────────────────┼────────────────────────────┤
-        │ Empty          │                          0 │
-        ├────────────────┼────────────────────────────┤
-        │ Unique         │                        649 │
-        ├────────────────┼────────────────────────────┤
-        │ Most frequent  │                  122.0(22) │
-        ├────────────────┼────────────────────────────┤
-        │ Least frequent │           117.853546143(1) │
-        └────────────────┴────────────────────────────┘
-        Distribution(bins=10) histogram
-        66.0 - 77.9    [ 30]  ████▊
-        77.9 - 89.8    [ 73]  ███████████▍
-        89.8 - 101.7   [203]  ███████████████████████████████▊
-        101.7 - 113.6  [221]  ██████████████████████████████████▌
-        113.6 - 125.5  [256]  ████████████████████████████████████████
-        125.5 - 137.4  [208]  ████████████████████████████████▌
-        137.4 - 149.3  [183]  ████████████████████████████▋
-        149.3 - 161.2  [ 87]  █████████████▋
-        161.2 - 173.1  [107]  ████████████████▊
-        173.1 - 185.0  [ 24]  ███▊
-        ```
-        
-        
-        `beet describe genre`
-        
-        ```text
-        ┌────────────────┬───────────────────────────┐
-        │ Name           │                     Value │
-        ╞════════════════╪═══════════════════════════╡
-        │ Field name     │                     genre │
-        ├────────────────┼───────────────────────────┤
-        │ Field type     │ beets.dbcore.types.String │
-        ├────────────────┼───────────────────────────┤
-        │ Count          │                      1392 │
-        ├────────────────┼───────────────────────────┤
-        │ Empty          │                        19 │
-        ├────────────────┼───────────────────────────┤
-        │ Unique         │                        91 │
-        ├────────────────┼───────────────────────────┤
-        │ Most frequent  │               Oldies(202) │
-        ├────────────────┼───────────────────────────┤
-        │ Least frequent │              Post-Punk(1) │
-        └────────────────┴───────────────────────────┘
-        Unique element histogram
-        Oldies                  [202]  ████████████████████████████████████████
-        Classic Rock            [139]  ███████████████████████████▌
-        Soul                    [124]  ████████████████████████▌
-        Blues                   [120]  ███████████████████████▊
-        Rock                    [109]  █████████████████████▋
-        Pop                     [105]  ████████████████████▊
-        Dance                   [ 86]  █████████████████
-        New Wave                [ 48]  █████████▌
-        Reggae                  [ 44]  ████████▊
-        Heavy Metal             [ 33]  ██████▌
-        Trance                  [ 24]  ████▊
-        Blues Rock              [ 20]  ████
-        Jazz                    [ 20]  ████
-                                [ 19]  ███▊
-        Soundtrack              [ 17]  ███▍
-        Ska                     [ 16]  ███▏
-        Synthpop                [ 16]  ███▏
-        Rap                     [ 15]  ███
-        Pop Rock                [ 14]  ██▊
-        Funk                    [ 12]  ██▍
-        Metal                   [ 12]  ██▍
-        Alternative Metal       [ 12]  ██▍
-        Alternative Rock        [ 11]  ██▏
-        Soft Rock               [ 10]  ██
-        Hard Rock               [ 10]  ██
-        Singer-Songwriter       [  9]  █▊
-        Rockabilly              [  8]  █▋
-        Metalcore               [  6]  █▎
-        Electronic              [  6]  █▎
-        Rock And Roll           [  6]  █▎
-        R&B                     [  6]  █▎
-        House                   [  5]  █
-        Disco                   [  5]  █
-        Progressive Rock        [  5]  █
-        Psychedelic Rock        [  5]  █
-        Punk Rock               [  4]  ▊
-        Thrash Metal            [  4]  ▊
-        Progressive Metal       [  4]  ▊
-        Contemporary R&B        [  3]  ▋
-        Nu Metal                [  3]  ▋
-        Symphonic Metal         [  3]  ▋
-        Funk Soul               [  3]  ▋
-        World Music             [  3]  ▋
-        Death Metal             [  3]  ▋
-        Britpop                 [  2]  ▍
-        Industrial Metal        [  2]  ▍
-        Contemporary Classical  [  2]  ▍
-        Post-Grunge             [  2]  ▍
-        Psychedelic             [  2]  ▍
-        Motown                  [  2]  ▍
-        Glam Rock               [  2]  ▍
-        Rock, Hard Rock, Metal  [  2]  ▍
-        Blue-Eyed Soul          [  2]  ▍
-        Black Metal             [  2]  ▍
-        Indie Rock              [  2]  ▍
-        Indie Pop               [  2]  ▍
-        Industrial              [  2]  ▍
-        Pop Punk                [  2]  ▍
-        Surf Rock               [  2]  ▍
-        Hip Hop                 [  1]  ▎
-        Gospel                  [  1]  ▎
-        Ragga                   [  1]  ▎
-        Indie                   [  1]  ▎
-        Speed Metal             [  1]  ▎
-        Gypsy Jazz              [  1]  ▎
-        ```
-        
-        
-        ## Configuration
-        There are no configuration options for this plugin.
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
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: termtables
+Requires-Dist: termplotlib
 Provides-Extra: tests
+
+[![Test & Release & Deploy](https://github.com/adamjakab/BeetsPluginDescribe/actions/workflows/test_release_deploy.yml/badge.svg)](https://github.com/adamjakab/BeetsPluginDescribe/actions/workflows/test_release_deploy.yml)
+[![Coverage Status](https://coveralls.io/repos/github/adamjakab/BeetsPluginDescribe/badge.svg?branch=master)](https://coveralls.io/github/adamjakab/BeetsPluginDescribe?branch=master)
+[![PyPi](https://img.shields.io/pypi/v/beets-describe.svg)](https://pypi.org/project/beets-describe/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/beets-describe.svg)](https://pypi.org/project/beets-describe/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE.txt)
+
+# Describe (Beets Plugin)
+
+The _beets-describe_ plugin attempts to give you the full picture on a single attribute of your library item.
+
+**NOTE: Under heavy development but works!**
+
+## Installation:
+
+```shell script
+$ pip install beets-describe
+```
+
+and activate the plugin the usual way
+
+```yaml
+plugins:
+  - describe
+```
+
+## Usage:
+
+```bash
+beet describe field_name
+```
+
+You can of course add any queries after the name of the field to describe such as:
+
+```bash
+beet describe genre albumartist:'Various Artists'
+```
+
+## Sample Output
+
+`beet describe bpm`
+
+```text
+┌────────────────┬────────────────────────────┐
+│ Name           │                      Value │
+╞════════════════╪════════════════════════════╡
+│ Field name     │                        bpm │
+├────────────────┼────────────────────────────┤
+│ Field type     │ beets.dbcore.types.Integer │
+├────────────────┼────────────────────────────┤
+│ Count          │                       1392 │
+├────────────────┼────────────────────────────┤
+│ Min            │              65.9922409058 │
+├────────────────┼────────────────────────────┤
+│ Max            │                      185.0 │
+├────────────────┼────────────────────────────┤
+│ Mean           │         122.99097545119291 │
+├────────────────┼────────────────────────────┤
+│ Median         │                      122.0 │
+├────────────────┼────────────────────────────┤
+│ Empty          │                          0 │
+├────────────────┼────────────────────────────┤
+│ Unique         │                        649 │
+├────────────────┼────────────────────────────┤
+│ Most frequent  │                  122.0(22) │
+├────────────────┼────────────────────────────┤
+│ Least frequent │           117.853546143(1) │
+└────────────────┴────────────────────────────┘
+Distribution(bins=10) histogram
+66.0 - 77.9    [ 30]  ████▊
+77.9 - 89.8    [ 73]  ███████████▍
+89.8 - 101.7   [203]  ███████████████████████████████▊
+101.7 - 113.6  [221]  ██████████████████████████████████▌
+113.6 - 125.5  [256]  ████████████████████████████████████████
+125.5 - 137.4  [208]  ████████████████████████████████▌
+137.4 - 149.3  [183]  ████████████████████████████▋
+149.3 - 161.2  [ 87]  █████████████▋
+161.2 - 173.1  [107]  ████████████████▊
+173.1 - 185.0  [ 24]  ███▊
+```
+
+`beet describe genre`
+
+```text
+┌────────────────┬───────────────────────────┐
+│ Name           │                     Value │
+╞════════════════╪═══════════════════════════╡
+│ Field name     │                     genre │
+├────────────────┼───────────────────────────┤
+│ Field type     │ beets.dbcore.types.String │
+├────────────────┼───────────────────────────┤
+│ Count          │                      1392 │
+├────────────────┼───────────────────────────┤
+│ Empty          │                        19 │
+├────────────────┼───────────────────────────┤
+│ Unique         │                        91 │
+├────────────────┼───────────────────────────┤
+│ Most frequent  │               Oldies(202) │
+├────────────────┼───────────────────────────┤
+│ Least frequent │              Post-Punk(1) │
+└────────────────┴───────────────────────────┘
+Unique element histogram
+Oldies                  [202]  ████████████████████████████████████████
+Classic Rock            [139]  ███████████████████████████▌
+Soul                    [124]  ████████████████████████▌
+Blues                   [120]  ███████████████████████▊
+Rock                    [109]  █████████████████████▋
+Pop                     [105]  ████████████████████▊
+Dance                   [ 86]  █████████████████
+New Wave                [ 48]  █████████▌
+Reggae                  [ 44]  ████████▊
+Heavy Metal             [ 33]  ██████▌
+Trance                  [ 24]  ████▊
+Blues Rock              [ 20]  ████
+Jazz                    [ 20]  ████
+                        [ 19]  ███▊
+Soundtrack              [ 17]  ███▍
+Ska                     [ 16]  ███▏
+Synthpop                [ 16]  ███▏
+Rap                     [ 15]  ███
+Pop Rock                [ 14]  ██▊
+Funk                    [ 12]  ██▍
+Metal                   [ 12]  ██▍
+Alternative Metal       [ 12]  ██▍
+Alternative Rock        [ 11]  ██▏
+Soft Rock               [ 10]  ██
+Hard Rock               [ 10]  ██
+Singer-Songwriter       [  9]  █▊
+Rockabilly              [  8]  █▋
+Metalcore               [  6]  █▎
+Electronic              [  6]  █▎
+Rock And Roll           [  6]  █▎
+R&B                     [  6]  █▎
+House                   [  5]  █
+Disco                   [  5]  █
+Progressive Rock        [  5]  █
+Psychedelic Rock        [  5]  █
+Punk Rock               [  4]  ▊
+Thrash Metal            [  4]  ▊
+Progressive Metal       [  4]  ▊
+Contemporary R&B        [  3]  ▋
+Nu Metal                [  3]  ▋
+Symphonic Metal         [  3]  ▋
+Funk Soul               [  3]  ▋
+World Music             [  3]  ▋
+Death Metal             [  3]  ▋
+Britpop                 [  2]  ▍
+Industrial Metal        [  2]  ▍
+Contemporary Classical  [  2]  ▍
+Post-Grunge             [  2]  ▍
+Psychedelic             [  2]  ▍
+Motown                  [  2]  ▍
+Glam Rock               [  2]  ▍
+Rock, Hard Rock, Metal  [  2]  ▍
+Blue-Eyed Soul          [  2]  ▍
+Black Metal             [  2]  ▍
+Indie Rock              [  2]  ▍
+Indie Pop               [  2]  ▍
+Industrial              [  2]  ▍
+Pop Punk                [  2]  ▍
+Surf Rock               [  2]  ▍
+Hip Hop                 [  1]  ▎
+Gospel                  [  1]  ▎
+Ragga                   [  1]  ▎
+Indie                   [  1]  ▎
+Speed Metal             [  1]  ▎
+Gypsy Jazz              [  1]  ▎
+```
+
+## Configuration
+
+There are no configuration options for this plugin.
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

### Comparing `beets-describe-0.0.4/beetsplug/describe/__init__.py` & `beets_describe-0.0.5/beetsplug/describe/__init__.py`

 * *Files identical despite different names*

### Comparing `beets-describe-0.0.4/beetsplug/describe/about.py` & `beets_describe-0.0.5/beetsplug/describe/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  Author: Adam Jakab <adam at jakab dot pro>
 #  License: See LICENSE.txt
 
 __author__ = u'Adam Jakab'
 __email__ = u'adam@jakab.pro'
 __copyright__ = u'Copyright (c) 2020, {} <{}>'.format(__author__, __email__)
 __license__ = u'License :: OSI Approved :: MIT License'
-__version__ = u'0.0.4'
+__version__ = u'0.0.5'
 __status__ = u'Kickstarted'
 
 __PACKAGE_TITLE__ = u'Describe'
 __PACKAGE_NAME__ = u'beets-describe'
 __PACKAGE_DESCRIPTION__ = u'A beets plugin that describes attributes in depth',
 __PACKAGE_URL__ = u'https://github.com/adamjakab/BeetsPluginDescribe'
 __PLUGIN_NAME__ = u'describe'
```

### Comparing `beets-describe-0.0.4/beetsplug/describe/command.py` & `beets_describe-0.0.5/beetsplug/describe/command.py`

 * *Files identical despite different names*

### Comparing `beets-describe-0.0.4/beetsplug/describe/common.py` & `beets_describe-0.0.5/beetsplug/describe/common.py`

 * *Files identical despite different names*

### Comparing `beets-describe-0.0.4/setup.py` & `beets_describe-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,37 +32,39 @@
     long_description_content_type='text/markdown',
     platforms='ALL',
 
     include_package_data=True,
     test_suite='test',
     packages=['beetsplug.describe'],
 
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 
     install_requires=[
         'beets>=1.4.9',
         'numpy',
         'pandas',
         'termtables',
         'termplotlib',
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

