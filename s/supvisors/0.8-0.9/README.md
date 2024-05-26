# Comparing `tmp/supvisors-0.8.tar.gz` & `tmp/supvisors-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/supvisors-0.8.tar", last modified: Sun Aug 22 18:54:59 2021, max compression
+gzip compressed data, was "dist/supvisors-0.9.tar", last modified: Tue Aug 31 20:41:44 2021, max compression
```

## Comparing `supvisors-0.8.tar` & `supvisors-0.9.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/client/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)        0 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/client/__init__.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     6720 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/client/subscriber.py
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/tests/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       56 2021-03-02 00:03:51.000000 supvisors-0.8/supvisors/tests/__init__.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11713 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/base.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    12534 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/configurations.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2010 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/conftest.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     6869 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_address.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4809 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_addressmapper.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    17916 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_application.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    58291 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_commander.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    37483 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_context.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     8893 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_infosource.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     5113 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_initializer.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    12129 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_listener.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    15786 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/test_mainloop.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    10672 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/test_options.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2057 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_plot.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3697 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_plugin.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    36176 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_process.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    45569 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_rpcinterface.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2383 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_rpcrequests.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    18029 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_sparser.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    37739 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_statemachine.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4193 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_statscollector.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    17005 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_statscompiler.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    37540 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/test_strategy.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    25943 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_supvisorsctl.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    25533 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_supvisorszmq.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3070 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_ttypes.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4378 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_utils.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    26020 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/test_viewapplication.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    22503 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_viewcontext.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    45812 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_viewhandler.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    18241 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_viewhostaddress.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3795 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_viewimage.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    20180 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_viewprocaddress.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     7791 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/tests/test_viewsupstatus.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    33363 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tests/test_viewsupvisors.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     5213 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/tests/test_webutils.py
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/tools/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)        0 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tools/__init__.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     7612 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/tools/breed.py
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/ui/
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/ui/css/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      795 2021-08-18 09:52:16.000000 supvisors-0.8/supvisors/ui/css/button.css
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      832 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/css/main_page.css
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      957 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/css/menu.css
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11331 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/css/ui_style.css
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/ui/fonts/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    19886 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.eot
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    62308 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.svg
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    40276 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.ttf
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    23284 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.woff
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors/ui/img/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      465 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/arrow-orange_12.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2104 2021-02-14 23:48:28.000000 supvisors-0.8/supvisors/ui/img/auto_reload_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     1043 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/erro_20.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     1159 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/info_20.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2762 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/ui/img/leds_empty_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2963 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/ui/img/leds_green_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2986 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/ui/img/leds_red_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3012 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/ui/img/leds_yellow_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     5013 2021-08-15 17:42:37.000000 supvisors-0.8/supvisors/ui/img/red_light_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2237 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/reload_30.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3823 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/restart_40.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3889 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/shutdown_40.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3537 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/start_40.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3158 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/stop_40.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      983 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/ui/img/warn_20.png
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     9368 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/application.html
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     8548 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/hostaddress.html
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     6730 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/index.html
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     8950 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ui/procaddress.html
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       56 2021-02-21 16:40:32.000000 supvisors-0.8/supvisors/__init__.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     6770 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/address.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4907 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/addressmapper.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    17576 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/application.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    41536 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/commander.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    19487 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/context.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     7848 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/infosource.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4756 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/initializer.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11251 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/listener.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    10162 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/mainloop.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11485 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/options.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4007 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/plot.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3973 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/plugin.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    27121 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/process.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    34124 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/rpcinterface.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     1901 2021-08-15 17:42:36.000000 supvisors-0.8/supvisors/rpcrequests.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4146 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/rules.xsd
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    21459 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/sparser.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    28042 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/statemachine.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3268 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/statscollector.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     8990 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/statscompiler.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    33890 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/strategy.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    40662 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/supvisorsctl.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    21965 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/supvisorszmq.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     2627 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/ttypes.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4623 2021-08-15 17:42:37.000000 supvisors-0.8/supvisors/utils.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       12 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/version.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    13646 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/viewapplication.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    12295 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/viewcontext.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    21471 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/viewhandler.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     8694 2021-08-20 11:50:18.000000 supvisors-0.8/supvisors/viewhostaddress.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3275 2020-12-14 12:06:35.000000 supvisors-0.8/supvisors/viewimage.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11135 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/viewprocaddress.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4413 2021-08-15 17:42:37.000000 supvisors-0.8/supvisors/viewsupstatus.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    15655 2021-08-22 17:26:30.000000 supvisors-0.8/supvisors/viewsupvisors.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4030 2021-07-31 22:46:35.000000 supvisors-0.8/supvisors/webutils.py
-drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-22 18:54:59.000000 supvisors-0.8/supvisors.egg-info/
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    18937 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/PKG-INFO
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3474 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/SOURCES.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)        1 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/dependency_links.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       10 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/namespace_packages.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)        1 2021-08-15 18:25:14.000000 supvisors-0.8/supvisors.egg-info/not-zip-safe
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      232 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/requires.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       10 2021-08-22 18:54:58.000000 supvisors-0.8/supvisors.egg-info/top_level.txt
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    11357 2016-06-02 22:38:39.000000 supvisors-0.8/LICENSE
--rw-rw-r--   0 cliche    (1000) cliche    (1000)      153 2021-08-22 17:26:29.000000 supvisors-0.8/MANIFEST.in
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     4420 2021-08-22 17:26:29.000000 supvisors-0.8/README.md
--rw-rw-r--   0 cliche    (1000) cliche    (1000)       79 2021-08-22 18:54:59.000000 supvisors-0.8/setup.cfg
--rw-rw-r--   0 cliche    (1000) cliche    (1000)     3148 2021-08-22 17:26:30.000000 supvisors-0.8/setup.py
--rw-rw-r--   0 cliche    (1000) cliche    (1000)    18937 2021-08-22 18:54:59.000000 supvisors-0.8/PKG-INFO
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/client/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)        0 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/client/__init__.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     6720 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/client/subscriber.py
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/tests/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       56 2021-03-02 00:03:51.000000 supvisors-0.9/supvisors/tests/__init__.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11831 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/base.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11735 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/configurations.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2019 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/conftest.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     6869 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_address.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4809 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_addressmapper.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    20966 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_application.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    10704 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_breed.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    58493 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_commander.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    37483 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_context.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8893 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_infosource.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3670 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_initializer.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    12129 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_listener.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    15786 2021-08-15 17:42:36.000000 supvisors-0.9/supvisors/tests/test_mainloop.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    10441 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_options.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2057 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_plot.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3697 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_plugin.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    36903 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_process.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    45571 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_rpcinterface.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2383 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_rpcrequests.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    18193 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_sparser.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    37739 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_statemachine.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4193 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_statscollector.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    17005 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_statscompiler.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    37540 2021-08-15 17:42:36.000000 supvisors-0.9/supvisors/tests/test_strategy.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    27120 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_supvisorsctl.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    25533 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_supvisorszmq.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3070 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_ttypes.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4378 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_utils.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    26144 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_viewapplication.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    22745 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_viewcontext.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    46474 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tests/test_viewhandler.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    18241 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_viewhostaddress.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3795 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_viewimage.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    20180 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_viewprocaddress.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     7791 2021-08-15 17:42:36.000000 supvisors-0.9/supvisors/tests/test_viewsupstatus.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    33363 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tests/test_viewsupvisors.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     5213 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/tests/test_webutils.py
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/tools/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)        0 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/tools/__init__.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8849 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/tools/breed.py
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/ui/
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/ui/css/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      795 2021-08-18 09:52:16.000000 supvisors-0.9/supvisors/ui/css/button.css
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      832 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/css/main_page.css
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      957 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/css/menu.css
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11331 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/ui/css/ui_style.css
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/ui/fonts/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    19886 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.eot
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    62308 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.svg
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    40276 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.ttf
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    23284 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.woff
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors/ui/img/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      465 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/arrow-orange_12.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2104 2021-02-14 23:48:28.000000 supvisors-0.9/supvisors/ui/img/auto_reload_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     1043 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/erro_20.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     1159 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/info_20.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2762 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/ui/img/leds_empty_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2963 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/ui/img/leds_green_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2986 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/ui/img/leds_red_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3012 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/ui/img/leds_yellow_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     5013 2021-08-15 17:42:37.000000 supvisors-0.9/supvisors/ui/img/red_light_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2237 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/reload_30.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3823 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/restart_40.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3889 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/shutdown_40.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3537 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/start_40.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3158 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/stop_40.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      983 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/ui/img/warn_20.png
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     9368 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/application.html
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8548 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/hostaddress.html
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     6730 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/index.html
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8950 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ui/procaddress.html
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       56 2021-02-21 16:40:32.000000 supvisors-0.9/supvisors/__init__.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     6770 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/address.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4907 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/addressmapper.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    21391 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/application.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    41996 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/commander.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    19501 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/context.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     7848 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/infosource.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4719 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/initializer.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11251 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/listener.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    10162 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/mainloop.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     9919 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/options.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4007 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/plot.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3983 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/plugin.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    27938 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/process.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    34124 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/rpcinterface.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     1901 2021-08-15 17:42:36.000000 supvisors-0.9/supvisors/rpcrequests.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4047 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/rules.xsd
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    20569 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/sparser.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    28042 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/statemachine.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3268 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/statscollector.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8990 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/statscompiler.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    33890 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/strategy.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    41533 2021-08-31 20:40:18.000000 supvisors-0.9/supvisors/supvisorsctl.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    21965 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/supvisorszmq.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     2627 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/ttypes.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4623 2021-08-15 17:42:37.000000 supvisors-0.9/supvisors/utils.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       12 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/version.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    15377 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/viewapplication.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    12630 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/viewcontext.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    21652 2021-08-31 20:40:19.000000 supvisors-0.9/supvisors/viewhandler.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     8694 2021-08-20 11:50:18.000000 supvisors-0.9/supvisors/viewhostaddress.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3275 2020-12-14 12:06:35.000000 supvisors-0.9/supvisors/viewimage.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11135 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/viewprocaddress.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4413 2021-08-15 17:42:37.000000 supvisors-0.9/supvisors/viewsupstatus.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    15655 2021-08-22 17:26:30.000000 supvisors-0.9/supvisors/viewsupvisors.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4030 2021-07-31 22:46:35.000000 supvisors-0.9/supvisors/webutils.py
+drwxrwxr-x   0 cliche    (1000) cliche    (1000)        0 2021-08-31 20:41:44.000000 supvisors-0.9/supvisors.egg-info/
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    20342 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/PKG-INFO
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3540 2021-08-31 20:41:43.000000 supvisors-0.9/supvisors.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)        1 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      107 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/entry_points.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       10 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)        1 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/not-zip-safe
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      232 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/requires.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       10 2021-08-31 20:41:42.000000 supvisors-0.9/supvisors.egg-info/top_level.txt
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    11357 2016-06-02 22:38:39.000000 supvisors-0.9/LICENSE
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)      153 2021-08-22 17:26:29.000000 supvisors-0.9/MANIFEST.in
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     4420 2021-08-22 17:26:29.000000 supvisors-0.9/README.md
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)       79 2021-08-31 20:41:44.000000 supvisors-0.9/setup.cfg
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)     3318 2021-08-31 20:40:18.000000 supvisors-0.9/setup.py
+-rw-rw-r--   0 cliche    (1000) cliche    (1000)    20342 2021-08-31 20:41:44.000000 supvisors-0.9/PKG-INFO
```

### Comparing `supvisors-0.8/supvisors/client/subscriber.py` & `supvisors-0.9/supvisors/client/subscriber.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/base.py` & `supvisors-0.9/supvisors/tests/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 import os
 import random
 
 from socket import gethostname
 from unittest.mock import Mock
 
 from supervisor.datatypes import Automatic
-from supervisor.loggers import LevelsByName, Logger
+from supervisor.loggers import getLogger, handle_stdout, LevelsByName, Logger
 from supervisor.rpcinterface import SupervisorNamespaceRPCInterface
 from supervisor.states import STOPPED_STATES
 
 from supvisors.addressmapper import AddressMapper
 from supvisors.context import Context
 from supvisors.infosource import SupervisordSource
+from supvisors.initializer import Supvisors
 from supvisors.ttypes import StartingStrategies
 from supvisors.utils import extract_process_info
 
 
 class DummyOptions:
     """ Simple options with dummy attributes. """
 
@@ -135,15 +136,16 @@
                                 'port': 1234,
                                 'username': 'user',
                                 'password': 'p@$$w0rd'}]
         self.serverurl = 'url'
         self.mood = 'mood'
         self.nodaemon = True
         self.silent = False
-        self.logger = Mock(handlers=[Mock()])
+        self.logger = getLogger()
+        handle_stdout(self.logger, Supvisors.LOGGER_FORMAT)
         # build a fake http config
         self.httpservers = [[None, DummyHttpServer()]]
         self.httpserver = self.httpservers[0][1]
         # prepare storage for close_httpservers test
         self.storage = None
 
     def close_httpservers(self):
```

### Comparing `supvisors-0.8/supvisors/tests/configurations.py` & `supvisors-0.9/supvisors/tests/configurations.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 # Contents of a minimal Supervisor configuration file including program definitions
 ProgramConfiguration = StringIO('''
 [inet_http_server]
 port=:60000
 
 [supervisord]
-[supvisors]
 
 [program:dummy]
 command=ls
 
 [program:dummies]
 command=ls
 process_name=dummy_%(process_num)d
@@ -47,51 +46,14 @@
 [program:dumber]
 command=ls
 process_name=dumber_%(process_num)d
 numprocs=2
 numprocs_start=10
 ''')
 
-# Contents of a minimal Supervisor configuration file without
-#  Supvisors options defined
-DefaultOptionConfiguration = StringIO('''
-[inet_http_server]
-port=:60000
-
-[supervisord]
-[supvisors]
-''')
-
-# Contents of a minimal Supervisor configuration file including
-#  Supvisors options defined
-DefinedOptionConfiguration = StringIO('''
-[inet_http_server]
-port=:60000
-
-[supervisord]
-
-[supvisors]
-address_list=cliche01,cliche03,cliche02
-rules_file=my_movies.xml
-auto_fence=true
-internal_port=60001
-event_port=60002
-synchro_timeout=20
-force_synchro_if=cliche01,cliche03
-starting_strategy=MOST_LOADED
-conciliation_strategy=SENICIDE
-stats_periods=5,60,600
-stats_histo=100
-stats_irix_mode=true
-logfile=/tmp/supvisors.log
-logfile_maxbytes=50KB
-logfile_backups=5
-loglevel=error
-''')
-
 # Contents of a rules file including schema errors
 InvalidXmlTest = b'''\
 <?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <root>
     <alias name="not used">nodes_prg_B3, nodes_appli_D</alias>
     <alias name="not used too">#, 10.0.0.1, 192.168.12.20</alias>
     <alias name="nodes_prg_B1">#</alias>
@@ -291,16 +253,15 @@
         <distributed>false</distributed>
         <start_sequence>1</start_sequence>
         <stop_sequence>4</stop_sequence>
         <starting_strategy>CONFIG</starting_strategy>
         <starting_failure_strategy>STOP</starting_failure_strategy>
         <running_failure_strategy>RESTART_PROCESS</running_failure_strategy>
 
-        <program name="dummy_program_B0">
-        </program>
+        <program name="dummy_program_B0"/>
 
         <program name="dummy_program_B1">
             <addresses>#</addresses>
             <start_sequence>3</start_sequence>
             <stop_sequence>50</stop_sequence>
             <required>true</required>
             <wait_exit>false</wait_exit>
@@ -359,18 +320,18 @@
         <addresses>nodes_appli_D</addresses>
         <start_sequence>-1</start_sequence>
         <stop_sequence>100</stop_sequence>
         <starting_strategy>LESS_LOADED</starting_strategy>
         <starting_failure_strategy>CONTINUE</starting_failure_strategy>
         <running_failure_strategy>RESTART_APPLICATION</running_failure_strategy>
 
-        <pattern name="dummies_">
+        <program pattern="dummies_">
             <reference>dummy_model_03</reference>
             <start_sequence>50</start_sequence>
-        </pattern>
+        </program>
 
         <program pattern="dummies_01_">
             <addresses>#, 10.0.0.1, 10.0.0.5</addresses>
             <start_sequence>1</start_sequence>
             <stop_sequence>1</stop_sequence>
             <required>false</required>
             <wait_exit>true</wait_exit>
```

### Comparing `supvisors-0.8/supvisors/tests/conftest.py` & `supvisors-0.9/supvisors/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def create_any_process(supvisors):
     return create_process(any_process_info(), supvisors)
 
 
 def create_application(application_name, supvisors):
     """ Create an ApplicationStatus. """
-    return ApplicationStatus(application_name, ApplicationRules(), supvisors)
+    return ApplicationStatus(application_name, ApplicationRules(supvisors), supvisors)
 
 
 # fixture for common global structures
 @pytest.fixture
 def supervisor():
     return DummySupervisor()
```

### Comparing `supvisors-0.8/supvisors/tests/test_address.py` & `supvisors-0.9/supvisors/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_addressmapper.py` & `supvisors-0.9/supvisors/tests/test_addressmapper.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_application.py` & `supvisors-0.9/supvisors/tests/test_application.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,60 +16,136 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ======================================================================
 
 import pytest
 import random
 
+from unittest.mock import call
+
 from supvisors.application import *
 
 from .base import database_copy, any_process_info, any_stopped_process_info, any_process_info_by_state
 from .conftest import create_application, create_process
 
 
 # ApplicationRules part
 @pytest.fixture
-def rules():
+def rules(supvisors):
     """ Return the instance to test. """
-    return ApplicationRules()
+    return ApplicationRules(supvisors)
 
 
 def test_rules_create(rules):
     """ Test the values set at construction. """
     # check application default rules
     assert not rules.managed
     assert rules.distributed
     assert rules.node_names == ['*']
+    assert rules.hash_node_names == []
     assert rules.start_sequence == 0
-    assert rules.stop_sequence == 0
+    assert rules.stop_sequence == -1
     assert rules.starting_strategy == StartingStrategies.CONFIG
     assert rules.starting_failure_strategy == StartingFailureStrategies.ABORT
     assert rules.running_failure_strategy == RunningFailureStrategies.CONTINUE
 
 
+def test_rules_check_stop_sequence(rules):
+    """ Test the assignment of stop sequence to start sequence if default still set. """
+    # test when default still used
+    assert rules.start_sequence == 0
+    assert rules.stop_sequence == -1
+    rules.check_stop_sequence('crash')
+    assert rules.start_sequence == 0
+    assert rules.stop_sequence == 0
+    # test when value has been set
+    rules.start_sequence = 12
+    rules.stop_sequence = 50
+    rules.check_stop_sequence('crash')
+    assert rules.start_sequence == 12
+    assert rules.stop_sequence == 50
+
+
+def test_rules_check_hash_nodes(rules):
+    """ Test the resolution of nodes when hash_node_names is set. """
+    # set initial attributes
+    rules.hash_node_names = ['*']
+    rules.node_names = []
+    rules.start_sequence = 1
+    # 1. test with application without ending index
+    rules.check_hash_nodes('crash')
+    # node_names is unchanged and start_sequence is invalidated
+    assert rules.hash_node_names == ['*']
+    assert rules.node_names == []
+    assert rules.start_sequence == 0
+    # 2. test with application with 0-ending index
+    rules.start_sequence = 1
+    rules.check_hash_nodes('sample_test_0')
+    # node_names is unchanged and start_sequence is invalidated
+    assert rules.hash_node_names == ['*']
+    assert rules.node_names == []
+    assert rules.start_sequence == 0
+    # 3. update rules to test '#' with all nodes available
+    # address '127.0.0.1' has an index of 1-1 in address_mapper
+    rules.start_sequence = 1
+    rules.check_hash_nodes('sample_test_1')
+    assert rules.node_names == ['127.0.0.1']
+    assert rules.start_sequence == 1
+    # 4. update rules to test '#' with a subset of nodes available
+    rules.hash_node_names = ['10.0.0.0', '10.0.0.3', '10.0.0.5']
+    rules.node_names = []
+    # here, at index 2-1 of this list, '10.0.0.5' can be found
+    rules.check_hash_nodes('sample_test_2')
+    assert rules.node_names == ['10.0.0.3']
+    assert rules.start_sequence == 1
+    # 5. test the case where procnumber is greater than the subset list of nodes available
+    rules.hash_node_names = ['10.0.0.1']
+    rules.node_names = []
+    rules.check_hash_nodes('sample_test_2')
+    assert rules.node_names == []
+    assert rules.start_sequence == 0
+
+
+def test_rules_check_dependencies(mocker, rules):
+    """ Test the dependencies in process rules. """
+    mocked_stop = mocker.patch('supvisors.application.ApplicationRules.check_stop_sequence')
+    mocked_hash = mocker.patch('supvisors.application.ApplicationRules.check_hash_nodes')
+    # test with no hash
+    rules.hash_node_names = []
+    rules.check_dependencies('dummy')
+    assert mocked_stop.call_args_list == [call('dummy')]
+    assert not mocked_hash.called
+    mocker.resetall()
+    # test with hash
+    rules.hash_node_names = ['*']
+    rules.check_dependencies('dummy')
+    assert mocked_stop.call_args_list == [call('dummy')]
+    assert mocked_hash.call_args_list == [call('dummy')]
+
+
 def test_rules_str(rules):
     """ Test the string output. """
-    assert str(rules) == "managed=False distributed=True node_names=['*'] start_sequence=0 stop_sequence=0"\
+    assert str(rules) == "managed=False distributed=True node_names=['*'] start_sequence=0 stop_sequence=-1"\
                          " starting_strategy=CONFIG starting_failure_strategy=ABORT running_failure_strategy=CONTINUE"
 
 
 def test_rules_serial(rules):
     """ Test the serialization of the ApplicationRules object. """
     # default is not managed so result is short
     assert rules.serial() == {'managed': False}
     # check managed and distributed
     rules.managed = True
     assert rules.serial() == {'managed': True, 'distributed': True,
-                              'start_sequence': 0, 'stop_sequence': 0,
+                              'start_sequence': 0, 'stop_sequence': -1,
                               'starting_strategy': 'CONFIG', 'starting_failure_strategy': 'ABORT',
                               'running_failure_strategy': 'CONTINUE'}
     # finally check managed and not distributed
     rules.distributed = False
     assert rules.serial() == {'managed': True, 'distributed': False, 'addresses': ['*'],
-                              'start_sequence': 0, 'stop_sequence': 0,
+                              'start_sequence': 0, 'stop_sequence': -1,
                               'starting_strategy': 'CONFIG', 'starting_failure_strategy': 'ABORT',
                               'running_failure_strategy': 'CONTINUE'}
 
 
 # ApplicationStatus part
 def test_application_create(supvisors):
     """ Test the values set at construction. """
@@ -82,15 +158,15 @@
     assert not application.processes
     assert not application.start_sequence
     assert not application.stop_sequence
     # check application default rules
     assert not application.rules.managed
     assert application.rules.distributed
     assert application.rules.start_sequence == 0
-    assert application.rules.stop_sequence == 0
+    assert application.rules.stop_sequence == -1
     assert application.rules.starting_failure_strategy == StartingFailureStrategies.ABORT
     assert application.rules.running_failure_strategy == RunningFailureStrategies.CONTINUE
 
 
 def test_application_running(supvisors):
     """ Test the running method. """
     application = create_application('ApplicationTest', supvisors)
```

### Comparing `supvisors-0.8/supvisors/tests/test_commander.py` & `supvisors-0.9/supvisors/tests/test_commander.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,15 @@
     assert printable == {0: {'if': {-1: [], 0: ['appli_A:dummy_A1', 'appli_A:dummy_A2', 'appli_A:dummy_A3']},
                              'then': {2: ['appli_B:dummy_B1']}},
                          3: {'else': {}}}
 
 
 def test_commander_process_application_jobs(mocker, commander, command_list_1, command_list_2):
     """ Test the Commander.process_application_jobs method. """
+    commander.pickup_logic = min
     # fill planned_jobs
     commander.planned_jobs = {'if': {0: command_list_1, 1: []}, 'then': {2: command_list_2}, 'else': {}}
 
     # define patch function
     def fill_jobs(*args, **_):
         args[1].append(args[0])
 
@@ -242,14 +243,15 @@
     assert commander.planned_jobs == {'then': {2: command_list_2}, 'else': {}}
     assert commander.current_jobs == {}
     assert not mocked_job.called
 
 
 def test_commander_trigger_jobs(mocker, commander, command_list_1, command_list_2):
     """ Test the Commander.trigger_jobs method. """
+    commander.pickup_logic = min
     # test with empty structure
     commander.planned_sequence = {}
     commander.trigger_jobs()
     assert commander.planned_jobs == {}
     # test with complex structure
     commander.planned_sequence = {0: {'if': {2: [], 0: command_list_1},
                                       'then': {2: command_list_2}},
@@ -1071,20 +1073,22 @@
     stopper.on_event(command.process)
     assert command in stopper.current_jobs['crash']
     assert not mocked_after.called
 
 
 def test_stopper_store_application_stop_sequence(stopper, command_list):
     """ Test the Stopper.store_application_stop_sequence method. """
-    # create 2 application start_sequences
+    # create 2 application stop sequences
     appli1 = create_application('sample_test_1', stopper.supvisors)
+    appli1.rules.stop_sequence = 0
     for command in command_list:
         if command.process.application_name == 'sample_test_1':
             appli1.stop_sequence.setdefault(len(command.process.namespec) % 3, []).append(command.process)
     appli2 = create_application('sample_test_2', stopper.supvisors)
+    appli2.rules.stop_sequence = 0
     for command in command_list:
         if command.process.application_name == 'sample_test_2':
             appli2.stop_sequence.setdefault(len(command.process.namespec) % 3, []).append(command.process)
     # call method and check result
     stopper.store_application_stop_sequence(appli1)
     # check application sequence in stopper planned sequence
     expected = {0: {'sample_test_1': {1: ['sample_test_1:xfontsel', 'sample_test_1:xlogo'],
@@ -1175,14 +1179,15 @@
     assert not stopper.stop_application(appli)
     assert mocked_store.call_args_list == [call(appli)]
     assert not mocked_jobs.called
 
 
 def test_stopper_stop_applications(mocker, stopper, command_list):
     """ Test the Stopper.stop_applications method. """
+    stopper.pickup_logic = max
     # create one running application with a start_sequence > 0
     appli = create_application('sample_test_1', stopper.supvisors)
     mocker.patch.object(appli, 'has_running_processes', return_value=True)
     appli.rules.stop_sequence = 2
     stopper.supvisors.context.applications['sample_test_1'] = appli
     for command in command_list:
         if command.process.application_name == 'sample_test_1':
@@ -1197,21 +1202,21 @@
     stopper.supvisors.context.applications['crash'] = appli
     for command in command_list:
         if command.process.application_name == 'crash':
             appli.stop_sequence.setdefault(len(command.process.namespec) % 3, []).append(command.process)
     # call starter start_applications and check that only sample_test_2 is triggered
     mocked_jobs = mocker.patch.object(stopper, 'process_application_jobs')
     stopper.stop_applications()
-    expected = {2: {'sample_test_1': {1: ['sample_test_1:xfontsel', 'sample_test_1:xlogo'],
-                                      2: ['sample_test_1:xclock']}}}
+    expected = {0: {'crash': {0: ['crash:late_segv'], 1: ['crash:segv']}}}
     assert stopper.printable_planned_sequence() == expected
-    assert stopper.printable_planned_jobs() == {'crash': {0: ['crash:late_segv'], 1: ['crash:segv']}}
+    assert stopper.printable_planned_jobs() == {'sample_test_1': {1: ['sample_test_1:xfontsel', 'sample_test_1:xlogo'],
+                                                                  2: ['sample_test_1:xclock']}}
     # current jobs is empty because of process_application_jobs mocking
     assert stopper.printable_current_jobs() == {}
-    assert mocked_jobs.call_args_list == [call('crash')]
+    assert mocked_jobs.call_args_list == [call('sample_test_1')]
 
 
 def test_stopper_after_jobs(stopper):
     """ Test the Stopper.after_jobs method. """
     # patch context
     appli_1 = Mock(start_failure=True)
     appli_2 = Mock(start_failure=False)
```

### Comparing `supvisors-0.8/supvisors/tests/test_context.py` & `supvisors-0.9/supvisors/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_infosource.py` & `supvisors-0.9/supvisors/tests/test_infosource.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_listener.py` & `supvisors-0.9/supvisors/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_mainloop.py` & `supvisors-0.9/supvisors/tests/test_mainloop.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_options.py` & `supvisors-0.9/supvisors/tests/test_options.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,220 +16,207 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ======================================================================
 
 import pytest
 import sys
 
+from supervisor.loggers import LevelsByName
+
 from supvisors.options import *
 from supvisors.ttypes import ConciliationStrategies, StartingStrategies
 
 from .configurations import *
 
 
 @pytest.fixture
 def opt():
     """ Create a Supvisors-like structure filled with some nodes. """
     return SupvisorsOptions()
 
 
 @pytest.fixture
+def filled_opt():
+    """ Test the values of options with defined Supvisors configuration. """
+    DefinedOptionConfiguration = {'address_list': 'cliche01,cliche03,cliche02',
+                                  'rules_file': 'my_movies.xml', 'auto_fence': 'true',
+                                  'internal_port': '60001', 'event_port': '60002',
+                                  'synchro_timeout': '20', 'force_synchro_if': 'cliche01,cliche03',
+                                  'starting_strategy': 'MOST_LOADED', 'conciliation_strategy': 'SENICIDE',
+                                  'stats_periods': '5,60,600', 'stats_histo': '100', 'stats_irix_mode': 'true',
+                                  'logfile': '/tmp/supvisors.log', 'logfile_maxbytes': '50KB',
+                                  'logfile_backups': '5', 'loglevel': 'error'}
+    return SupvisorsOptions(**DefinedOptionConfiguration)
+
+
+@pytest.fixture
 def server_opt():
     """ Create a Supvisors-like structure filled with some nodes. """
     return SupvisorsServerOptions()
 
 
 def test_options_creation(opt):
-    """ Test the values set at construction. """
+    """ Test the values set at construction with empty config. """
     # all attributes are None
-    assert opt.address_list is None
+    assert opt.address_list == [gethostname()]
     assert opt.rules_file is None
-    assert opt.internal_port is None
-    assert opt.event_port is None
-    assert opt.auto_fence is None
-    assert opt.synchro_timeout is None
-    assert opt.force_synchro_if is None
-    assert opt.conciliation_strategy is None
-    assert opt.starting_strategy is None
-    assert opt.stats_periods is None
-    assert opt.stats_histo is None
-    assert opt.stats_irix_mode is None
-    assert opt.logfile is None
-    assert opt.logfile_maxbytes is None
-    assert opt.logfile_backups is None
-    assert opt.loglevel is None
+    assert opt.internal_port == 65001
+    assert opt.event_port == 65002
+    assert not opt.auto_fence
+    assert opt.synchro_timeout == 15
+    assert opt.force_synchro_if == set()
+    assert opt.conciliation_strategy == ConciliationStrategies.USER
+    assert opt.starting_strategy == StartingStrategies.CONFIG
+    assert opt.stats_periods == [10]
+    assert opt.stats_histo == 200
+    assert not opt.stats_irix_mode
+    assert opt.logfile is Automatic
+    assert opt.logfile_maxbytes == 50 * 1024 * 1024
+    assert opt.logfile_backups == 10
+    assert opt.loglevel == LevelsByName.INFO
+    assert opt.procnumbers == {}
+
+
+def test_filled_options_creation(filled_opt):
+    """ Test the values set at construction with config provided by Supervisor. """
+    assert filled_opt.address_list == ['cliche01', 'cliche03', 'cliche02']
+    assert filled_opt.rules_file == 'my_movies.xml'
+    assert filled_opt.internal_port == 60001
+    assert filled_opt.event_port == 60002
+    assert filled_opt.auto_fence
+    assert filled_opt.synchro_timeout == 20
+    assert filled_opt.force_synchro_if == {'cliche01', 'cliche03'}
+    assert filled_opt.conciliation_strategy == ConciliationStrategies.SENICIDE
+    assert filled_opt.starting_strategy == StartingStrategies.MOST_LOADED
+    assert filled_opt.stats_periods == [5, 60, 600]
+    assert filled_opt.stats_histo == 100
+    assert filled_opt.stats_irix_mode
+    assert filled_opt.logfile == '/tmp/supvisors.log'
+    assert filled_opt.logfile_maxbytes == 50 * 1024
+    assert filled_opt.logfile_backups == 5
+    assert filled_opt.loglevel == 40
 
 
 def test_str(opt):
     """ Test the string output. """
-    assert str(opt) == 'address_list=None rules_file=None internal_port=None event_port=None auto_fence=None '\
-                       'synchro_timeout=None force_synchro_if=None conciliation_strategy=None ' \
-                       'starting_strategy=None stats_periods=None stats_histo=None ' \
-                       'stats_irix_mode=None logfile=None logfile_maxbytes=None logfile_backups=None loglevel=None'
+    assert str(opt) == "address_list=['{}'] rules_file=None internal_port=65001 event_port=65002 auto_fence=False"\
+                       " synchro_timeout=15 force_synchro_if=set() conciliation_strategy=USER"\
+                       " starting_strategy=CONFIG stats_periods=[10] stats_histo=200 stats_irix_mode=False"\
+                       " logfile={} logfile_maxbytes={} logfile_backups=10 loglevel=20 procnumbers={}"\
+                       .format(gethostname(), Automatic, 50 * 1024 * 1024, {})
 
 
 common_error_message = r'invalid value for {}'
 
 
 def test_port_num():
     """ Test the conversion into to a port number. """
     error_message = common_error_message.format('port')
     # test invalid values
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_port_num('-1')
+        SupvisorsOptions.to_port_num('-1')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_port_num('0')
+        SupvisorsOptions.to_port_num('0')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_port_num('65536')
+        SupvisorsOptions.to_port_num('65536')
     # test valid values
-    assert SupvisorsServerOptions.to_port_num('1') == 1
-    assert SupvisorsServerOptions.to_port_num('65535') == 65535
+    assert SupvisorsOptions.to_port_num('1') == 1
+    assert SupvisorsOptions.to_port_num('65535') == 65535
 
 
 def test_timeout():
     """ Test the conversion of a string to a timeout value. """
     error_message = common_error_message.format('synchro_timeout')
     # test invalid values
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_timeout('-1')
+        SupvisorsOptions.to_timeout('-1')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_timeout('0')
+        SupvisorsOptions.to_timeout('0')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_timeout('14')
+        SupvisorsOptions.to_timeout('14')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_timeout('1201')
+        SupvisorsOptions.to_timeout('1201')
     # test valid values
-    assert SupvisorsServerOptions.to_timeout('15') == 15
-    assert SupvisorsServerOptions.to_timeout('1200') == 1200
+    assert SupvisorsOptions.to_timeout('15') == 15
+    assert SupvisorsOptions.to_timeout('1200') == 1200
 
 
 def test_conciliation_strategy():
     """ Test the conversion of a string to a conciliation strategy. """
     error_message = common_error_message.format('conciliation_strategy')
     # test invalid values
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_conciliation_strategy('123456')
+        SupvisorsOptions.to_conciliation_strategy('123456')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_conciliation_strategy('dummy')
+        SupvisorsOptions.to_conciliation_strategy('dummy')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_conciliation_strategy('user')
+        SupvisorsOptions.to_conciliation_strategy('user')
     # test valid values
-    assert SupvisorsServerOptions.to_conciliation_strategy('SENICIDE') == ConciliationStrategies.SENICIDE
-    assert SupvisorsServerOptions.to_conciliation_strategy('INFANTICIDE') == ConciliationStrategies.INFANTICIDE
-    assert SupvisorsServerOptions.to_conciliation_strategy('USER') == ConciliationStrategies.USER
-    assert SupvisorsServerOptions.to_conciliation_strategy('STOP') == ConciliationStrategies.STOP
-    assert SupvisorsServerOptions.to_conciliation_strategy('RESTART') == ConciliationStrategies.RESTART
+    assert SupvisorsOptions.to_conciliation_strategy('SENICIDE') == ConciliationStrategies.SENICIDE
+    assert SupvisorsOptions.to_conciliation_strategy('INFANTICIDE') == ConciliationStrategies.INFANTICIDE
+    assert SupvisorsOptions.to_conciliation_strategy('USER') == ConciliationStrategies.USER
+    assert SupvisorsOptions.to_conciliation_strategy('STOP') == ConciliationStrategies.STOP
+    assert SupvisorsOptions.to_conciliation_strategy('RESTART') == ConciliationStrategies.RESTART
 
 
 def test_starting_strategy():
     """ Test the conversion of a string to a starting strategy. """
     error_message = common_error_message.format('starting_strategy')
     # test invalid values
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_starting_strategy('123456')
+        SupvisorsOptions.to_starting_strategy('123456')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_starting_strategy('dummy')
+        SupvisorsOptions.to_starting_strategy('dummy')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_starting_strategy('config')
+        SupvisorsOptions.to_starting_strategy('config')
     # test valid values
-    assert SupvisorsServerOptions.to_starting_strategy('CONFIG') == StartingStrategies.CONFIG
-    assert SupvisorsServerOptions.to_starting_strategy('LESS_LOADED') == StartingStrategies.LESS_LOADED
-    assert SupvisorsServerOptions.to_starting_strategy('MOST_LOADED') == StartingStrategies.MOST_LOADED
+    assert SupvisorsOptions.to_starting_strategy('CONFIG') == StartingStrategies.CONFIG
+    assert SupvisorsOptions.to_starting_strategy('LESS_LOADED') == StartingStrategies.LESS_LOADED
+    assert SupvisorsOptions.to_starting_strategy('MOST_LOADED') == StartingStrategies.MOST_LOADED
 
 
 def test_periods():
     """ Test the conversion of a string to a list of periods. """
     error_message = common_error_message.format('stats_periods')
     # test invalid values
     with pytest.raises(ValueError, match='unexpected number of stats_periods'):
-        SupvisorsServerOptions.to_periods([])
+        SupvisorsOptions.to_periods([])
     with pytest.raises(ValueError, match='unexpected number of stats_periods'):
-        SupvisorsServerOptions.to_periods(['1', '2', '3', '4'])
+        SupvisorsOptions.to_periods(['1', '2', '3', '4'])
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_periods(['4', '3600'])
+        SupvisorsOptions.to_periods(['4', '3600'])
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_periods(['5', '3601'])
+        SupvisorsOptions.to_periods(['5', '3601'])
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_periods(['6', '3599'])
+        SupvisorsOptions.to_periods(['6', '3599'])
     # test valid values
-    assert SupvisorsServerOptions.to_periods(['5']) == [5]
-    assert SupvisorsServerOptions.to_periods(['60', '3600']) == [60, 3600]
-    assert SupvisorsServerOptions.to_periods(['120', '720', '1800']) == [120, 720, 1800]
+    assert SupvisorsOptions.to_periods(['5']) == [5]
+    assert SupvisorsOptions.to_periods(['60', '3600']) == [60, 3600]
+    assert SupvisorsOptions.to_periods(['120', '720', '1800']) == [120, 720, 1800]
 
 
 def test_histo():
     """ Test the conversion of a string to a history depth. """
     error_message = common_error_message.format('stats_histo')
     # test invalid values
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_histo('-1')
+        SupvisorsOptions.to_histo('-1')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_histo('9')
+        SupvisorsOptions.to_histo('9')
     with pytest.raises(ValueError, match=error_message):
-        SupvisorsServerOptions.to_histo('1501')
+        SupvisorsOptions.to_histo('1501')
     # test valid values
-    assert SupvisorsServerOptions.to_histo('10') == 10
-    assert SupvisorsServerOptions.to_histo('1500') == 1500
-
-
-def test_incorrect_supvisors(mocker, server_opt):
-    """ Test that exception is raised when the supvisors section is missing. """
-    with pytest.raises(ValueError):
-        create_server(mocker, server_opt, NoSupvisors)
+    assert SupvisorsOptions.to_histo('10') == 10
+    assert SupvisorsOptions.to_histo('1500') == 1500
 
 
 def test_program_numbers(mocker, server_opt):
     """ Test that the internal numbers of homogeneous programs are stored. """
     server = create_server(mocker, server_opt, ProgramConfiguration)
-    assert server.supvisors_options.procnumbers == {'dummy': 0, 'dummy_0': 0, 'dummy_1': 1, 'dummy_2': 2,
-                                                    'dumber_10': 0, 'dumber_11': 1}
-
-
-def test_default_options(mocker, server_opt):
-    """ Test the default values of options with empty Supvisors configuration. """
-    server = create_server(mocker, server_opt, DefaultOptionConfiguration)
-    opt = server.supvisors_options
-    assert opt.address_list == [gethostname()]
-    assert opt.rules_file is None
-    assert opt.internal_port == 65001
-    assert opt.event_port == 65002
-    assert not opt.auto_fence
-    assert opt.synchro_timeout == 15
-    assert opt.force_synchro_if == set()
-    assert opt.conciliation_strategy == ConciliationStrategies.USER
-    assert opt.starting_strategy == StartingStrategies.CONFIG
-    assert opt.stats_periods == [10]
-    assert opt.stats_histo == 200
-    assert not opt.stats_irix_mode
-    assert opt.logfile == Automatic
-    assert opt.logfile_maxbytes == 50 * 1024 * 1024
-    assert opt.logfile_backups == 10
-    assert opt.loglevel == 20
-
-
-def test_defined_options(mocker, server_opt):
-    """ Test the values of options with defined Supvisors configuration. """
-    server = create_server(mocker, server_opt, DefinedOptionConfiguration)
-    opt = server.supvisors_options
-    assert opt.address_list == ['cliche01', 'cliche03', 'cliche02']
-    assert opt.rules_file == 'my_movies.xml'
-    assert opt.internal_port == 60001
-    assert opt.event_port == 60002
-    assert opt.auto_fence
-    assert opt.synchro_timeout == 20
-    assert opt.force_synchro_if == {'cliche01', 'cliche03'}
-    assert opt.conciliation_strategy == ConciliationStrategies.SENICIDE
-    assert opt.starting_strategy == StartingStrategies.MOST_LOADED
-    assert opt.stats_periods == [5, 60, 600]
-    assert opt.stats_histo == 100
-    assert opt.stats_irix_mode
-    assert opt.logfile == '/tmp/supvisors.log'
-    assert opt.logfile_maxbytes == 50 * 1024
-    assert opt.logfile_backups == 5
-    assert opt.loglevel == 40
+    assert server.procnumbers == {'dummy': 0, 'dummy_0': 0, 'dummy_1': 1, 'dummy_2': 2, 'dumber_10': 0, 'dumber_11': 1}
 
 
 def create_server(mocker, server_opt, config):
     """ Create a SupvisorsServerOptions instance using patches on Supervisor source code.
     This is required because the unit test does not include existing files. """
     mocker.patch.object(ServerOptions, 'default_configfile', return_value='supervisord.conf')
     mocker.patch.object(ServerOptions, 'exists', return_value=True)
```

### Comparing `supvisors-0.8/supvisors/tests/test_plot.py` & `supvisors-0.9/supvisors/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_plugin.py` & `supvisors-0.9/supvisors/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_process.py` & `supvisors-0.9/supvisors/tests/test_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,31 +37,32 @@
     return ProcessRules(supvisors)
 
 
 def test_rules_create(supvisors, rules):
     """ Test the values set at construction. """
     assert rules.supvisors is supvisors
     assert rules.node_names == ['*']
+    assert rules.hash_node_names == []
     assert rules.start_sequence == 0
-    assert rules.stop_sequence == 0
+    assert rules.stop_sequence == -1
     assert not rules.required
     assert not rules.wait_exit
     assert rules.expected_load == 0
     assert rules.running_failure_strategy == RunningFailureStrategies.CONTINUE
 
 
 def test_rules_str(rules):
     """ Test the string output. """
-    assert str(rules) == "node_names=['*'] hash_node_names=[] start_sequence=0 stop_sequence=0 required=False"\
+    assert str(rules) == "node_names=['*'] hash_node_names=[] start_sequence=0 stop_sequence=-1 required=False"\
         " wait_exit=False expected_load=0 running_failure_strategy=CONTINUE"
 
 
 def test_rules_serial(rules):
     """ Test the serialization of the ProcessRules object. """
-    assert rules.serial() == {'addresses': ['*'], 'start_sequence': 0, 'stop_sequence': 0,
+    assert rules.serial() == {'addresses': ['*'], 'start_sequence': 0, 'stop_sequence': -1,
                               'required': False, 'wait_exit': False, 'expected_loading': 0,
                               'running_failure_strategy': 'CONTINUE'}
 
 
 def test_rules_check_start_sequence(rules):
     """ Test the dependencies in process rules. """
     # 1. test with not required and no start sequence
@@ -94,14 +95,30 @@
     # check dependencies
     rules.check_dependencies('dummy')
     # check rules unchanged
     assert rules.start_sequence == 1
     assert rules.required
 
 
+def test_rules_check_stop_sequence(rules):
+    """ Test the assignment of stop sequence to start sequence if default still set. """
+    # test when default still used
+    assert rules.start_sequence == 0
+    assert rules.stop_sequence == -1
+    rules.check_stop_sequence('crash')
+    assert rules.start_sequence == 0
+    assert rules.stop_sequence == 0
+    # test when value has been set
+    rules.start_sequence = 12
+    rules.stop_sequence = 50
+    rules.check_stop_sequence('crash')
+    assert rules.start_sequence == 12
+    assert rules.stop_sequence == 50
+
+
 def test_rules_check_autorestart(rules):
     """ Test the dependency related to running failure strategy in process rules.
     Done in a separate test as it impacts the supervisor internal model. """
     # test based on programs unknown to Supervisor
     mocked_disable = rules.supvisors.info_source.disable_autorestart
     mocked_autorestart = rules.supvisors.info_source.autorestart
     mocked_autorestart.side_effect = KeyError
@@ -136,26 +153,25 @@
             assert not mocked_disable.called
         else:
             assert mocked_disable.call_args_list == [call('dummy_process_1')]
             mocked_disable.reset_mock()
 
 
 def test_rules_check_hash_nodes(rules):
-    """ Test the resolution of addresses when hash_address is set. """
-    # check initial attributes
-    assert rules.node_names == ['*']
-    assert rules.hash_node_names == []
+    """ Test the resolution of nodes when hash_node_names is set. """
+    # set initial attributes
+    rules.hash_node_names = ['*']
+    rules.node_names = []
     # in mocked supvisors, xclock has a procnumber of 2
     # 1. test with unknown namespec
     rules.check_hash_nodes('sample_test_1:xfontsel')
     # node_names is unchanged
-    assert rules.node_names == ['*']
+    assert rules.hash_node_names == ['*']
+    assert rules.node_names == []
     # 2. update rules to test '#' with all nodes available
-    rules.hash_node_names = ['*']
-    rules.node_names = []
     # address '10.0.0.2' has an index of 2 in address_mapper
     rules.check_hash_nodes('sample_test_1:xclock')
     assert rules.node_names == ['10.0.0.2']
     # 3. update rules to test '#' with a subset of nodes available
     rules.hash_node_names = ['10.0.0.0', '10.0.0.3', '10.0.0.5']
     rules.node_names = []
     # here, at index 2 of this list, '10.0.0.5' can be found
@@ -169,31 +185,33 @@
 
 
 def test_rules_check_dependencies(mocker, rules):
     """ Test the dependencies in process rules. """
     mocked_hash = mocker.patch('supvisors.process.ProcessRules.check_hash_nodes')
     mocked_auto = mocker.patch('supvisors.process.ProcessRules.check_autorestart')
     mocked_start = mocker.patch('supvisors.process.ProcessRules.check_start_sequence')
+    mocked_stop = mocker.patch('supvisors.process.ProcessRules.check_stop_sequence')
     # test with no hash
     rules.hash_node_names = []
     # check dependencies
     rules.check_dependencies('dummy')
     # test calls
     assert mocked_start.call_args_list == [call('dummy')]
+    assert mocked_stop.call_args_list == [call('dummy')]
     assert mocked_auto.call_args_list == [call('dummy')]
     assert not mocked_hash.called
     # reset mocks
-    mocked_start.reset_mock()
-    mocked_auto.reset_mock()
+    mocker.resetall()
     # test with hash
     rules.hash_node_names = ['*']
     # check dependencies
     rules.check_dependencies('dummy')
     # test calls
     assert mocked_start.call_args_list == [call('dummy')]
+    assert mocked_stop.call_args_list == [call('dummy')]
     assert mocked_auto.call_args_list == [call('dummy')]
     assert mocked_hash.call_args_list == [call('dummy')]
 
 
 # ProcessStatus part
 def test_process_create(supvisors):
     """ Test the values set at ProcessStatus construction. """
```

### Comparing `supvisors-0.8/supvisors/tests/test_rpcinterface.py` & `supvisors-0.9/supvisors/tests/test_rpcinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,24 +197,24 @@
     assert rpc.get_application_rules('appli') == expected
     assert mocked_check.call_args_list == [call()]
     assert mocked_get.call_args_list == [call('appli')]
     mocker.resetall()
     # test RPC call with application name and managed/distributed application
     application.rules.managed = True
     expected = {'application_name': 'appli', 'managed': True, 'distributed': True,
-                'start_sequence': 0, 'stop_sequence': 0, 'starting_strategy': 'CONFIG',
+                'start_sequence': 0, 'stop_sequence': -1, 'starting_strategy': 'CONFIG',
                 'starting_failure_strategy': 'ABORT', 'running_failure_strategy': 'CONTINUE'}
     assert rpc.get_application_rules('appli') == expected
     assert mocked_check.call_args_list == [call()]
     assert mocked_get.call_args_list == [call('appli')]
     mocker.resetall()
     # test RPC call with application name and managed/non-distributed application
     application.rules.distributed = False
     expected = {'application_name': 'appli', 'managed': True, 'distributed': False, 'addresses': ['*'],
-                'start_sequence': 0, 'stop_sequence': 0, 'starting_strategy': 'CONFIG',
+                'start_sequence': 0, 'stop_sequence': -1, 'starting_strategy': 'CONFIG',
                 'starting_failure_strategy': 'ABORT', 'running_failure_strategy': 'CONTINUE'}
     assert rpc.get_application_rules('appli') == expected
     assert mocked_check.call_args_list == [call()]
     assert mocked_get.call_args_list == [call('appli')]
 
 
 def test_process_rules(mocker, rpc):
```

### Comparing `supvisors-0.8/supvisors/tests/test_rpcrequests.py` & `supvisors-0.9/supvisors/tests/test_rpcrequests.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_sparser.py` & `supvisors-0.9/supvisors/tests/test_sparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     assert rules.required == required
     assert rules.wait_exit == wait
     assert rules.expected_load == expected_load
     assert rules.running_failure_strategy == running_strategy
 
 
 def load_application_rules(parser, application_name):
-    rules = ApplicationRules()
+    rules = ApplicationRules(parser.supvisors)
     parser.load_application_rules(application_name, rules)
     return rules
 
 
 def load_program_rules(parser, application_name, process_name):
     rules = ProcessRules(parser.supvisors)
     parser.load_program_rules('%s:%s' % (application_name, process_name), rules)
@@ -109,15 +109,14 @@
                              StartingFailureStrategies.STOP, RunningFailureStrategies.RESTART_PROCESS)
     # check third application
     rules = load_application_rules(parser, 'dummy_application_C')
     assert_application_rules(rules, True, True, ['*'], 20, 0, StartingStrategies.LOCAL,
                              StartingFailureStrategies.ABORT, RunningFailureStrategies.STOP_APPLICATION)
     # check fourth application
     rules = load_application_rules(parser, 'dummy_application_D')
-    print(rules)
     assert_application_rules(rules, True, False, ['10.0.0.1', '10.0.0.5'], 0, 100, StartingStrategies.LESS_LOADED,
                              StartingFailureStrategies.CONTINUE, RunningFailureStrategies.RESTART_APPLICATION)
     # check loop application
     rules = load_application_rules(parser, 'dummy_application_E')
     assert_application_rules(rules, True, True,  ['*'], 0, 0,  StartingStrategies.MOST_LOADED,
                              StartingFailureStrategies.ABORT, RunningFailureStrategies.CONTINUE)
     # check program from unknown application: all default
@@ -130,55 +129,48 @@
     rules = load_program_rules(parser, 'dummy_application_A', 'dummy_program_B1')
     assert_default_process_rules(rules)
     # check known empty program
     rules = load_program_rules(parser, 'dummy_application_B', 'dummy_program_B0')
     assert_default_process_rules(rules)
     # check dash addresses and valid other values
     rules = load_program_rules(parser, 'dummy_application_B', 'dummy_program_B1')
-    assert_process_rules(rules, [], ['*'], 3, 50, True, False, 5,
-                         RunningFailureStrategies.CONTINUE)
+    assert_process_rules(rules, [], ['*'], 3, 50, True, False, 5, RunningFailureStrategies.CONTINUE)
     # check single address with required not applicable and out of range loading
     rules = load_program_rules(parser, 'dummy_application_B', 'dummy_program_B2')
-    assert_process_rules(rules, ['10.0.0.3'], [], 0, 0, False, False, 0,
-                         RunningFailureStrategies.RESTART_PROCESS)
+    assert_process_rules(rules, ['10.0.0.3'], [], 0, 0, False, False, 0, RunningFailureStrategies.RESTART_PROCESS)
     # check wildcard address, optional and max loading
     rules = load_program_rules(parser, 'dummy_application_B', 'dummy_program_B3')
-    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 100,
-                         RunningFailureStrategies.STOP_APPLICATION)
+    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 100, RunningFailureStrategies.STOP_APPLICATION)
     # check multiple addresses, all other incorrect values
     rules = load_program_rules(parser, 'dummy_application_B', 'dummy_program_B4')
     assert_process_rules(rules, ['10.0.0.3', '10.0.0.1', '10.0.0.5'], [], 0, 0, False, False, 0,
                          RunningFailureStrategies.RESTART_APPLICATION)
     # check empty reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C0')
     assert_default_process_rules(rules)
     # check unknown reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C1')
     assert_default_process_rules(rules)
     # check known reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C2')
-    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 25,
-                         RunningFailureStrategies.STOP_APPLICATION)
+    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 25, RunningFailureStrategies.STOP_APPLICATION)
     # check other known reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C3')
-    assert_process_rules(rules, [], ['*'], 1, 0, True, True, 0,
-                         RunningFailureStrategies.CONTINUE)
+    assert_process_rules(rules, [], ['*'], 1, 1, True, True, 0, RunningFailureStrategies.CONTINUE)
     # check pattern with single matching and reference
     rules = load_program_rules(parser, 'dummy_application_D', 'dummies_any')
     assert_process_rules(rules, ['10.0.0.4', '10.0.0.2'], [], 50, 100, False, False, 10,
                          RunningFailureStrategies.CONTINUE)
     # check pattern with multiple matching and configuration
     rules = load_program_rules(parser, 'dummy_application_D', 'dummies_01_any')
-    assert_process_rules(rules, [], ['10.0.0.1', '10.0.0.5'], 1, 1, False, True, 75,
-                         RunningFailureStrategies.CONTINUE)
+    assert_process_rules(rules, [], ['10.0.0.1', '10.0.0.5'], 1, 1, False, True, 75, RunningFailureStrategies.CONTINUE)
     # check pattern with multiple matching and incorrect reference (model calling for another model)
     # this is valid since Supvisors 0.5
     rules = load_program_rules(parser, 'dummy_application_D', 'any_dummies_02_')
-    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 20,
-                         RunningFailureStrategies.STOP_APPLICATION)
+    assert_process_rules(rules, ['*'], [], 0, 0, False, False, 20, RunningFailureStrategies.STOP_APPLICATION)
     # check multiple reference (over the maximum defined)
     # almost all rules set to default, despite enf of chain is on dummy_model_01
     rules = load_program_rules(parser, 'dummy_application_E', 'dummy_program_E')
     assert_process_rules(rules, ['*'], [], 0, 0, False, False, 15,
                          RunningFailureStrategies.CONTINUE)
 
 
@@ -254,43 +246,43 @@
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C1')
     assert_default_process_rules(rules)
     # check known reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C2')
     assert_process_rules(rules, ['*'], [], 0, 0, False, False, 25, RunningFailureStrategies.STOP_APPLICATION)
     # check other known reference
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C3')
-    assert_process_rules(rules, [], ['*'], 1, 0, True, True, 0, RunningFailureStrategies.CONTINUE)
+    assert_process_rules(rules, [], ['*'], 1, 1, True, True, 0, RunningFailureStrategies.CONTINUE)
     # check other known reference with additional unexpected configuration
-    # WARN: this is valid since Supvisors 0.5
     rules = load_program_rules(parser, 'dummy_application_C', 'dummy_program_C4')
     assert_process_rules(rules, [], ['*'], 3, 100, True, False, 5, RunningFailureStrategies.CONTINUE)
     # check pattern with single matching and reference
     # check that existing values are not reset
     rules = ProcessRules(parser.supvisors)
     rules.running_failure_strategy = RunningFailureStrategies.RESTART_APPLICATION
     parser.load_program_rules('dummy_application_D:dummies_any', rules)
     assert_process_rules(rules, ['10.0.0.4', '10.0.0.2'], [], 0, 100, False, False, 10,
                          RunningFailureStrategies.RESTART_APPLICATION)
     # check pattern with multiple matching and configuration
     rules = load_program_rules(parser, 'dummy_application_D', 'dummies_01_any')
     assert_process_rules(rules, [], ['*'], 1, 1, False, True, 75, RunningFailureStrategies.CONTINUE)
     # check pattern with multiple matching and recursive reference
-    # WARN: this is valid since Supvisors 0.5
     rules = load_program_rules(parser, 'dummy_application_D', 'any_dummies_02_')
     assert_process_rules(rules, ['*'], [], 0, 0, False, False, 25, RunningFailureStrategies.STOP_APPLICATION)
 
 
 @pytest.fixture
 def lxml_import():
     return pytest.importorskip('lxml')
 
 
 def test_valid_lxml(mocker, lxml_import, supvisors):
     """ Test the parsing using lxml (optional dependency). """
     mocker.patch.object(supvisors.options, 'rules_file', BytesIO(XmlTest))
+    mocker.patch('supvisors.application.ApplicationRules.check_hash_nodes')
+    mocker.patch('supvisors.process.ProcessRules.check_hash_nodes')
     parser = Parser(supvisors)
     check_valid(parser)
 
 
 def test_invalid_lxml(mocker, supvisors):
     """ Test the parsing of an invalid XML using lxml (optional dependency). """
     mocker.patch('supvisors.sparser.stderr')
@@ -313,17 +305,21 @@
         Parser(supvisors)
 
 
 def test_valid_element_tree(mocker, supvisors, lxml_fail_import):
     """ Test the parsing of a valid XML using ElementTree. """
     # create Parser instance
     mocker.patch.object(supvisors.options, 'rules_file', BytesIO(XmlTest))
+    mocker.patch('supvisors.application.ApplicationRules.check_hash_nodes')
+    mocker.patch('supvisors.process.ProcessRules.check_hash_nodes')
     parser = Parser(supvisors)
     check_valid(parser)
 
 
 def test_invalid_element_tree(mocker, supvisors, lxml_fail_import):
     """ Test the parsing of an invalid XML using ElementTree. """
     # create Parser instance
     mocker.patch.object(supvisors.options, 'rules_file', BytesIO(InvalidXmlTest))
+    mocker.patch('supvisors.application.ApplicationRules.check_hash_nodes')
+    mocker.patch('supvisors.process.ProcessRules.check_hash_nodes')
     parser = Parser(supvisors)
     check_invalid(parser)
```

### Comparing `supvisors-0.8/supvisors/tests/test_statemachine.py` & `supvisors-0.9/supvisors/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_statscollector.py` & `supvisors-0.9/supvisors/tests/test_statscollector.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_statscompiler.py` & `supvisors-0.9/supvisors/tests/test_statscompiler.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_strategy.py` & `supvisors-0.9/supvisors/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_supvisorsctl.py` & `supvisors-0.9/supvisors/tests/test_supvisorsctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # limitations under the License.
 # ======================================================================
 
 import pytest
 
 from unittest.mock import call, Mock
 
-from supervisor.supervisorctl import Controller
 from supervisor.xmlrpc import Faults
 
 from supvisors.supvisorsctl import *
 
 
 @pytest.fixture
 def controller():
@@ -68,15 +67,15 @@
         mocked_check.reset_mock()
     # test RPC
     assert mocked_rpc.call_args_list == rpc_result
     mocked_rpc.reset_mock()
     # test output (with no error)
     _check_output_error(controller, False)
     # test request error
-    mocked_rpc.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_rpc.side_effect = xmlrpclib.Fault(0, 'error')
     do_fct(arg)
     mocked_rpc.side_effect = None
     # test upcheck call if any
     if mocked_check:
         assert mocked_check.call_args_list == [call()]
         mocked_check.reset_mock()
     # test RPC
@@ -112,15 +111,15 @@
     assert mocked_appli.call_args_list == [call(), call()]
     mocked_appli.reset_mock()
     # test help and request for starting a selection
     _check_call(controller, mocked_check, mocked_rpc, help_cmd, do_cmd, 'CONFIG ' + sel_args,
                 [call(0, sel_result[0]), call(0, sel_result[1])])
     # test help and request with get_all_applications_info error
     mocked_appli.reset_mock()
-    mocked_appli.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_appli.side_effect = xmlrpclib.Fault(0, 'error')
     do_cmd('LESS_LOADED')
     assert mocked_appli.call_args_list == [call()]
     assert mocked_rpc.call_count == 0
     _check_output_error(controller, True)
 
 
 def _check_stop_command(controller, mocked_check, mocked_appli, mocked_rpc,
@@ -139,15 +138,15 @@
     assert mocked_appli.call_args_list == [call(), call()]
     mocked_appli.reset_mock()
     # test help and request for starting a selection of applications
     _check_call(controller, mocked_check, mocked_rpc, help_cmd, do_cmd,
                 sel_args, [call(sel_result[0]), call(sel_result[1])])
     # test help and request with get_all_applications_info error
     mocked_appli.reset_mock()
-    mocked_appli.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_appli.side_effect = xmlrpclib.Fault(0, 'error')
     do_cmd('')
     assert mocked_appli.call_args_list == [call()]
     assert mocked_rpc.call_count == 0
     _check_output_error(controller, True)
 
 
 def test_supvisors(controller, plugin):
@@ -280,15 +279,15 @@
     # test help and request for rules from a selection of application names
     mocked_rpc.side_effect = returned_rules
     _check_call(controller, mocked_check, mocked_rpc, plugin.help_application_rules, plugin.do_application_rules,
                 'appli_3 appli_2 appli_1', [call('appli_3'), call('appli_2'), call('appli_1')])
     assert mocked_appli.call_count == 0
     # test help and request with get_all_applications_info error
     mocked_appli.reset_mock()
-    mocked_appli.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_appli.side_effect = xmlrpclib.Fault(0, 'error')
     plugin.do_application_rules('')
     assert mocked_appli.call_args_list == [call()]
     assert mocked_rpc.call_count == 0
     _check_output_error(controller, True)
 
 
 def test_process_rules(controller, plugin, mocked_check):
@@ -317,15 +316,15 @@
     # test help and request for rules from a selection of namespecs
     mocked_rpc.side_effect = returned_rules
     _check_call(controller, mocked_check, mocked_rpc, plugin.help_process_rules, plugin.do_process_rules,
                 'appli_2:proc_3 appli_1:proc_1', [call('appli_2:proc_3'), call('appli_1:proc_1')])
     assert mocked_appli.call_count == 0
     # test help and request with get_all_applications_info error
     mocked_appli.reset_mock()
-    mocked_appli.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_appli.side_effect = xmlrpclib.Fault(0, 'error')
     plugin.do_process_rules('')
     assert mocked_appli.call_args_list == [call()]
     assert mocked_rpc.call_count == 0
     _check_output_error(controller, True)
 
 
 def test_conflicts(controller, plugin, mocked_check):
@@ -493,15 +492,15 @@
     # test handled RPC error
     mocked_rpc.side_effect = xmlrpclib.Fault(Faults.UNKNOWN_METHOD, '')
     assert not plugin._upcheck()
     _check_output_error(controller, True)
     assert mocked_rpc.call_args_list == [call()]
     mocked_rpc.reset_mock()
     # test not handled RPC error
-    mocked_rpc.side_effect = xmlrpclib.Fault('0', 'error')
+    mocked_rpc.side_effect = xmlrpclib.Fault(0, 'error')
     with pytest.raises(xmlrpclib.Fault):
         plugin._upcheck()
     assert mocked_rpc.call_args_list == [call()]
     mocked_rpc.reset_mock()
     # test handled socket errors
     mocked_rpc.side_effect = socket.error(errno.ECONNREFUSED)
     assert not plugin._upcheck()
@@ -527,7 +526,31 @@
 
 
 def test_make_plugin(mocker, controller):
     """ Test the plugin factory. """
     mocked_plugin = mocker.patch('supvisors.supvisorsctl.ControllerPlugin')
     make_supvisors_controller_plugin(controller)
     assert mocked_plugin.call_args_list == [call(controller)]
+
+
+def test_main(mocker):
+    """ Test the plugin factory. """
+    mocked_client_options = Mock(args=['start', 'program'], interactive=False, plugin_factories=[])
+    mocked_controller = Mock(exitstatus=2)
+    mocker.patch('supvisors.supvisorsctl.ClientOptions', return_value=mocked_client_options)
+    mocker.patch('supvisors.supvisorsctl.Controller', return_value=mocked_controller)
+    mocked_sys = mocker.patch('supvisors.supvisorsctl.sys')
+    # test with arguments
+    main(args='command args')
+    assert mocked_client_options.realize.call_args_list == [call('command args', doc=supervisorctl.__doc__)]
+    assert mocked_controller.onecmd.call_args_list == [call('start program')]
+    assert not mocked_controller.exec_cmdloop.called
+    assert mocked_sys.exit.call_args_list == [call(2)]
+    mocker.resetall()
+    # test without arguments
+    mocked_client_options.args = None
+    mocked_client_options.interactive = True
+    main()
+    assert mocked_client_options.realize.call_args_list == [call(None, doc=supervisorctl.__doc__)]
+    assert not mocked_controller.onecmd.called
+    assert mocked_controller.exec_cmdloop.call_args_list == [call(None, mocked_client_options)]
+    assert mocked_sys.exit.call_args_list == [call(0)]
```

### Comparing `supvisors-0.8/supvisors/tests/test_supvisorszmq.py` & `supvisors-0.9/supvisors/tests/test_supvisorszmq.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_ttypes.py` & `supvisors-0.9/supvisors/tests/test_ttypes.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_utils.py` & `supvisors-0.9/supvisors/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_viewapplication.py` & `supvisors-0.9/supvisors/tests/test_viewapplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,32 +47,33 @@
     assert isinstance(view, MeldView)
     assert view.application_name == ''
     assert view.application is None
 
 
 def test_handle_parameters(mocker, view):
     """ Test the handle_parameters method. """
-    mocked_message = mocker.patch('supvisors.viewapplication.error_message', return_value='an error')
+    mocker.patch('supvisors.viewapplication.error_message', return_value='an error')
     mocked_handle = mocker.patch('supvisors.viewhandler.ViewHandler.handle_parameters')
     # patch context
-    view.view_ctx = Mock(parameters={APPLI: None})
+    view.view_ctx = Mock(parameters={APPLI: None}, store_message=None, redirect=False)
     # test with no application selected
     view.handle_parameters()
     assert mocked_handle.call_args_list == [call(view)]
     assert view.application is None
-    assert view.view_ctx.message.call_args_list == [call('an error')]
+    assert view.view_ctx.store_message == 'an error'
+    assert view.view_ctx.redirect
     mocked_handle.reset_mock()
-    view.view_ctx.message.reset_mock()
     # test with application selected
-    view.view_ctx = Mock(parameters={APPLI: 'dummy_appli'})
+    view.view_ctx = Mock(parameters={APPLI: 'dummy_appli'}, store_message=None, redirect=False)
     view.sup_ctx.applications['dummy_appli'] = 'dummy_appli'
     view.handle_parameters()
     assert mocked_handle.call_args_list == [call(view)]
     assert view.application == 'dummy_appli'
-    assert view.view_ctx.message.call_args_list == []
+    assert view.view_ctx.store_message is None
+    assert not view.view_ctx.redirect
 
 
 def test_write_navigation(mocker, view):
     """ Test the write_navigation method. """
     mocked_handle = mocker.patch('supvisors.viewhandler.ViewHandler.write_nav')
     view.application_name = 'dummy_appli'
     # test with no application selected
@@ -193,14 +194,15 @@
     mocked_stats = mocker.patch('supvisors.viewhandler.ViewHandler.write_process_statistics')
     mocked_table = mocker.patch('supvisors.viewapplication.ApplicationView.write_process_table')
     mocked_data = mocker.patch('supvisors.viewapplication.ApplicationView.get_process_data',
                                side_effect=([{'namespec': 'dummy'}], [{'namespec': 'dummy'}],
                                             [{'namespec': 'dummy'}], [{'namespec': 'dummy_proc'}],
                                             [{'namespec': 'dummy_proc'}]))
     view.application_name = 'dummy_appli'
+    view.application = Mock()
     # patch context
     view.view_ctx = Mock(parameters={PROCESS: None}, **{'get_process_status.return_value': None})
     # patch the meld elements
     mocked_root = Mock()
     # test call with no process selected
     view.write_contents(mocked_root)
     assert mocked_data.call_args_list == [call()]
@@ -363,14 +365,15 @@
     mocked_start_proc = mocker.patch.object(view, 'start_process_action', return_value='Start process')
     mocked_restart_app = mocker.patch.object(view, 'restart_application_action', return_value='Restart application')
     mocked_stop_app = mocker.patch.object(view, 'stop_application_action', return_value='Stop application')
     mocked_start_app = mocker.patch.object(view, 'start_application_action', return_value='Start application')
     mocker.patch.object(view, 'refresh_action', return_value='Refresh')
     # patch view context
     view.view_ctx = Mock(parameters={STRATEGY: 'LOCAL'}, **{'get_process_status.return_value': None})
+    view.application = Mock()
     # test calls for different actions
     assert view.make_callback('', 'refresh') == 'Refresh'
     assert view.make_callback('', 'startapp') == 'Start application'
     assert mocked_start_app.call_args_list == [call(StartingStrategies.LOCAL)]
     assert view.make_callback('', 'stopapp') == 'Stop application'
     assert mocked_stop_app.call_args_list == [call()]
     assert view.make_callback('', 'restartapp') == 'Restart application'
```

### Comparing `supvisors-0.8/supvisors/tests/test_viewcontext.py` & `supvisors-0.9/supvisors/tests/test_viewcontext.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,19 @@
     """ Test the values set at ViewContext construction. """
     assert ctx.http_context is http_context
     assert ctx.supvisors is http_context.supervisord.supvisors
     assert ctx.local_node_name == ctx.supvisors.address_mapper.local_node_name
     assert ctx.parameters == {'node': '10.0.0.4', 'namespec': None, 'period': 5,
                               'appliname': None, 'processname': None, 'cpuid': 0,
                               'intfname': None, 'auto': False, 'strategy': 'CONFIG', 'shex': ''}
+    # errors must be set due to dummy values
+    assert isinstance(ctx.store_message, tuple)
+    assert len(ctx.store_message) == 2
+    assert ctx.store_message[0] == 'erro'
+    assert not ctx.redirect
 
 
 def test_get_server_port(ctx):
     """ Test the ViewContext.get_server_port method. """
     assert ctx.get_server_port() == 7777
 
 
@@ -384,17 +389,18 @@
     regexp = base_address + parameters
     matches = re.match(regexp, url)
     assert matches is not None
     expected = ['appliname=dummy_appli', 'node=10.0.0.4', 'period=10', 'strategy=CONFIG']
     assert sorted(matches.groups()) == expected
 
 
-def test_message(ctx):
-    """ Test the ViewContext.message method. """
-    ctx.message(('warning', 'not as expected'))
+def test_fire_message(ctx):
+    """ Test the ViewContext.fire_message method. """
+    ctx.store_message = ('warning', 'not as expected')
+    ctx.fire_message()
     # result depends on dict contents so ordering is unreliable
     url = ctx.http_context.response['headers']['Location']
     base_address = r'http://10.0.0.1:7777/index.html\?'
     parameters = r'&'.join([url_attr_template for _ in range(3)])
     regexp = base_address + parameters
     matches = re.match(regexp, url)
     assert matches is not None
```

### Comparing `supvisors-0.8/supvisors/tests/test_viewhandler.py` & `supvisors-0.9/supvisors/tests/test_viewhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,20 @@
     assert mocked_autorefresh.attrib['class'] == 'button'
     assert handler.view_ctx.format_url.call_args_list == [call('', SUPVISORS_PAGE),
                                                           call('', 'dummy.html', action='refresh'),
                                                           call('', 'dummy.html', action='refresh', auto=True)]
     assert mocked_msg.call_args_list == [call(mocked_root, 'severe', 'a message')]
 
 
+def test_write_navigation(handler):
+    """ Test the write_navigation method. """
+    with pytest.raises(NotImplementedError):
+        handler.write_navigation(Mock())
+
+
 def test_write_nav(mocker, handler):
     """ Test the write_nav method. """
     mocked_appli = mocker.patch('supvisors.viewhandler.ViewHandler.write_nav_applications')
     mocked_nodes = mocker.patch('supvisors.viewhandler.ViewHandler.write_nav_nodes')
     handler.write_nav('root', 'address', 'appli')
     assert mocked_nodes.call_args_list == [call('root', 'address')]
     assert mocked_appli.call_args_list == [call('root', 'appli')]
@@ -368,14 +374,20 @@
     assert href_elt.attrib['class'] == 'on'
     assert handler.view_ctx.format_url.call_args_list == [call('', 'application.html', appliname='dummy_appli',
                                                                strategy='LESS_LOADED')]
     assert href_elt.attributes.call_args_list == [call(href='an url')]
     assert href_elt.content.call_args_list == [call('dummy_appli')]
 
 
+def test_write_header(handler):
+    """ Test the write_header method. """
+    with pytest.raises(NotImplementedError):
+        handler.write_header(Mock())
+
+
 def test_write_periods(handler):
     """ Test the write_periods method. """
     # patch the meld elements
     href_elt = Mock(attrib={'class': ''})
     period_elt = Mock(attrib={}, **{'findmeld.return_value': href_elt})
     mocked_mid = Mock(**{'repeat.return_value': [(period_elt, 5)]})
     mocked_root = Mock(**{'findmeld.return_value': mocked_mid})
@@ -402,14 +414,20 @@
     assert period_elt.findmeld.call_args_list == [call('period_a_mid')]
     assert href_elt.attrib['class'] == ''
     assert handler.view_ctx.format_url.call_args_list == [call('', None, period=5)]
     assert href_elt.attributes.call_args_list == [call(href='an url')]
     assert href_elt.content.call_args_list == [call('5s')]
 
 
+def test_write_contents(handler):
+    """ Test the write_contents method. """
+    with pytest.raises(NotImplementedError):
+        handler.write_contents(Mock())
+
+
 def test_write_common_process_cpu(handler):
     """ Test the write_common_process_cpu method. """
     # patch the view context
     handler.view_ctx = Mock(parameters={PROCESS: 'dummy_proc'}, **{'format_url.return_value': 'an url'})
     # patch the meld elements
     cell_elt = Mock(attrib={'class': ''})
     tr_elt = Mock(attrib={}, **{'findmeld.return_value': cell_elt})
@@ -846,15 +864,21 @@
     handler.callback = None
     handler.make_callback = Mock(return_value=lambda: 'a message')
     assert handler.handle_action() == NOT_DONE_YET
     assert handler.make_callback.call_args_list == [call('dummy_proc', 'test')]
     handler.make_callback.reset_mock()
     assert not handler.handle_action()
     assert handler.make_callback.call_args_list == []
-    assert handler.view_ctx.message.call_args_list == [call(('info', 'a message'))]
+    assert handler.view_ctx.store_message == ('info', 'a message')
+
+
+def test_make_callback(handler):
+    """ Test the make_callback method. """
+    with pytest.raises(NotImplementedError):
+        handler.make_callback('dummy_namespec', 'dummy_action')
 
 
 def test_set_slope_class():
     """ Test the set_slope_class method. """
     elt = Mock(attrib={})
     # test with values around 0
     ViewHandler.set_slope_class(elt, 0)
```

### Comparing `supvisors-0.8/supvisors/tests/test_viewhostaddress.py` & `supvisors-0.9/supvisors/tests/test_viewhostaddress.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_viewimage.py` & `supvisors-0.9/supvisors/tests/test_viewimage.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_viewprocaddress.py` & `supvisors-0.9/supvisors/tests/test_viewprocaddress.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_viewsupstatus.py` & `supvisors-0.9/supvisors/tests/test_viewsupstatus.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_viewsupvisors.py` & `supvisors-0.9/supvisors/tests/test_viewsupvisors.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tests/test_webutils.py` & `supvisors-0.9/supvisors/tests/test_webutils.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/tools/breed.py` & `supvisors-0.9/supvisors/tools/breed.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,164 +19,191 @@
 
 import os
 import sys
 
 from argparse import Action, ArgumentParser
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Dict, Mapping, Sequence, Tuple
+from typing import Dict, Mapping, List, Tuple
 
-# annotation types
-TemplateGroups = Mapping[str, int]
-TemplatePrograms = Mapping[str, Sequence[str]]
-SectionConfigMap = Dict[str, ConfigParser]
-FileConfigMap = Dict[Path, ConfigParser]
-
-# verbosity global variable
-VERBOSE = False
-
-
-def read_config_files(file_pattern: str) -> Tuple[SectionConfigMap, FileConfigMap]:
-    """ Get all configuration files and create a parser for each of them.
-
-    :param file_pattern: the filepath pattern to search for config files from the current working directory
-    :return: the parsers grouped by section names and by file names
-    """
-    parser_map, parser_files = {}, {}
-    for filename in Path('.').glob(file_pattern):
-        config = ConfigParser(interpolation=None)
-        config.read(filename)
-        parser_files[filename] = config
-        for section in config.sections():
-            parser_map[section] = config
-    return parser_map, parser_files
 
+def is_folder(arg_parser, arg):
+    """ Test if the argument is a folder.
 
-def write_config_files(dst_folder: str, parser_files: FileConfigMap) -> None:
-    """ Write the contents of the parsers in new config files.
-
-    :param dst_folder: the destination folder
-    :param parser_files: the parsers to write, identified by their original file name
-    :return: None
+    :param arg_parser: the argument parser
+    :param arg: the argument to test
+    :return: True if the argument is a folder
     """
-    for filename, config in parser_files.items():
-        filepath = os.path.join(dst_folder, filename)
-        if VERBOSE:
-            print('Writing file: {}'.format(filepath))
-        # create path if it doesn't exist
-        folder_name = os.path.dirname(filepath)
-        os.makedirs(folder_name, exist_ok=True)
-        # write new config file from parser
-        with open(filepath, 'w') as configfile:
-            config.write(configfile)
-
-
-def breed_groups(parsers, template_groups: TemplateGroups) -> TemplatePrograms:
-    """ Find template groups in config files and replace them by X versions of the group.
-    Return the template programs that have to be multiplied.
-
-    :param parsers: all the config parsers found
-    :param template_groups: the template groups
-    :return: the template programs
-    """
-    template_programs = {}
-    for group, cardinality in template_groups.items():
-        if group in parsers:
-            config = parsers[group]
-            programs = config[group]['programs'].split(',')
-            # duplicate and update <cardinality> versions of the group
-            for idx in range(1, cardinality + 1):
-                new_section = group + '_%02d' % idx
-                new_programs = [program + '_%02d' % idx for program in programs]
-                config[new_section] = {'programs': ','.join(new_programs)}
-                if VERBOSE:
-                    print('New [{}]'.format(new_section))
-                    print('\tprograms={}'.format(','.join(new_programs)))
-                for program in programs:
-                    template_programs.setdefault('program:' + program, []).append(program + '_%02d' % idx)
-            # remove template
-            del config[group]
-    return template_programs
-
-
-def breed_programs(parsers, template_programs: TemplatePrograms) -> None:
-    """ Find template programs in config files and replace them by X versions of the program.
-
-    :param parsers: all the config parsers found
-    :param template_programs: the template programs
-    :return: None
-    """
-    for program, new_programs in template_programs.items():
-        if program in parsers:
-            config = parsers[program]
-            # duplicate and update X versions of the program
-            # at the end, remove template
-            for new_program in new_programs:
-                # copy template section to new_section
-                new_section = 'program:' + new_program
-                config[new_section] = config[program]
-            # remove template
-            del config[program]
+    if not os.path.isdir(arg):
+        arg_parser.error('The folder "%s" does not exist' % arg)
+    return arg
 
 
 class KeyValue(Action):
+    """ Simple action to manage key / value pairs. """
+
+    def __call__(self, arg_parser, namespace, values, option_string=None) -> None:
+        """ Check the format and store key/value pairs found from values.
 
-    def __call__(self, arg_parser, namespace, values, option_string=None):
+        :param arg_parser: the argument parser
+        :param namespace: the destination storage in argument parser
+        :param values: the argument to process
+        :param option_string: not used. kept for signature
+        :return: None
+        """
         setattr(namespace, self.dest, {})
         for value in values:
             if '=' not in value:
                 arg_parser.error('breed format must be: key=value')
             key, value = value.split('=')
             if not value.isdigit():
                 arg_parser.error('breed value must be an integer')
-            getattr(namespace, self.dest)[key] = int(value)
+            int_value = int(value)
+            if int_value < 1:
+                arg_parser.error('breed value must be strictly positive')
+            getattr(namespace, self.dest)[key] = int_value
 
 
-def is_folder(arg_parser, arg):
-    if not os.path.isdir(arg):
-        arg_parser.error('The folder "%s" does not exist' % arg)
-    return arg
-
-
-if __name__ == '__main__':
-    """ Create X definitions of group and programs based on group/program template.
+class Breed(object):
+    """ Create X group definitions based on group template.
     This is typically useful when an application could be started X times.
     As there's no concept of homogeneous group in Supervisor, this script duplicates X times the definition of a group
-    and its related programs and removes the original definition.
+    and removes the original definition.
     The resulting configuration files are written to a separate folder.
     """
-    # get arguments
+
+    # annotation types
+    TemplateGroups = Mapping[str, int]
+    SectionConfigMap = Dict[str, ConfigParser]
+    FileConfigMap = Dict[Path, ConfigParser]
+
+    # verbosity global variable
+    VERBOSE = False
+
+    def __init__(self, verbose: bool = False):
+        """ Initialization of the attributes. """
+        self.verbose = verbose
+        self.config_map: Breed.SectionConfigMap = {}
+        self.config_files: Breed.FileConfigMap = {}
+
+    def read_config_files(self, file_pattern: str):
+        """ Get all configuration files and create a parser for each of them.
+
+        :param file_pattern: the filepath pattern to search for config files from the current working directory
+        :return: None
+        """
+        for filename in Path('.').glob(file_pattern):
+            config = ConfigParser(interpolation=None)
+            config.read(filename)
+            self.config_files[filename] = config
+            for section in config.sections():
+                if section.startswith('group:'):
+                    self.config_map[section] = config
+        if self.verbose:
+            print('Configuration files found:\n\t{}'.format('\n\t'.join([str(file) for file in self.config_files])))
+            print('Template group elements found:\n\t{}'.format('\n\t'.join(self.config_map.keys())))
+
+    def write_config_files(self, dst_folder: str) -> None:
+        """ Write the contents of the parsers in new config files.
+
+        :param dst_folder: the destination folder
+        :return: None
+        """
+        for filename, config in self.config_files.items():
+            if config.sections():
+                filepath = os.path.join(dst_folder, filename)
+                if self.verbose:
+                    print('Writing file: {}'.format(filepath))
+                # create path if it doesn't exist
+                folder_name = os.path.dirname(filepath)
+                os.makedirs(folder_name, exist_ok=True)
+                # write new config file from parser
+                with open(filepath, 'w') as configfile:
+                    config.write(configfile)
+            else:
+                if self.verbose:
+                    print('Empty sections for file: {}'.format(filename))
+
+    def breed_groups(self, template_groups: TemplateGroups, new_files: bool) -> None:
+        """ Find template groups in config files and replace them by X versions of the group.
+
+        :param template_groups: the template groups
+        :param new_files: True if new configuration files required
+        :return: None
+        """
+        for group, cardinality in template_groups.items():
+            if group in self.config_map:
+                ref_group_config = self.config_map[group]
+                programs = ref_group_config[group]['programs']
+                # duplicate and update <cardinality> versions of the group
+                for idx in range(1, cardinality + 1):
+                    new_section = group + '_%02d' % idx
+                    # if new files are requested, add the new configuration in a new parser
+                    if new_files:
+                        group_config = self.create_new_parser(new_section, ref_group_config)
+                    else:
+                        group_config = ref_group_config
+                    group_config[new_section] = {'programs': programs}
+                    if self.verbose:
+                        print('New [{}]'.format(new_section))
+                # remove template
+                del ref_group_config[group]
+
+    def create_new_parser(self, section: str, ref_config: ConfigParser) -> ConfigParser:
+        """ Create a new ConfigParser whose dirpath is similar to reference.
+        The new instance is stored in internal maps.
+
+        :param section: the config section to store in a new ConfigParser
+        :param ref_config: the reference ConfigParser
+        :return: the new ConfigParser
+        """
+        config = ConfigParser(interpolation=None)
+        self.config_map[section] = config
+        # add a new file reference
+        ref_filename = next(filename for filename, config in self.config_files.items()
+                            if config is ref_config)
+        filename = Path(os.path.join(os.path.dirname(ref_filename), '_'.join(section.split(':')) + '.ini'))
+        self.config_files[filename] = config
+        if self.verbose:
+            print('New File: {}'.format(filename))
+        return config
+
+
+def parse_args(args):
+    """ Parse arguments got from the command line.
+
+    :param args: the command line arguments
+    :return: the parsed arguments
+    """
     parser = ArgumentParser(description='Duplicate the application definitions')
     parser.add_argument('-t', '--template', type=lambda x: is_folder(parser, x), required=True,
                         help='the template folder')
     parser.add_argument('-p', '--pattern', type=str, default='**/*.ini',
                         help='the search pattern from the template folder')
     parser.add_argument('-d', '--destination', type=str, required=True, help='the destination folder')
-    parser.add_argument('-b', '--breed', metavar='app=nb', action=KeyValue, nargs='+',
+    parser.add_argument('-b', '--breed', metavar='app=nb', action=KeyValue, nargs='+', required=True,
                         help='the applications to breed')
+    parser.add_argument('-x', '--extra', action='store_true', help='create new files')
     parser.add_argument('-v', '--verbose', action='store_true', help='activate logs')
-    args = parser.parse_args()
-    # set verbosity global variable
-    VERBOSE = args.verbose
-    if VERBOSE:
+    return parser.parse_args(args)
+
+
+def main():
+    args = parse_args(sys.argv[1:])
+    if args.verbose:
         print('ArgumentParser: {}'.format(args))
     # change working directory
     ref_directory = os.getcwd()
     os.chdir(args.template)
+    # create the Breed instance
+    breed = Breed(args.verbose)
     # get one parser per template file
-    config_map, config_files = read_config_files(args.pattern)
-    if VERBOSE:
-        print('Configuration files found:\n\t{}'
-              .format('\n\t'.join([str(file) for file in config_files])))
-        print('Template elements found:\n\t{}'
-              .format('\n\t'.join(config_map.keys())))
-    if not len(config_files):
+    breed.read_config_files(args.pattern)
+    if not len(breed.config_files):
         print('No configuration files found')
         sys.exit(0)
     # update all groups configurations
     group_breed = {'group:' + key: value for key, value in args.breed.items()}
-    program_breed = breed_groups(config_map, group_breed)
-    # update program configurations found in groups
-    breed_programs(config_map, program_breed)
+    breed.breed_groups(group_breed, args.extra)
     # back to previous directory and write files
     os.chdir(ref_directory)
-    write_config_files(args.destination, config_files)
+    breed.write_config_files(args.destination)
```

### Comparing `supvisors-0.8/supvisors/ui/css/button.css` & `supvisors-0.9/supvisors/ui/css/button.css`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/css/main_page.css` & `supvisors-0.9/supvisors/ui/css/main_page.css`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/css/menu.css` & `supvisors-0.9/supvisors/ui/css/menu.css`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/css/ui_style.css` & `supvisors-0.9/supvisors/ui/css/ui_style.css`

 * *Files 1% similar despite different names*

```diff
@@ -481,15 +481,15 @@
 
 .expected {
     font-style: italic;
 }
 
 /* fix some column width (button actions have a fixed content) */
 table .name {
-  width: 180px;
+  width: 200px;
 }
 
 table .state {
     width: 50px;
 }
 
 table .desc {
```

### Comparing `supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.eot` & `supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.eot`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.svg` & `supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.svg`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.ttf` & `supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.ttf`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.woff` & `supvisors-0.9/supvisors/ui/fonts/Kingthings_Calligraphica_2-webfont.woff`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/auto_reload_30.png` & `supvisors-0.9/supvisors/ui/img/auto_reload_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/erro_20.png` & `supvisors-0.9/supvisors/ui/img/erro_20.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/info_20.png` & `supvisors-0.9/supvisors/ui/img/info_20.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/leds_empty_30.png` & `supvisors-0.9/supvisors/ui/img/leds_empty_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/leds_green_30.png` & `supvisors-0.9/supvisors/ui/img/leds_green_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/leds_red_30.png` & `supvisors-0.9/supvisors/ui/img/leds_red_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/leds_yellow_30.png` & `supvisors-0.9/supvisors/ui/img/leds_yellow_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/red_light_30.png` & `supvisors-0.9/supvisors/ui/img/red_light_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/reload_30.png` & `supvisors-0.9/supvisors/ui/img/reload_30.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/restart_40.png` & `supvisors-0.9/supvisors/ui/img/restart_40.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/shutdown_40.png` & `supvisors-0.9/supvisors/ui/img/shutdown_40.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/start_40.png` & `supvisors-0.9/supvisors/ui/img/start_40.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/stop_40.png` & `supvisors-0.9/supvisors/ui/img/stop_40.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/img/warn_20.png` & `supvisors-0.9/supvisors/ui/img/warn_20.png`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/application.html` & `supvisors-0.9/supvisors/ui/application.html`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/hostaddress.html` & `supvisors-0.9/supvisors/ui/hostaddress.html`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/index.html` & `supvisors-0.9/supvisors/ui/index.html`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ui/procaddress.html` & `supvisors-0.9/supvisors/ui/procaddress.html`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/address.py` & `supvisors-0.9/supvisors/address.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/addressmapper.py` & `supvisors-0.9/supvisors/addressmapper.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/application.py` & `supvisors-0.9/supvisors/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ======================================================================
 
+import re
+
 from typing import Any, Dict, List, Sequence
 
 from supervisor.loggers import Logger
 from supervisor.states import ProcessStates
 
 from .process import ProcessStatus
 from .ttypes import (ApplicationStates, NameList, Payload, StartingStrategies,
@@ -30,37 +32,109 @@
 class ApplicationRules(object):
     """ Definition of the rules for starting an application, iaw rules file.
 
     Attributes are:
         - managed: set to True when application rules are found from the rules file;
         - distributed: set to False if all processes must be running on the same node;
         - node_names: the nodes where the application can be started (all by default) if not distributed,
+        - hash_node_names: when # rule is used, the application can be started on one of these nodes (to be resolved),
         - start_sequence: defines the order of this application when starting all the applications
           in the DEPLOYMENT state (0 means: no automatic start);
         - stop_sequence: defines the order of this application when stopping all the applications
           (0 means: immediate stop);
         - starting_strategy: defines the strategy to apply when choosing the node where the process shall be started
           during the starting of the application;
         - starting_failure_strategy: defines the strategy to apply when a required process cannot be started
           during the starting of the application;
         - running_failure_strategy: defines the default strategy to apply when a required process crashes
           when the application is running.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, supvisors: Any) -> None:
         """ Initialization of the attributes. """
+        # keep a reference to the Supvisors global structure
+        self.supvisors = supvisors
+        self.logger: Logger = supvisors.logger
+        # attributes
         self.managed: bool = False
         self.distributed: bool = True
         self.node_names: NameList = ['*']
+        self.hash_node_names: NameList = []
         self.start_sequence: int = 0
-        self.stop_sequence: int = 0
+        self.stop_sequence: int = -1
         self.starting_strategy: StartingStrategies = StartingStrategies.CONFIG
         self.starting_failure_strategy: StartingFailureStrategies = StartingFailureStrategies.ABORT
         self.running_failure_strategy: RunningFailureStrategies = RunningFailureStrategies.CONTINUE
 
+    def check_stop_sequence(self, application_name: str) -> None:
+        """ Check the stop_sequence value.
+        If stop_sequence hasn't been set from the rules file, use the same value as start_sequence.
+
+        :param namespec: the namespec of the program considered.
+        :return: None
+        """
+        if self.stop_sequence < 0:
+            self.logger.trace('ApplicationRules.check_stop_sequence: {} - set stop_sequence to {} '
+                              .format(application_name, self.start_sequence))
+            self.stop_sequence = self.start_sequence
+
+    def check_hash_nodes(self, application_name: str) -> None:
+        """ When a '#' is set in application rules, an association has to be done between the 'index' of the application
+        and the index of the node in the applicable node list.
+        Unlike programs, there is no unquestionable index that Supvisors could get because Supervisor does not support
+        homogeneous applications. It thus has to be a convention.
+        The chosen covenant is that the application_name MUST match r'[-_]\d+$'. The first index name is 1.
+
+        hash_node_names is expected to contain:
+            - either ['*'] when all nodes are applicable
+            - or any subset of these nodes.
+
+        :param application_name: the name of the application considered.
+        :return: None
+        """
+        error = True
+        result = re.match(r'.*[-_](\d+)$', application_name)
+        if not result:
+            self.logger.error('ApplicationRules.check_hash_nodes: application_name={} incompatible with the use of #'
+                              .format(application_name))
+        else:
+            appnumber = int(result.group(1)) - 1
+            if appnumber < 0:
+                self.logger.error('ApplicationRules.check_hash_nodes: index of application_name={} must be > 0'
+                                  .format(application_name))
+            else:
+                self.logger.debug('ApplicationRules.check_hash_nodes: application_name={} appnumber={}'
+                                  .format(application_name, appnumber))
+                if '*' in self.hash_node_names:
+                    # all nodes defined in the supvisors section of the supervisor configuration file are applicable
+                    ref_node_names = self.supvisors.address_mapper.node_names
+                else:
+                    # the subset of applicable nodes is the hash_node_names
+                    ref_node_names = self.hash_node_names
+                if appnumber < len(ref_node_names):
+                    self.node_names = [ref_node_names[appnumber]]
+                    error = False
+                else:
+                    self.logger.error('ApplicationRules.check_hash_nodes: application={} has no applicable node'
+                                      .format(application_name))
+        if error:
+            self.logger.warn('ApplicationRules.check_hash_nodes: application={} start_sequence reset'
+                             .format(application_name))
+            self.start_sequence = 0
+
+    def check_dependencies(self, application_name: str) -> None:
+        """ Update rules after they have been read from the rules file.
+
+        :param application_name: the name of the application considered.
+        :return: None
+        """
+        self.check_stop_sequence(application_name)
+        if self.hash_node_names:
+            self.check_hash_nodes(application_name)
+
     def __str__(self) -> str:
         """ Get the application rules as string.
 
         :return: the printable application rules
         """
         return 'managed={} distributed={} node_names={} start_sequence={} stop_sequence={} starting_strategy={}'\
                ' starting_failure_strategy={} running_failure_strategy={}' \
```

### Comparing `supvisors-0.8/supvisors/commander.py` & `supvisors-0.9/supvisors/commander.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """ Wrapper of the process to include data only used here.
 
     Attributes are:
         - process: the process wrapped,
         - node_name: the node to which the command is requested,
         - request_time: the date when the command is requested,
         - strategy: the strategy used to start the process if applicable,
-        - distributed: set to False if the process belongs to an application that cannot de distributed,
+        - distributed: set to False if the process belongs to an application that cannot be distributed,
         - ignore_wait_exit: used to command a process out of its application starting sequence,
         - extra_args: additional arguments to the command line.
     """
     TIMEOUT = 10
 
     def __init__(self, process: ProcessStatus, strategy: StartingStrategies = None) -> None:
         """ Initialization of the attributes.
@@ -110,14 +110,16 @@
         # keep a reference of the Supvisors data
         self.supvisors = supvisors
         self.logger = supvisors.logger
         # attributes
         self.planned_sequence: Commander.PlannedSequence = {}
         self.planned_jobs: Commander.PlannedJobs = {}
         self.current_jobs: Commander.CurrentJobs = {}
+        # pickup logic
+        self.pickup_logic = None
 
     def in_progress(self) -> bool:
         """ Return True if there are jobs planned or in progress.
 
         :return: the progress status
         """
         self.logger.trace('Commander.in_progress: planned_sequence={} planned_jobs={} current_jobs={}'
@@ -187,22 +189,22 @@
         """ Triggers the next sequence from the jobs planned (start or stop).
 
         :return: None
         """
         self.logger.info('Commander.trigger_jobs: planned_sequence={}'.format(self.printable_planned_sequence()))
         # pop lower sequence from planned_sequence
         while self.planned_sequence and not self.planned_jobs and not self.current_jobs:
-            min_sequence = min(self.planned_sequence.keys())
-            self.planned_jobs = self.planned_sequence.pop(min_sequence)
-            self.logger.debug('Commander.trigger_jobs: min_sequence={} planned_jobs={}'
-                              .format(min_sequence, self.printable_planned_jobs()))
+            sequence = self.pickup_logic(self.planned_sequence.keys())
+            self.planned_jobs = self.planned_sequence.pop(sequence)
+            self.logger.debug('Commander.trigger_jobs: sequence={} planned_jobs={}'
+                              .format(sequence, self.printable_planned_jobs()))
             # iterate on copy to avoid problems with key deletions
             for application_name in list(self.planned_jobs.keys()):
                 self.logger.info('Commander.trigger_jobs: triggering sequence {} - application_name={}'
-                                 .format(min_sequence, application_name))
+                                 .format(sequence, application_name))
                 self.prepare_application_jobs(application_name)
                 self.process_application_jobs(application_name)
 
     def prepare_application_jobs(self, application_name, application: ApplicationStatus = None) -> None:
         """ Prepare the ProcessCommand instances linked to application planned jobs.
         Implemented in Starter only.
 
@@ -219,19 +221,19 @@
         """
         if application_name in self.planned_jobs:
             sequence = self.planned_jobs[application_name]
             self.current_jobs[application_name] = jobs = []
             # loop until there is something to do in sequence
             while sequence and not jobs and application_name in self.planned_jobs:
                 # pop lower group from sequence
-                min_sequence = min(sequence.keys())
-                group = sequence.pop(min_sequence)
+                app_sequence = self.pickup_logic(sequence.keys())
+                group = sequence.pop(app_sequence)
                 self.logger.debug('Commander.process_application_jobs: application_name={}'
-                                  ' - next group: min_sequence={} group={}'
-                                  .format(application_name, min_sequence, self.printable_command_list(group)))
+                                  ' - next group: app_sequence={} group={}'
+                                  .format(application_name, app_sequence, self.printable_command_list(group)))
                 for command in group:
                     self.logger.debug('Commander.process_application_jobs: {} - state={}'
                                       .format(command.process.namespec, command.process.state_string()))
                     self.process_job(command, jobs)
             self.logger.debug('Commander.process_application_jobs: current_jobs={}'
                               .format(self.printable_current_jobs()))
             # if nothing in progress when exiting the loop, delete application entry in current_jobs
@@ -343,16 +345,18 @@
 
     def __init__(self, supvisors: Any) -> None:
         """ Initialization of the attributes.
 
         :param supvisors: the global Supvisors structure.
         """
         super().__init__(supvisors)
+        # pick jobs from the planned sequence using the lowest sequence number
+        self.pickup_logic = min
         # attributes
-        self.application_stop_requests = []
+        self.application_stop_requests: List[str] = []
 
     def abort(self) -> None:
         """ Abort all planned current jobs.
         Do not erase current_jobs. Wait for their completion.
 
         :return: None
         """
@@ -673,21 +677,30 @@
                         load_request_map.setdefault(command.node_name, []).append(command.process.rules.expected_load)
         return {node_name: sum(load_list) for node_name, load_list in load_request_map.items() if node_name}
 
 
 class Stopper(Commander):
     """ Class handling the stopping of processes and applications. """
 
+    def __init__(self, supvisors: Any) -> None:
+        """ Initialization of the attributes.
+
+        :param supvisors: the global Supvisors structure.
+        """
+        super().__init__(supvisors)
+        # pick jobs from the planned sequence using the greatest sequence number
+        self.pickup_logic = max
+
     def stop_applications(self):
         """ Plan and start the necessary jobs to stop all the applications having a stop_sequence. """
         self.logger.info('Stopper.stop_applications: stop all applications')
         # stopping initialization: push program list in jobs list
         for application in self.supvisors.context.applications.values():
             # do not check the application state are running processes may be excluded in the evaluation
-            if application.has_running_processes() and application.rules.stop_sequence >= 0:
+            if application.has_running_processes():
                 self.store_application_stop_sequence(application)
         self.logger.debug('Stopper.stop_applications: planned_sequence={}'.format(self.printable_planned_sequence()))
         # start work
         self.trigger_jobs()
 
     def stop_application(self, application: ApplicationStatus) -> bool:
         """ Plan and start the necessary jobs to stop the application in parameter. """
```

### Comparing `supvisors-0.8/supvisors/context.py` & `supvisors-0.9/supvisors/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         :param application_name: the name of the application
         :return: the application stored in the Supvisors context
         """
         # find existing application
         application = self.applications.get(application_name)
         if not application:
             # load rules from rules file
-            rules = ApplicationRules()
+            rules = ApplicationRules(self.supvisors)
             if self.supvisors.parser:
                 # apply default starting strategy from options
                 rules.starting_strategy = self.supvisors.options.starting_strategy
                 self.supvisors.parser.load_application_rules(application_name, rules)
                 self.logger.debug('Context.setdefault_application: application={} rules={}'
                                   .format(application_name, rules))
             # create new instance
```

### Comparing `supvisors-0.8/supvisors/infosource.py` & `supvisors-0.9/supvisors/infosource.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/initializer.py` & `supvisors-0.9/supvisors/initializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,46 +16,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ======================================================================
 
 from typing import Any
 
 from supervisor import loggers
-from supervisor.datatypes import Automatic
 from supervisor.xmlrpc import Faults, RPCError
 
 from .addressmapper import AddressMapper
 from .commander import Starter, Stopper
 from .context import Context
 from .infosource import SupervisordSource
 from .listener import SupervisorListener
-from .options import SupvisorsServerOptions
+from .options import *
 from .sparser import Parser
 from .statemachine import FiniteStateMachine
 from .statscompiler import StatisticsCompiler
 from .strategy import RunningFailureHandler
 
 
 class Supvisors(object):
     """ The Supvisors class used as a global structure passed to most Supvisors objects. """
 
     # logger output (use ';' as separator as easier to cut)
     LOGGER_FORMAT = '%(asctime)s;%(levelname)s;%(message)s\n'
 
-    def __init__(self, supervisord: Any) -> None:
+    def __init__(self, supervisord: Any, **config) -> None:
         """ Instantiation of all the Supvisors objects.
 
         :param supervisord: the Supervisor global structure
         """
         # declare zmq context (will be created in listener)
         self.zmq = None
         # get options from config file
+        self.options = SupvisorsOptions(**config)
         server_options = SupvisorsServerOptions()
         server_options.realize()
-        self.options = server_options.supvisors_options
+        self.options.procnumbers = server_options.procnumbers
         # create logger
         self.logger = self.create_logger(supervisord)
         # configure supervisor info source
         self.info_source = SupervisordSource(supervisord, self.logger)
         # set addresses and check local address
         self.address_mapper = AddressMapper(self.logger)
         self.address_mapper.node_names = self.options.address_list
@@ -73,16 +73,15 @@
         self.failure_handler = RunningFailureHandler(self)
         # create state machine
         self.fsm = FiniteStateMachine(self)
         # check parsing
         try:
             self.parser = Parser(self)
         except Exception as exc:
-            self.logger.warn('Supvisors.__init__: cannot parse rules file: {} - {}'
-                             .format(self.options.rules_file, exc))
+            self.logger.warn('Supvisors: cannot parse rules file: {} - {}'.format(self.options.rules_file, exc))
             self.parser = None
         # create event subscriber
         self.listener = SupervisorListener(self)
 
     def create_logger(self, supervisord):
         """ Create the logger that will be used in Supvisors.
         If logfile is not set or set to AUTO, Supvisors will use Supervisor logger.
```

### Comparing `supvisors-0.8/supvisors/listener.py` & `supvisors-0.9/supvisors/listener.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/mainloop.py` & `supvisors-0.9/supvisors/mainloop.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/options.py` & `supvisors-0.9/supvisors/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,118 +48,64 @@
         - starting_strategy: strategy used to start processes on addresses,
         - stats_periods: list of periods for which the statistics will be provided in the Supvisors web page,
         - stats_histo: depth of statistics history,
         - logfile: absolute or relative path of the Supvisors log file,
         - logfile_maxbytes: maximum size of the Supvisors log file,
         - logfile_backups: number of Supvisors backup log files,
         - loglevel: logging level,
-        - procnumbers: a dictionary giving the number of the program in a homogeneous group.
+        - procnumbers: a dictionary giving the number of the program in a homogeneous program group.
     """
 
     SYNCHRO_TIMEOUT_MIN = 15
+    SYNCHRO_TIMEOUT_MAX = 1200
 
-    _Options = ['address_list', 'rules_file', 'internal_port', 'event_port', 'auto_fence',
-                'synchro_timeout', 'force_synchro_if',
-                'conciliation_strategy', 'starting_strategy',
-                'stats_periods', 'stats_histo', 'stats_irix_mode',
-                'logfile', 'logfile_maxbytes', 'logfile_backups', 'loglevel']
+    def __init__(self, **config):
+        """ Initialization of the attributes.
 
-    def __init__(self):
-        """ Initialization of the attributes. """
-        # option list
-        for option in SupvisorsOptions._Options:
-            setattr(self, option, None)
-        # second parse
+        :param procnumbers: the num program numbers
+        :param config: the configuration provided by Supervisor from the [rpcinterface:supvisors] section
+        """
+        # get values from config
+        self.address_list = filter(None, list_of_strings(config.get('address_list', gethostname())))
+        self.address_list = list(OrderedDict.fromkeys(self.address_list))
+        self.rules_file = config.get('rules_file', None)
+        if self.rules_file:
+            self.rules_file = existing_dirpath(self.rules_file)
+        self.internal_port = self.to_port_num(config.get('internal_port', '65001'))
+        self.event_port = self.to_port_num(config.get('event_port', '65002'))
+        self.auto_fence = boolean(config.get('auto_fence', 'false'))
+        self.synchro_timeout = self.to_timeout(config.get('synchro_timeout', str(self.SYNCHRO_TIMEOUT_MIN)))
+        self.force_synchro_if = filter(None, list_of_strings(config.get('force_synchro_if', None)))
+        self.force_synchro_if = {node for node in self.force_synchro_if if node in self.address_list}
+        self.conciliation_strategy = self.to_conciliation_strategy(config.get('conciliation_strategy', 'USER'))
+        self.starting_strategy = self.to_starting_strategy(config.get('starting_strategy', 'CONFIG'))
+        # configure statistics
+        self.stats_periods = self.to_periods(list_of_strings(config.get('stats_periods', '10')))
+        self.stats_histo = self.to_histo(config.get('stats_histo', 200))
+        self.stats_irix_mode = boolean(config.get('stats_irix_mode', 'false'))
+        # configure logger
+        self.logfile = logfile_name(config.get('logfile', Automatic))
+        self.logfile_maxbytes = byte_size(config.get('logfile_maxbytes', '50MB'))
+        self.logfile_backups = integer(config.get('logfile_backups', 10))
+        self.loglevel = logging_level(config.get('loglevel', 'info'))
+        # attribute got from SupvisorsServerOptions
         self.procnumbers = {}
 
     def __str__(self):
         """ Contents as string. """
-        return ('address_list={} rules_file={} internal_port={} event_port={} auto_fence={} '
-                'synchro_timeout={} force_synchro_if={} conciliation_strategy={} '
-                'starting_strategy={} stats_periods={} stats_histo={} '
-                'stats_irix_mode={} logfile={} logfile_maxbytes={} '
-                'logfile_backups={} loglevel={}'.format(self.address_list, self.rules_file,
-                                                        self.internal_port, self.event_port, self.auto_fence,
-                                                        self.synchro_timeout, self.force_synchro_if,
-                                                        self.conciliation_strategy, self.starting_strategy,
-                                                        self.stats_periods, self.stats_histo, self.stats_irix_mode,
-                                                        self.logfile, self.logfile_maxbytes, self.logfile_backups,
-                                                        self.loglevel))
-
-
-class SupvisorsServerOptions(ServerOptions):
-    """ Class used to parse the options of the 'supvisors' section in the
-    supervisor configuration file.
-
-    Attributes are:
-        - supvisors_options: the instance holding all Supvisors options,
-        - _Section: constant for the name of the Supvisors section in the Supervisor configuration file.
-    """
-
-    # Name of the Supvisors section in the Supervisor configuration file
-    _Section = 'supvisors'
-
-    def __init__(self):
-        """ Initialization of the attributes. """
-        ServerOptions.__init__(self)
-        self.supvisors_options = SupvisorsOptions()
-
-    def _processes_from_section(self, parser, section, group_name, klass=None):
-        """ This method is overridden to: store the program number of a homogeneous program.
-
-        This is originally used in Supervisor to set the real program name from the format defined in the ini file.
-        However, Supervisor does not keep this information in its internal structure.
-        """
-        # call super behaviour
-        programs = ServerOptions._processes_from_section(self, parser, section, group_name, klass)
-        # store the number of each program
-        for idx, program in enumerate(programs):
-            self.supvisors_options.procnumbers[program.name] = idx
-        # return original result
-        return programs
-
-    def server_configs_from_parser(self, parser):
-        """ The following has nothing to deal with Supervisor's server configurations.
-        It gets Supvisors configuration.
-        Supervisor's ServerOptions has not been designed to be specialized.
-        This method is overridden just to have an access point to the Supervisor parser.
-        """
-        configs = ServerOptions.server_configs_from_parser(self, parser)
-        # set section
-        if not parser.has_section(SupvisorsServerOptions._Section):
-            raise ValueError('.ini file ({}) does not include a [{}] section'
-                             .format(self.configfile, SupvisorsServerOptions._Section))
-        temp, parser.mysection = parser.mysection, SupvisorsServerOptions._Section
-        # get values
-        opt = self.supvisors_options
-        opt.address_list = filter(None, list_of_strings(parser.getdefault('address_list', gethostname())))
-        opt.address_list = list(OrderedDict.fromkeys(opt.address_list))
-        opt.rules_file = parser.getdefault('rules_file', None)
-        if opt.rules_file:
-            opt.rules_file = existing_dirpath(opt.rules_file)
-        opt.internal_port = self.to_port_num(parser.getdefault('internal_port', '65001'))
-        opt.event_port = self.to_port_num(parser.getdefault('event_port', '65002'))
-        opt.auto_fence = boolean(parser.getdefault('auto_fence', 'false'))
-        opt.synchro_timeout = self.to_timeout(parser.getdefault('synchro_timeout', str(opt.SYNCHRO_TIMEOUT_MIN)))
-        opt.force_synchro_if = filter(None, list_of_strings(parser.getdefault('force_synchro_if', None)))
-        opt.force_synchro_if = {node for node in opt.force_synchro_if if node in opt.address_list}
-        opt.conciliation_strategy = self.to_conciliation_strategy(parser.getdefault('conciliation_strategy', 'USER'))
-        opt.starting_strategy = self.to_starting_strategy(parser.getdefault('starting_strategy', 'CONFIG'))
-        # configure statistics
-        opt.stats_periods = self.to_periods(list_of_strings(parser.getdefault('stats_periods', '10')))
-        opt.stats_histo = self.to_histo(parser.getdefault('stats_histo', 200))
-        opt.stats_irix_mode = boolean(parser.getdefault('stats_irix_mode', 'false'))
-        # configure logger
-        opt.logfile = logfile_name(parser.getdefault('logfile', Automatic))
-        opt.logfile_maxbytes = byte_size(parser.getdefault('logfile_maxbytes', '50MB'))
-        opt.logfile_backups = integer(parser.getdefault('logfile_backups', 10))
-        opt.loglevel = logging_level(parser.getdefault('loglevel', 'info'))
-        # reset mysection and return original result
-        parser.mysection = temp
-        return configs
+        return "address_list={} rules_file={} internal_port={} event_port={} auto_fence={}"\
+               " synchro_timeout={} force_synchro_if={} conciliation_strategy={}"\
+               " starting_strategy={} stats_periods={} stats_histo={} stats_irix_mode={}"\
+               " logfile={} logfile_maxbytes={} logfile_backups={} loglevel={} procnumbers={}"\
+               .format(self.address_list, self.rules_file, self.internal_port, self.event_port, self.auto_fence,
+                       self.synchro_timeout, self.force_synchro_if,
+                       self.conciliation_strategy.name, self.starting_strategy.name,
+                       self.stats_periods, self.stats_histo, self.stats_irix_mode,
+                       self.logfile, self.logfile_maxbytes, self.logfile_backups, self.loglevel,
+                       self.procnumbers)
 
     # conversion utils (completion of supervisor.datatypes)
     @staticmethod
     def to_port_num(value: str) -> int:
         """ Convert a string into a port number, in [1;65535].
 
         :param value: the port number as a string
@@ -174,17 +120,18 @@
     def to_timeout(value: str) -> int:
         """ Convert a string into a timeout value, in [15;1200].
 
         :param value: the timeout as a string
         :return: the timeout as an integer
         """
         value = integer(value)
-        if 15 <= value <= 1200:
+        if SupvisorsOptions.SYNCHRO_TIMEOUT_MIN <= value <= SupvisorsOptions.SYNCHRO_TIMEOUT_MAX:
             return value
-        raise ValueError('invalid value for synchro_timeout: %d. expected in [15;1200] (seconds)' % value)
+        raise ValueError('invalid value for synchro_timeout: {}. expected in [{};{}] (seconds)'
+                         .format(value, SupvisorsOptions.SYNCHRO_TIMEOUT_MIN, SupvisorsOptions.SYNCHRO_TIMEOUT_MAX))
 
     @staticmethod
     def to_conciliation_strategy(value):
         """ Convert a string into a ConciliationStrategies enum. """
         try:
             strategy = ConciliationStrategies[value]
         except KeyError:
@@ -226,7 +173,30 @@
         :param value: the historic size as a string
         :return: the historic size as an integer
         """
         histo = integer(value)
         if 10 <= histo <= 1500:
             return histo
         raise ValueError('invalid value for stats_histo: {}. expected in [10;1500] (seconds)'.format(value))
+
+
+class SupvisorsServerOptions(ServerOptions):
+    """ Class used to parse the options of the 'supvisors' section in the supervisor configuration file. """
+
+    def __init__(self):
+        """ Initialization of the attributes. """
+        ServerOptions.__init__(self)
+        self.procnumbers = {}
+
+    def _processes_from_section(self, parser, section, group_name, klass=None):
+        """ This method is overridden to: store the program number of a homogeneous program.
+
+        This is originally used in Supervisor to set the real program name from the format defined in the ini file.
+        However, Supervisor does not keep this information in its internal structure.
+        """
+        # call super behaviour
+        programs = ServerOptions._processes_from_section(self, parser, section, group_name, klass)
+        # store the number of each program
+        for idx, program in enumerate(programs):
+            self.procnumbers[program.name] = idx
+        # return original result
+        return programs
```

### Comparing `supvisors-0.8/supvisors/plot.py` & `supvisors-0.9/supvisors/plot.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/plugin.py` & `supvisors-0.9/supvisors/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,10 +87,10 @@
     ServerOptions.cleanup_fds = cleanup_fds
     # patch inheritance of supervisor.web.StatusView
     # 2 reasons:
     #    * waiting for Supervisor#1273 to be fixed
     #    * to benefit from the commonalities done in supvisors.ViewHandler
     StatusView.__bases__ = (ViewHandler,)
     # store the Supvisors instance in supervisord instance to ensure persistence
-    supervisord.supvisors = Supvisors(supervisord)
+    supervisord.supvisors = Supvisors(supervisord, **config)
     # create and return handler
     return RPCInterface(supervisord.supvisors)
```

### Comparing `supvisors-0.8/supvisors/process.py` & `supvisors-0.9/supvisors/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 
     def __init__(self, supvisors: Any) -> None:
         """ Initialization of the attributes.
 
         :param supvisors: the global Supvisors structure.
         """
         # TODO: think about adding a period for tasks (period > startsecs / autorestart = False)
-        # keep a reference to the Supvisors data
+        # keep a reference to the Supvisors global structure
         self.supvisors = supvisors
         self.logger: Logger = supvisors.logger
         # attributes
         self.node_names: NameList = ['*']
         self.hash_node_names: NameList = []
         self.start_sequence: int = 0
-        self.stop_sequence: int = 0
+        self.stop_sequence: int = -1
         self.required: bool = False
         self.wait_exit: bool = False
         self.expected_load: int = 0
         self.running_failure_strategy: RunningFailureStrategies = RunningFailureStrategies.CONTINUE
 
     def check_start_sequence(self, namespec: str) -> None:
         """ ProcessRules having required=True MUST have start_sequence > 0,
@@ -72,14 +72,26 @@
         :return: None
         """
         if self.required and self.start_sequence == 0:
             self.logger.warn('ProcessRules.check_start_sequence: {} - required forced to False because '
                              'no start_sequence defined'.format(namespec))
             self.required = False
 
+    def check_stop_sequence(self, namespec: str) -> None:
+        """ Check the stop_sequence value.
+        If stop_sequence hasn't been set from the rules file, use the same value as start_sequence.
+
+        :param namespec: the namespec of the program considered.
+        :return: None
+        """
+        if self.stop_sequence < 0:
+            self.logger.trace('ProcessRules.check_stop_sequence: {} - set stop_sequence to {} '
+                              .format(namespec, self.start_sequence))
+            self.stop_sequence = self.start_sequence
+
     def check_autorestart(self, namespec: str) -> None:
         """ Disable autorestart when RunningFailureStrategies is related to applications.
         In these cases, Supvisors triggers behaviors that are different so supervisor.
 
         :param namespec: the namespec of the program considered.
         :return: None
         """
@@ -101,42 +113,48 @@
         In this case, rules.hash_addresses is expected to contain:
             - either ['*'] when all nodes are applicable
             - or any subset of these nodes.
 
         :param namespec: the namespec of the program considered.
         :return: None
         """
+        error = True
         _, process_name = split_namespec(namespec)
         try:
             procnumber = self.supvisors.options.procnumbers[process_name]
         except KeyError:
-            self.logger.error('ProcessStatus.check_hash_nodes: cannot apply "#" to unknown program={}'
+            self.logger.error('ProcessRules.check_hash_nodes: cannot apply "#" to unknown program={}'
                               .format(namespec))
         else:
-            self.logger.debug('ProcessStatus.check_hash_nodes: namespec={} procnumber={}'
+            self.logger.debug('ProcessRules.check_hash_nodes: namespec={} procnumber={}'
                               .format(namespec, procnumber))
             if '*' in self.hash_node_names:
                 # all nodes defined in the supvisors section of the supervisor configuration file are applicable
                 ref_node_names = self.supvisors.address_mapper.node_names
             else:
                 # the subset of applicable nodes is the second element of rule addresses
                 ref_node_names = self.hash_node_names
             if procnumber < len(ref_node_names):
                 self.node_names = [ref_node_names[procnumber]]
+                error = False
             else:
-                self.logger.warn('ProcessStatus.check_hash_nodes: program={} has no applicable node'.format(namespec))
-                self.start_sequence = 0
+                self.logger.error('ProcessRules.check_hash_nodes: program={} has no applicable node'.format(namespec))
+        if error:
+            self.logger.warn('ProcessRules.check_hash_nodes: program={} start_sequence reset'
+                             .format(namespec))
+            self.start_sequence = 0
 
     def check_dependencies(self, namespec: str) -> None:
         """ Update rules after they have been read from the rules file.
 
         :param namespec: the namespec of the program considered.
         :return: None
         """
         self.check_start_sequence(namespec)
+        self.check_stop_sequence(namespec)
         self.check_autorestart(namespec)
         if self.hash_node_names:
             self.check_hash_nodes(namespec)
 
     def __str__(self) -> str:
         """ Get the process rules as string.
```

### Comparing `supvisors-0.8/supvisors/rpcinterface.py` & `supvisors-0.9/supvisors/rpcinterface.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/rpcrequests.py` & `supvisors-0.9/supvisors/rpcrequests.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/rules.xsd` & `supvisors-0.9/supvisors/rules.xsd`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,14 @@
             <xs:element type="xs:byte" name="start_sequence" minOccurs="0"/>
             <xs:element type="xs:byte" name="stop_sequence" minOccurs="0"/>
             <xs:element type="StartingStrategy" name="starting_strategy" minOccurs="0"/>
             <xs:element type="StartingFailureStrategy" name="starting_failure_strategy" minOccurs="0"/>
             <xs:element type="RunningFailureStrategy" name="running_failure_strategy" minOccurs="0"/>
             <xs:choice minOccurs="0" maxOccurs="unbounded">
                 <xs:element type="ProgramModel" name="program"/>
-                <!-- obsolete -->
-                <xs:element type="ProgramModel" name="pattern"/>
             </xs:choice>
         </xs:sequence>
 	    <!-- no way to check one of the two is required unless XSD 1.1 is supported -->
         <xs:attribute type="xs:string" name="name"/>
         <xs:attribute type="xs:string" name="pattern"/>
     </xs:complexType>
     <xs:element name="root">
```

### Comparing `supvisors-0.8/supvisors/sparser.py` & `supvisors-0.9/supvisors/sparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,22 +63,14 @@
         self.logger.debug('Parser: found models {}'.format(self.models.keys()))
         # get application patterns
         app_elements = self.root.findall(".//application[@pattern]")
         self.application_patterns = {app_element.get('pattern'): app_element for app_element in app_elements}
         self.logger.debug('Parser: found application patterns {}'.format(self.application_patterns.keys()))
         # get program patterns
         self.program_patterns = {}
-        app_elements = self.root.findall(".//application/pattern[@name]/..")
-        for app_element in app_elements:
-            prg_elements = app_element.findall("./pattern[@name]")
-            self.program_patterns[app_element] = {prg_element.get('name'): prg_element for prg_element in prg_elements}
-        if self.program_patterns:
-            self.logger.warn('Parser: usage of pattern elements is deprecated -'
-                             ' please convert {} to program elements with pattern attribute.'
-                             .format(self.printable_program_patterns()))
         app_elements = self.root.findall(".//application/program[@pattern]/..")
         for app_element in app_elements:
             prg_elements = app_element.findall("./program[@pattern]")
             prg_patterns = self.program_patterns.setdefault(app_element, {})
             prg_patterns.update({prg_element.get('pattern'): prg_element for prg_element in prg_elements})
         self.logger.debug('Parser: found program patterns {}'.format(self.printable_program_patterns()))
 
@@ -100,22 +92,25 @@
         # find application element using an xpath
         self.logger.trace('Parser.load_application_rules: searching application element for {}'
                           .format(application_name))
         application_elt = self.get_application_element(application_name)
         if application_elt is not None:
             rules.managed = True
             self.load_boolean(application_elt, 'distributed', rules)
-            self.load_application_nodes(application_elt, rules)
+            self.load_nodes(application_elt, rules)
             self.load_sequence(application_elt, 'start_sequence', rules)
             self.load_sequence(application_elt, 'stop_sequence', rules)
             self.load_enum(application_elt, 'starting_strategy', StartingStrategies, rules)
             self.load_enum(application_elt, 'starting_failure_strategy', StartingFailureStrategies, rules)
             self.load_enum(application_elt, 'running_failure_strategy', RunningFailureStrategies, rules)
             self.logger.debug('Parser.load_application_rules: application {} - rules {}'
                               .format(application_name, rules))
+        # check that rules are compliant with dependencies
+        rules.check_dependencies(application_name)
+        self.logger.debug('Parser.load_application_rules: application={} rules={}'.format(application_name, rules))
 
     def get_application_element(self, application_name: str) -> Optional[Any]:
         """ Try to find the definition of an application in rules files.
         First try to to find the definition based on the exact application name.
         If not found, second try to find a corresponding pattern.
 
         :param application_name: the application name
@@ -142,22 +137,22 @@
         """ Find an entry corresponding to the process in the rules, then load the parameters found.
         A final check is performed to detect inconsistencies.
 
         :param namespec: the process namespec
         :param rules: the process rules to fill
         :return: None
         """
-        self.logger.trace('Parser.load_process_rules: searching program element for {}'.format(namespec))
+        self.logger.trace('Parser.load_program_rules: searching program element for {}'.format(namespec))
         program_elt = self.get_program_element(namespec)
         if program_elt is not None:
             # load element parameters into rules
             self.load_model_rules(program_elt, rules, Parser.LOOP_CHECK)
-            # check that rules are compliant with dependencies
-            rules.check_dependencies(namespec)
-            self.logger.debug('Parser.load_process_rules: process {} - rules {}'.format(namespec, rules))
+        # check that rules are compliant with dependencies
+        rules.check_dependencies(namespec)
+        self.logger.debug('Parser.load_program_rules: process={} rules={}'.format(namespec, rules))
 
     def load_model_rules(self, program_elt: Any, rules: ProcessRules, loop_check: int) -> None:
         """ Load the parameters found whatever it is given by a program or a model section.
         If the section includes a reference to a model, it is loaded first and then eventually superseded
         by other attributes.
 
         :param program_elt: the XML element containing rules definition
@@ -175,15 +170,15 @@
         if model_elt is not None:
             self.logger.trace('Parser.load_model_rules: found model={} from program={}'
                               .format(model_elt.get('name'), Parser.get_element_name(program_elt)))
             # a model can reference another model
             # WARN: recursive call, counter decreased
             self.load_model_rules(model_elt, rules, loop_check - 1)
         # other attributes found may be used to complete or supersede the possible model
-        self.load_program_nodes(program_elt, rules)
+        self.load_nodes(program_elt, rules)
         self.load_sequence(program_elt, 'start_sequence', rules)
         self.load_sequence(program_elt, 'stop_sequence', rules)
         self.load_boolean(program_elt, 'required', rules)
         self.load_boolean(program_elt, 'wait_exit', rules)
         self.load_expected_loading(program_elt, rules)
         self.load_enum(program_elt, 'running_failure_strategy', RunningFailureStrategies, rules)
 
@@ -267,26 +262,15 @@
             # filter the unknown nodes (or remaining aliases)
             node_names = self.supvisors.address_mapper.filter(node_names)
         # re-inject the hashtag if needed. position does not matter
         if ref_hashtag:
             node_names.append('#')
         return node_names
 
-    def load_application_nodes(self, elt: Any, rules: ApplicationRules) -> None:
-        """ Get the nodes where the non-distributed application is authorized to run.
-
-        :param elt: the XML element containing rules definition for an application
-        :param rules: the application structure used to store the rules found
-        :return: None
-        """
-        value = elt.findtext('addresses')
-        if value:
-            rules.node_names = self.check_node_list(value)
-
-    def load_program_nodes(self, elt: Any, rules: ProcessRules) -> None:
+    def load_nodes(self, elt: Any, rules: AnyRules) -> None:
         """ Get the nodes where the program is authorized to run.
 
         :param elt: the XML element containing rules definition for a program
         :param rules: the process structure used to store the rules found
         :return: None
         """
         value = elt.findtext('addresses')
```

### Comparing `supvisors-0.8/supvisors/statemachine.py` & `supvisors-0.9/supvisors/statemachine.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/statscollector.py` & `supvisors-0.9/supvisors/statscollector.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/statscompiler.py` & `supvisors-0.9/supvisors/statscompiler.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/strategy.py` & `supvisors-0.9/supvisors/strategy.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/supvisorsctl.py` & `supvisors-0.9/supvisors/supvisorsctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ======================================================================
 
 import errno
 import socket
+import sys
 
+from supervisor import supervisorctl
 from supervisor import xmlrpc
 from supervisor.compat import xmlrpclib
 from supervisor.loggers import getLevelNumByDescription, LOG_LEVELS_BY_NUM
-from supervisor.options import split_namespec
+from supervisor.options import ClientOptions, split_namespec
 from supervisor.states import getProcessStateDescription
-from supervisor.supervisorctl import ControllerPluginBase
+from supervisor.supervisorctl import Controller, ControllerPluginBase
 
 from .rpcinterface import API_VERSION, RPCInterface
 from .ttypes import ConciliationStrategies, StartingStrategies, PayloadList
 from .utils import simple_localtime
 
 
 class ControllerPlugin(ControllerPluginBase):
@@ -207,15 +209,15 @@
                     rules_list.append(rules)
             # print results
             if rules_list:
                 # get longer from application names and title
                 max_appli = max(len(rules['application_name']) for rules in rules_list)
                 max_appli = max(max_appli, len('Application')) + 2
                 # get longer from distribution nodes and title
-                max_nodes = max(len(rules.get('addresses', '')) for rules in rules_list)
+                max_nodes = max(len('{}'.format(rules.get('addresses', ''))) for rules in rules_list)
                 max_nodes = max(max_nodes, len('Nodes')) + 2
                 # print title
                 template_managed = '%(appli)-{}s%(managed)-9s%(distributed)-13s%(nodes)-{}s' \
                                    '%(start_seq)-7s%(stop_seq)-7s' \
                                    '%(starting_strategy)-13s%(starting_failure_strategy)-18s' \
                                    '%(running_failure_strategy)s' \
                     .format(max_appli, max_nodes)
@@ -810,7 +812,28 @@
         """ Write the information template. """
         self.ctl.output(template % payload)
 
 
 def make_supvisors_controller_plugin(controller):
     """ Create a plugin for the Supvisors commands. """
     return ControllerPlugin(controller)
+
+
+# Copied and adapted from supervisor.supervisorctl source code
+def main(args=None, options=None):
+    # read options
+    if options is None:
+        options = ClientOptions()
+    options.realize(args, doc=supervisorctl.__doc__)
+    # add supvisors plugin if not there
+    if not any(factory[0] == 'supvisors' for factory in options.plugin_factories):
+        options.plugin_factories.append(('supvisors', make_supvisors_controller_plugin, {}))
+    # create controller
+    c = Controller(options)
+    # process single command
+    if options.args:
+        c.onecmd(' '.join(options.args))
+        sys.exit(c.exitstatus)
+    # enter the interactive mode
+    if options.interactive:
+        c.exec_cmdloop(args, options)
+        sys.exit(0)  # exitstatus always 0 for interactive mode
```

### Comparing `supvisors-0.8/supvisors/supvisorszmq.py` & `supvisors-0.9/supvisors/supvisorszmq.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/ttypes.py` & `supvisors-0.9/supvisors/ttypes.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/utils.py` & `supvisors-0.9/supvisors/utils.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/viewapplication.py` & `supvisors-0.9/supvisors/viewapplication.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,49 +40,55 @@
         self.application: Optional[ApplicationStatus] = None
 
     def handle_parameters(self):
         """ Retrieve the parameters selected on the web page. """
         ViewHandler.handle_parameters(self)
         # check if application name is available
         self.application_name = self.view_ctx.parameters[APPLI]
-        if self.application_name:
+        try:
             # store application
             self.application = self.sup_ctx.applications[self.application_name]
-        else:
-            self.view_ctx.message(error_message('No application'))
+        except KeyError:
+            # may happen when the user clicks from a page of the previous launch while the current Supvisors is still
+            # in INITIALIZATION stats or if wrong appliname set in URL
+            self.logger.error('ApplicationView.handle_parameters: unknown application_name={}'
+                              .format(self.application_name))
+            # redirect page to main page to avoid infinite error loop
+            self.view_ctx.store_message = error_message('Unknown application: {}'.format(self.application_name))
+            self.view_ctx.redirect = True
 
     def write_navigation(self, root):
-        """ Rendering of the navigation menu with selection
-        of the current application. """
+        """ Rendering of the navigation menu with selection of the current application. """
         self.write_nav(root, appli=self.application_name)
 
     # RIGHT SIDE / HEADER part
     def write_header(self, root):
         """ Rendering of the header part of the Supvisors Application page. """
-        # set application name
-        elt = root.findmeld('application_mid')
-        elt.content(self.application_name)
-        # set application state
-        elt = root.findmeld('state_mid')
-        elt.content(self.application.state.name)
-        # set LED iaw major/minor failures
-        elt = root.findmeld('state_led_mid')
-        if self.application.major_failure:
-            elt.attrib['class'] = 'status_red'
-        elif self.application.minor_failure:
-            elt.attrib['class'] = 'status_yellow'
-        elif self.application.running():
-            elt.attrib['class'] = 'status_green'
-        else:
-            elt.attrib['class'] = 'status_empty'
-        # write options
-        self.write_starting_strategy(root)
-        self.write_periods(root)
-        # write actions related to application
-        self.write_application_actions(root)
+        if self.application:
+            # set application name
+            elt = root.findmeld('application_mid')
+            elt.content(self.application_name)
+            # set application state
+            elt = root.findmeld('state_mid')
+            elt.content(self.application.state.name)
+            # set LED iaw major/minor failures
+            elt = root.findmeld('state_led_mid')
+            if self.application.major_failure:
+                elt.attrib['class'] = 'status_red'
+            elif self.application.minor_failure:
+                elt.attrib['class'] = 'status_yellow'
+            elif self.application.running():
+                elt.attrib['class'] = 'status_green'
+            else:
+                elt.attrib['class'] = 'status_empty'
+            # write options
+            self.write_starting_strategy(root)
+            self.write_periods(root)
+            # write actions related to application
+            self.write_application_actions(root)
 
     def write_starting_strategy(self, root):
         """ Write applicable starting strategies. """
         # get the current strategy
         strategy = self.view_ctx.parameters[STRATEGY]
         # set hyperlinks for strategy actions
         for str_strategy in StartingStrategies._member_names_:
@@ -107,28 +113,30 @@
         elt = root.findmeld('restartapp_a_mid')
         url = self.view_ctx.format_url('', self.page_name, **{ACTION: 'restartapp'})
         elt.attributes(href=url)
 
     # RIGHT SIDE / BODY part
     def write_contents(self, root):
         """ Rendering of the contents part of the page. """
-        data = self.get_process_data()
-        self.write_process_table(root, data)
-        # check selected Process Statistics
-        namespec = self.view_ctx.parameters[PROCESS]
-        if namespec:
-            status = self.view_ctx.get_process_status(namespec)
-            if not status or status.stopped() or status.application_name != self.application_name:
-                self.logger.warn('unselect Process Statistics for {}'.format(namespec))
-                # form parameter is not consistent. remove it
-                self.view_ctx.parameters[PROCESS] = ''
-        # write selected Process Statistics
-        namespec = self.view_ctx.parameters[PROCESS]
-        info = next(filter(lambda x: x['namespec'] == namespec, data), {})
-        self.write_process_statistics(root, info)
+        if self.application:
+            data = self.get_process_data()
+            self.write_process_table(root, data)
+            # check selected Process Statistics
+            namespec = self.view_ctx.parameters[PROCESS]
+            if namespec:
+                status = self.view_ctx.get_process_status(namespec)
+                if not status or status.stopped() or status.application_name != self.application_name:
+                    self.logger.warn('ApplicationView.write_contents: unselect Process Statistics for {}'
+                                     .format(namespec))
+                    # form parameter is not consistent. remove it
+                    self.view_ctx.parameters[PROCESS] = ''
+            # write selected Process Statistics
+            namespec = self.view_ctx.parameters[PROCESS]
+            info = next(filter(lambda x: x['namespec'] == namespec, data), {})
+            self.write_process_statistics(root, info)
 
     def get_process_last_desc(self, namespec: str) -> Tuple[Optional[str], str]:
         """ Get the latest description received from the process across all nodes.
         A priority is given to the info coming from a node where the process is running. """
         status = self.view_ctx.get_process_status(namespec)
         return status.get_last_description()
 
@@ -181,45 +189,46 @@
                 if node_name == info['node_name']:
                     update_attrib(elt, 'class', 'active')
         else:
             elt = tr_elt.findmeld('running_ul_mid')
             elt.replace('')
 
     # ACTIONS
-    def make_callback(self, namespec, action):
+    def make_callback(self, namespec: str, action: str):
         """ Triggers processing iaw action requested. """
         if action == 'refresh':
             return self.refresh_action()
-        # get current strategy
-        strategy = StartingStrategies[self.view_ctx.parameters[STRATEGY]]
-        if action == 'startapp':
-            return self.start_application_action(strategy)
-        if action == 'stopapp':
-            return self.stop_application_action()
-        if action == 'restartapp':
-            return self.restart_application_action(strategy)
-        if namespec:
-            if self.view_ctx.get_process_status(namespec) is None:
-                return delayed_error('No such process named %s' % namespec)
-            if action == 'start':
-                return self.start_process_action(strategy, namespec)
-            if action == 'stop':
-                return self.stop_process_action(namespec)
-            if action == 'restart':
-                return self.restart_process_action(strategy, namespec)
-            if action == 'clearlog':
-                return self.clearlog_process_action(namespec)
+        if self.application:
+            # get current strategy
+            strategy = StartingStrategies[self.view_ctx.parameters[STRATEGY]]
+            if action == 'startapp':
+                return self.start_application_action(strategy)
+            if action == 'stopapp':
+                return self.stop_application_action()
+            if action == 'restartapp':
+                return self.restart_application_action(strategy)
+            if namespec:
+                if self.view_ctx.get_process_status(namespec) is None:
+                    return delayed_error('No such process named %s' % namespec)
+                if action == 'start':
+                    return self.start_process_action(strategy, namespec)
+                if action == 'stop':
+                    return self.stop_process_action(namespec)
+                if action == 'restart':
+                    return self.restart_process_action(strategy, namespec)
+                if action == 'clearlog':
+                    return self.clearlog_process_action(namespec)
 
     @staticmethod
     def refresh_action():
         """ Refresh web page. """
         return delayed_info('Page refreshed')
 
     # Common processing for starting and stopping actions
-    def start_action(self, strategy, rpc_name, arg_name, arg_type):
+    def start_action(self, strategy: StartingStrategies, rpc_name: str, arg_name: str, arg_type: str):
         """ Start/Restart an application or a process iaw the strategy. """
         try:
             rpc_intf = self.supvisors.info_source.supvisors_rpc_interface
             cb = getattr(rpc_intf, rpc_name)(strategy, arg_name)
         except RPCError as e:
             return delayed_error('{}: {}'.format(rpc_name, e.text))
         if callable(cb):
@@ -236,15 +245,15 @@
 
             onwait.delay = 0.1
             return onwait
         if cb:
             return delayed_info('{} {} started'.format(arg_type, arg_name))
         return delayed_warn('{} {} NOT started'.format(arg_type, arg_name))
 
-    def stop_action(self, rpc_name, arg_name, arg_type):
+    def stop_action(self, rpc_name: str, arg_name: str, arg_type):
         """ Stop an application or a process. """
         try:
             rpc_intf = self.supvisors.info_source.supvisors_rpc_interface
             cb = getattr(rpc_intf, rpc_name)(arg_name)
         except RPCError as e:
             return delayed_error('{}: {}'.format(rpc_name, e.text))
         if callable(cb):
@@ -260,41 +269,70 @@
             onwait.delay = 0.1
             return onwait
         if cb:
             return delayed_info('{} {} stopped'.format(arg_type, arg_name))
         return delayed_warn('{} {} NOT stopped'.format(arg_type, arg_name))
 
     # Application actions
-    def start_application_action(self, strategy):
-        """ Start the application iaw the strategy. """
+    def start_application_action(self, strategy) -> None:
+        """ Start the application iaw the strategy.
+
+        :param strategy: the strategy to apply for starting the application
+        :return: None
+        """
         return self.start_action(strategy, 'start_application', self.application_name, 'Application')
 
-    def restart_application_action(self, strategy):
-        """ Restart the application iaw the strategy. """
+    def restart_application_action(self, strategy) -> None:
+        """ Restart the application iaw the strategy.
+
+        :param strategy: the strategy to apply for restarting the application
+        :return: None
+        """
         return self.start_action(strategy, 'restart_application', self.application_name, 'Application')
 
-    def stop_application_action(self):
-        """ Stop the application. """
+    def stop_application_action(self) -> None:
+        """ Stop the application.
+
+        :return: None
+        """
         return self.stop_action('stop_application', self.application_name, 'Application')
 
     # Process actions
-    def start_process_action(self, strategy, namespec):
-        """ Start the process named namespec iaw the strategy. """
+    def start_process_action(self, strategy: StartingStrategies, namespec: str) -> None:
+        """ Start the process named namespec iaw the strategy.
+
+        :param strategy: the strategy to apply for starting the process
+        :param namespec: the process namespec
+        :return: None
+        """
         return self.start_action(strategy, 'start_process', namespec, 'Process')
 
-    def restart_process_action(self, strategy, namespec):
-        """ Restart the process named namespec iaw the strategy. """
+    def restart_process_action(self, strategy: StartingStrategies, namespec: str) -> None:
+        """ Restart the process named namespec iaw the strategy.
+
+        :param strategy: the strategy to apply for restarting the process
+        :param namespec: the process namespec
+        :return: None
+        """
         return self.start_action(strategy, 'restart_process', namespec, 'Process')
 
-    def stop_process_action(self, namespec):
-        """ Stop the process named namespec. """
+    def stop_process_action(self, namespec: str) -> None:
+        """ Stop the process named namespec.
+
+        :param namespec: the process namespec
+        :return: None
+        """
         return self.stop_action('stop_process', namespec, 'Process')
 
-    def clearlog_process_action(self, namespec):
+    def clearlog_process_action(self, namespec: str) -> None:
         """ Can't call supervisor StatusView source code from application view.
-        Just do the same job. """
+        Just do the same job.
+
+        :param namespec: the process namespec
+        :return: None
+        """
         try:
             rpc_intf = self.supvisors.info_source.supervisor_rpc_interface
             rpc_intf.clearProcessLogs(namespec)
         except RPCError as e:
             return delayed_error('unexpected rpc fault [%d] %s' % (e.code, e.text))
         return delayed_info('Log for %s cleared' % namespec)
```

### Comparing `supvisors-0.8/supvisors/viewcontext.py` & `supvisors-0.9/supvisors/viewcontext.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from distutils.util import strtobool
 from typing import Optional, Tuple
 from urllib.parse import quote
 
 from .process import ProcessStatus
 from .ttypes import StartingStrategies, NameList
-from .webutils import error_message
+from .webutils import SUPVISORS_PAGE, error_message
 
 
 # form parameters
 SERVER_URL = 'SERVER_URL'
 SERVER_PORT = 'SERVER_PORT'
 PATH_TRANSLATED = 'PATH_TRANSLATED'
 
@@ -67,14 +67,16 @@
         # keep references to Supvisors instance
         self.supvisors = context.supervisord.supvisors
         self.logger = self.supvisors.logger
         # keep reference to the local node
         self.local_node_name = self.supvisors.address_mapper.local_node_name
         # initialize parameters
         self.parameters = {}
+        self.store_message = None
+        self.redirect = False
         # extract parameters from context
         # WARN: period must be done before processname and cpuid as it requires to be set to access statistics
         self.update_period()
         self.update_strategy()
         self.update_auto_refresh()
         self.update_node_name()
         self.update_application_name()
@@ -157,15 +159,15 @@
         # extract mask from context
         str_value = self.http_context.form.get(SHRINK_EXPAND)
         if str_value:
             # check that value has correct format (only 0-1 and size equal to number of applications)
             if re.match(r'^[0-1]{%d}$' % len(value), str_value):
                 value = str_value
             else:
-                self.message(error_message('Incorrect SHRINK_EXPAND: {}'.format(str_value)))
+                self.store_message = error_message('Incorrect SHRINK_EXPAND: {}'.format(str_value))
         self.logger.trace('ViewContext.update_shrink_expand: SHRINK_EXPAND set to {}'.format(value))
         self.parameters[SHRINK_EXPAND] = value
 
     def url_parameters(self, reset_shex, **kwargs):
         """ Return the list of parameters for an URL. """
         parameters = dict(self.parameters, **kwargs)
         if reset_shex:
@@ -174,20 +176,23 @@
 
     def format_url(self, node_name, page, **kwargs):
         """ Format URL from parameters. """
         local_node_name = not node_name or node_name == self.local_node_name
         url = 'http://{}:{}/'.format(quote(node_name), self.get_server_port()) if node_name else ''
         return '{}{}?{}'.format(url, page, self.url_parameters(not local_node_name, **kwargs))
 
-    def message(self, message):
+    def fire_message(self) -> None:
         """ Set message in context response to be displayed at next refresh. """
-        form = self.http_context.form
-        args = {MESSAGE: message[1], GRAVITY: message[0]}
-        location = '{}{}?{}'.format(form[SERVER_URL], form[PATH_TRANSLATED], self.url_parameters(False, **args))
-        self.http_context.response[HEADERS][LOCATION] = location
+        if self.store_message:
+            form = self.http_context.form
+            args = {MESSAGE: self.store_message[1], GRAVITY: self.store_message[0]}
+            # if redirect requested, go back to main page
+            path_translated = '/' + SUPVISORS_PAGE if self.redirect else form[PATH_TRANSLATED]
+            location = '{}{}?{}'.format(form[SERVER_URL], path_translated, self.url_parameters(False, **args))
+            self.http_context.response[HEADERS][LOCATION] = location
 
     def get_nbcores(self, node_name=None):
         """ Get the number of processors of the local node. """
         stats_node = node_name or self.local_node_name
         return self.supvisors.statistician.nbcores.get(stats_node, 0)
 
     def get_node_stats(self, node_name: str = None):
@@ -241,47 +246,47 @@
         value = default_value
         str_value = self.http_context.form.get(param)
         if str_value:
             # check that value is known to Supvisors
             if str_value in check_list:
                 value = str_value
             else:
-                self.message(error_message('Incorrect {}: {}'.format(param, str_value)))
+                self.store_message = error_message('Incorrect {}: {}'.format(param, str_value))
         # assign value found or default
         self.logger.trace('ViewContext._update_string: {} set to {}'.format(param, value))
         self.parameters[param] = value
 
     def _update_integer(self, param, check_list, default_value=0):
         """ Extract information from context and convert to integer based on allowed values in check_list. """
         value = default_value
         str_value = self.http_context.form.get(param)
         if str_value:
             try:
                 int_value = int(str_value)
             except ValueError:
-                self.message(error_message('{} is not an integer: {}'.format(param, str_value)))
+                self.store_message = error_message('{} is not an integer: {}'.format(param, str_value))
             else:
                 # check that int_value is defined in check list
                 if int_value in check_list:
                     value = int_value
                 else:
-                    self.message(error_message('Incorrect {}: {}'.format(param, int_value)))
+                    self.store_message = error_message('Incorrect {}: {}'.format(param, int_value))
         # assign value found or default
         self.logger.trace('ViewContext._update_integer: {} set to {}'.format(param, value))
         self.parameters[param] = value
 
     def _update_boolean(self, param, default_value=False):
         """ Extract information from context and convert to boolean based on allowed values in check_list. """
         value = default_value
         str_value = self.http_context.form.get(param)
         if str_value:
             try:
                 value = strtobool(str_value)
             except ValueError:
-                self.message(error_message('{} is not a boolean-like: {}'.format(param, str_value)))
+                self.store_message = error_message('{} is not a boolean-like: {}'.format(param, str_value))
         # assign value found or default
         self.logger.trace('ViewContext._update_boolean: {} set to {}'.format(param, value))
         self.parameters[param] = value
 
     @staticmethod
     def cpu_id_to_string(idx):
         """ Get a printable form of cpu index. """
```

### Comparing `supvisors-0.8/supvisors/viewhandler.py` & `supvisors-0.9/supvisors/viewhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,21 @@
 from .utils import get_stats
 from .viewcontext import *
 from .viewimage import process_cpu_img, process_mem_img
 from .webutils import *
 
 
 class ViewHandler(MeldView):
-    """ Helper class to commonize rendering and behavior between handlers inheriting from MeldView. """
+    """ Helper class to share rendering and behavior between handlers inheriting from MeldView. """
 
     def __init__(self, context):
         """ Initialization of the attributes. """
         MeldView.__init__(self, context)
         self.page_name = None
         # add Supvisors shortcuts
-        # WARN: do not shortcut Supvisors context as it is already used by MeldView
         self.supvisors = context.supervisord.supvisors
         self.logger = self.supvisors.logger
         # cannot store context as it is named or it would crush the http context
         self.sup_ctx = self.supvisors.context
         # keep reference to the local node name
         self.local_node_name = self.supvisors.address_mapper.local_node_name
         # init view_ctx (only for tests)
@@ -71,14 +70,16 @@
             # display result
             root = self.clone()
             # write navigation menu, page header and contents
             self.write_common(root)
             self.write_navigation(root)
             self.write_header(root)
             self.write_contents(root)
+            # send error message only at the end to get all URL parameters
+            self.view_ctx.fire_message()
             return as_string(root.write_xhtmlstring())
 
     def handle_parameters(self):
         """ Retrieve the parameters selected on the web page. """
         self.view_ctx = ViewContext(self.context)
         self.logger.debug('New context: {}'. format(self.view_ctx.parameters))
 
@@ -115,14 +116,15 @@
             update_attrib(elt, 'class', 'active')
         # set bottom message
         print_message(root, self.view_ctx.get_gravity(), self.view_ctx.get_message())
 
     def write_navigation(self, root):
         """ Write the navigation menu.
         Subclasses will define the write_nav parameters to be used. """
+        raise NotImplementedError
 
     def write_nav(self, root, node_name=None, appli=None):
         """ Write the navigation menu. """
         self.write_nav_nodes(root, node_name)
         self.write_nav_applications(root, appli)
 
     def write_nav_nodes(self, root, node_name):
@@ -182,14 +184,15 @@
         # warn at title level if any application has a failure
         if any_failure:
             update_attrib(root.findmeld('appli_h_mid'), 'class', 'failure')
 
     def write_header(self, root):
         """ Write the header part of the page.
         Subclasses will define what's to be done. """
+        raise NotImplementedError
 
     def write_periods(self, root):
         """ Write configured periods for statistics. """
         mid_elt = root.findmeld('period_li_mid')
         periods = self.supvisors.options.stats_periods
         for li_elt, item in mid_elt.repeat(periods):
             # print period button
@@ -200,14 +203,15 @@
                 url = self.view_ctx.format_url('', self.page_name, **{PERIOD: item})
                 elt.attributes(href=url)
             elt.content('{}s'.format(item))
 
     def write_contents(self, root):
         """ Write the contents part of the page.
         Subclasses will define what's to be done. """
+        raise NotImplementedError
 
     def write_common_process_cpu(self, tr_elt, info):
         """ Write the CPU part of the common process status.
         Statistics data comes from node. """
         proc_stats = info['proc_stats']
         elt = tr_elt.findmeld('pcpu_a_mid')
         if proc_stats and len(proc_stats[0]) > 0:
@@ -443,19 +447,20 @@
                 return NOT_DONE_YET
             # intermediate check
             message = self.callback()
             if message is NOT_DONE_YET:
                 return NOT_DONE_YET
             # post to write message
             if message is not None:
-                self.view_ctx.message(format_gravity_message(message))
+                self.view_ctx.store_message = format_gravity_message(message)
 
-    def make_callback(self, namespec, action):
+    def make_callback(self, namespec: str, action: str):
         """ Triggers processing iaw action requested.
         Subclasses will define what's to be done. """
+        raise NotImplementedError
 
     @staticmethod
     def set_slope_class(elt, value):
         """ Set attribute class iaw positive or negative slope. """
         if abs(value) < .005:
             update_attrib(elt, 'class', 'stable')
         elif value > 0:
```

### Comparing `supvisors-0.8/supvisors/viewhostaddress.py` & `supvisors-0.9/supvisors/viewhostaddress.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/viewimage.py` & `supvisors-0.9/supvisors/viewimage.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/viewprocaddress.py` & `supvisors-0.9/supvisors/viewprocaddress.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/viewsupstatus.py` & `supvisors-0.9/supvisors/viewsupstatus.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/viewsupvisors.py` & `supvisors-0.9/supvisors/viewsupvisors.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors/webutils.py` & `supvisors-0.9/supvisors/webutils.py`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/supvisors.egg-info/PKG-INFO` & `supvisors-0.9/supvisors.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: supvisors
-Version: 0.8
+Version: 0.9
 Summary: A Control System for Distributed Applications
 Home-page: https://github.com/julien6387/supvisors
 Author: Julien Le Cléach
 Author-email: julien.6387.dev@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/julien6387/supvisors/archive/0.8.tar.gz
+Download-URL: https://github.com/julien6387/supvisors/archive/0.9.tar.gz
 Description: # **Supvisors**
         [![PyPI version][pypi-image]][pypi-url] [![Build Status][ci-image]][ci-url] [![Coverage Status][coveralls-image]][coveralls-url] [![Documentation Status][docs-image]][docs-url]
         
         
         **Supvisors** is a Control System for Distributed Applications, based on
         multiple instances of Supervisor.
         
@@ -105,45 +105,77 @@
         [coveralls-image]: https://coveralls.io/repos/github/julien6387/supvisors/badge.svg?branch=master
         [coveralls-url]: https://coveralls.io/github/julien6387/supvisors?branch=master
         
         [docs-image]: https://readthedocs.org/projects/supvisors/badge/?version=master
         [docs-url]: https://supvisors.readthedocs.io/en/master
         
         
-        Change Log
-        ==========
+        # Change Log
         
-        0.8 (2021-08-22)
-        ----------------
+        ## 0.9 (2021-08-31)
         
-        * Fixed exception in ``INITIALIZATION`` state when the *Master* declared by other nodes is not RUNNING yet and
+        * Enable the hash '#' for the `addresses` of a non-distributed application.
+        
+        * Add `supvisorsctl` to pally the lack of support of `supervisorctl` when used with `--serverurl URL` option.
+          See related [Supervisor Issue #1455](https://github.com/Supervisor/supervisor/issues/1455).
+        
+        * Provide `breed.py` as a binary of **Supvisors**: `supvisors_breed`.
+          The script only considers group duplication as it is fully valid to include multiple times a program definition
+          in several groups.
+        
+        * Move the contents of the `[supvisors]` section into the `[rpcinterface:supvisors]` section and benefit from the
+          configuration structure provided by Supervisor. The `[supvisors]` section itself is thus obsolete.
+        
+        * Remove deprecated support of `pattern` elements.
+        
+        * Fixed issue when using the Web UI Application page from a previous launch.
+        
+        * Invert the stop sequence logic, starting from the greatest ``stop_sequence`` number to the lowest one.
+        
+        * When ``stop_sequence`` is not set in the rules files, it is defaulted to the ``start_sequence`` value.
+          With the new stop sequence logic, the stop sequence is by default exactly the opposite of the start sequence.
+        
+        * Fixed Nodes column width for `supervisorctl application_rules`.
+        
+        * `CHANGES.rst` replaced with `CHANGES.md`.
+        
+        * 'Scenario 3' has been added to the **Supvisors** use cases.
+        
+        * A 'Gathering' configuration has been added to the **Supvisors** use cases. It combines all uses cases.
+        
+        * Update documentation.
+        
+        
+        ## 0.8 (2021-08-22)
+        
+        * Fixed exception in `INITIALIZATION` state when the *Master* declared by other nodes is not RUNNING yet and
           the *core nodes* are RUNNING.
         
         * Fixed exception when program rules and extra arguments are tested against a program unknown to the local Supervisor.
         
         * Fixed issue about program patterns that were applicable to all elements. The scope of program patterns is now limited
           to their owner application.
         
         * Fixed issue with infinite tries of application restart when the process cannot be started due to a lack of resources
-          and ``RESTART_APPLICATION`` is set on the program in the **Supvisors** rules file.
+          and `RESTART_APPLICATION` is set on the program in the **Supvisors** rules file.
         
         * Fixed issue about application state not updated after a node has become silent.
         
-        * Fixed issue when choosing a node in ``Starter``. Apply the requests that have not been satisfied yet for
+        * Fixed issue when choosing a node in `Starter`. Apply the requests that have not been satisfied yet for
           non-distributed applications.
         
         * Logic for application major / minor failures reviewed.
         
         * Simplify the insertion of applications to start or stop in Commander jobs.
         
         * In the rules file, support for application patterns has been added.
         
-        * In the rules file, ``pattern`` elements are **deprecated** and are replaced by ``program`` elements with a ``pattern``
-          attribute instead of a ``name`` attribute.
-          Support for ``pattern`` elements will be removed in the next version of **Supvisors**.
+        * In the rules file, `pattern` elements are **deprecated** and are replaced by `program` elements with a `pattern`
+          attribute instead of a `name` attribute.
+          Support for `pattern` elements will be removed in the next version of **Supvisors**.
         
         * Node aliases have been added to the rules file.
         
         * Add the current node to all pages of Web UI to be aware of the node that displays the page.
         
         * The Web UI is updated to handle a large list of applications, nodes, processor cores and network interfaces.
         
@@ -154,226 +186,219 @@
           has raised a failure.
         
         * In the Application page of the Web UI, default starting strategy is the starting strategy defined in the rules file
           for the application considered.
         
         * In the Application ang Process page, the detailed process statistics can be deselected.
         
-        * Titles added to the output of :program:`supervisorctl` ``address_status`` and ``application_info``.
+        * Titles added to the output of :program:`supervisorctl` `address_status` and `application_info`.
         
-        * The XML schema has been moved to a separate file ``rules.xsd``.
+        * The XML schema has been moved to a separate file `rules.xsd`.
         
         * Remove dependency to *netifaces* as *psutil* provides the function.
         
-        * Scenario 2 has been added to the **Supvisors** use cases.
+        * 'Scenario 2' has been added to the **Supvisors** use cases.
         
-        * A script ``breed.py`` has been added to the install package.
+        * A script `breed.py` has been added to the install package.
           It can be used to duplicate the applications based on a template configuration and more particularly used to prepare
           the Scenario 2 of the **Supvisors** use cases.
         
         * Update documentation.
         
         
-        0.7 (2021-08-15)
-        ----------------
+        ## 0.7 (2021-08-15)
         
-        * Fixed `Issue #92 <https://github.com/julien6387/supvisors/issues/92>`_.
+        * Fixed [Issue #92](https://github.com/julien6387/supvisors/issues/92).
           The *Master* drives the state of all **Supvisors** instances and a simplified state machine has been assigned
           to non-master **Supvisors** instances. The loss of the *Master* instance is managed in all relevant states.
         
-        * Fixed issue about applications that would be started automatically whereas their ``start_sequence`` is 0.
+        * Fixed issue about applications that would be started automatically whereas their `start_sequence` is 0.
           The regression has been introduced during the implementation of applications repair in **Supvisors 0.6**.
         
         * Enable stop sequence on *Unmanaged* applications.
         
         * In the application navigation menu of the Web UI, add a red light to applications having raised a failure.
         
-        * New application rules ``distributed`` and ``addresses`` added to the **Supvisors** rules file.
+        * New application rules `distributed` and `addresses` added to the **Supvisors** rules file.
           Non-distributed applications have all their processes started on the same node chosen in accordance with the
-          ``addresses`` and the ``starting_strategy``.
+          `addresses` and the `starting_strategy`.
         
         * Starting strategy added to the application rules.
         
-        * Fixed issue when choosing a node in ``Starter``. The starting strategies considers the current load of the nodes
+        * Fixed issue when choosing a node in `Starter`. The starting strategies considers the current load of the nodes
           and includes the requests that have not been satisfied yet.
         
-        * Fixed issue with infinite process restart when the process crashes and ``RESTART_PROCESS`` is set on the program
-          in the **Supvisors** rules file. When the process crashes, only the *Supervisor* ``autorestart`` applies.
-          The **Supvisors** ``RESTART_PROCESS`` applies only when the node becomes inactive.
+        * Fixed issue with infinite process restart when the process crashes and `RESTART_PROCESS` is set on the program
+          in the **Supvisors** rules file. When the process crashes, only the *Supervisor* `autorestart` applies.
+          The **Supvisors** `RESTART_PROCESS` applies only when the node becomes inactive.
         
         * Fixed exception when forcing the state on a process that is unknown to the local Supervisor.
         
-        * Promote the ``RESTART_PROCESS`` into ``RESTART_APPLICATION`` if the application is stopped.
+        * Promote the `RESTART_PROCESS` into `RESTART_APPLICATION` if the application is stopped.
         
-        * For the *Master* election, give a priority to nodes declared in the ``forced_synchro_if`` option if used.
+        * For the *Master* election, give a priority to nodes declared in the `forced_synchro_if` option if used.
         
-        * When using the ``forced_synchro_if`` option and when ``auto_fence`` is activated, do not isolate nodes as long as
-          ``synchro_timeout`` has not passed.
+        * When using the `forced_synchro_if` option and when `auto_fence` is activated, do not isolate nodes as long as
+          `synchro_timeout` has not passed.
         
-        * In the ``INITALIZATION`` state, skip the synchronization phase upon notification of a known *Master* and adopt it.
+        * In the `INITALIZATION` state, skip the synchronization phase upon notification of a known *Master* and adopt it.
         
-        * Add reciprocity to isolation even if ``auto_fence`` is not activated.
+        * Add reciprocity to isolation even if `auto_fence` is not activated.
         
         * In the process description of the Web UI Application page, add information about the node name.
           In particular, it is useful to know where the process was running when it is stopped.
         
         * Start adding use cases to documentation, inspired by real examples.
-          Scenario 1 has been added.
+          'Scenario 1' has been added.
         
         * Documentation updated.
         
         
-        0.6 (2021-08-01)
-        ----------------
+        ## 0.6 (2021-08-01)
         
         * Applications that are not declared in the rules file are not *managed*.
           *Unmanaged* applications have no start/stop sequence, no state and status (always STOPPED) and **Supvisors**
           does not raise a conflict if multiple instances are running over multiple nodes.
         
         * Improve **Supvisors** stability when dealing with remote programs undefined locally.
         
-        * Add expand / shrink actions to applications to the ``ProcAddressView`` of the Web UI.
+        * Add expand / shrink actions to applications to the `ProcAddressView` of the Web UI.
         
-        * Upon authorization of a new node in **Supvisors**, back to ``DEPLOYMENT`` state to repair applications.
+        * Upon authorization of a new node in **Supvisors**, back to `DEPLOYMENT` state to repair applications.
         
-        * Add RPC ``change_log_level`` to dynamically change the **Supvisors** logger level.
+        * Add RPC `change_log_level` to dynamically change the **Supvisors** logger level.
         
         * Application state is evaluated only against the starting sequence of its processes.
         
-        * Fixed blocking issue when *Master* is stopped while in ``DEPLOYMENT`` state.
+        * Fixed blocking issue when *Master* is stopped while in `DEPLOYMENT` state.
         
-        * Fixed issue with applications that would not fully stop when using the ``STOP_APPLICATION`` starting failure strategy.
+        * Fixed issue with applications that would not fully stop when using the `STOP_APPLICATION` starting failure strategy.
         
-        * Fixed issue related to `Issue #85 <https://github.com/julien6387/supvisors/issues/85>`_.
-          An exception was raised when the program ``procnum`` was greater than the list of applicable nodes.
+        * Fixed issue related to [Issue #85](https://github.com/julien6387/supvisors/issues/85).
+          An exception was raised when the program `procnum` was greater than the list of applicable nodes.
         
-        * Fixed `Issue #91 <https://github.com/julien6387/supvisors/issues/91>`_.
+        * Fixed [Issue #91](https://github.com/julien6387/supvisors/issues/91).
           Fix CSS style on the process tables in HTML.
         
-        * Fixed `Issue #90 <https://github.com/julien6387/supvisors/issues/90>`_.
-          The **Supvisors** *Master* node drives the transition to ``OPERATION``.
+        * Fixed [Issue #90](https://github.com/julien6387/supvisors/issues/90).
+          The **Supvisors** *Master* node drives the transition to `OPERATION`.
         
-        * In the Web UI, set the process state color to ``FATAL`` when the process has exited unexpectedly.
+        * In the Web UI, set the process state color to `FATAL` when the process has exited unexpectedly.
         
-        * Change the default expected loading to ``0`` in the program rules.
+        * Change the default expected loading to `0` in the program rules.
         
-        * Python ``Enum`` used for enumerations (not available in Python 2.7).
+        * Python `Enum` used for enumerations (not available in Python 2.7).
         
-        * Remove ``supvisors_shortcuts`` from source code to get rid of IDE warnings.
+        * Remove `supvisors_shortcuts` from source code to get rid of IDE warnings.
         
-        * All unit tests updated from ``unittest`` to ``pytest``.
+        * All unit tests updated from `unittest` to `pytest`.
         
         * Include this Change Log to documentation.
         
         * Documentation updated.
         
         
-        0.5 (2021-03-01)
-        ----------------
+        ## 0.5 (2021-03-01)
         
-        * New option ``force_synchro_if`` to force the end of the synchronization phase when a subset of nodes are active.
+        * New option `force_synchro_if` to force the end of the synchronization phase when a subset of nodes are active.
         
-        * New starting strategy ``LOCAL`` added to command the starting of an application on the local node only.
+        * New starting strategy `LOCAL` added to command the starting of an application on the local node only.
         
-        * Fixed `Issue #87 <https://github.com/julien6387/supvisors/issues/87>`_.
+        * Fixed [Issue #87](https://github.com/julien6387/supvisors/issues/87).
           Under particular circumstances, **Supvisors** could have multiple *Master* nodes.
         
-        * Fixed `Issue #86 <https://github.com/julien6387/supvisors/issues/86>`_.
+        * Fixed [Issue #86](https://github.com/julien6387/supvisors/issues/86).
           The starting and stopping sequences may fail and block when a sub-sequence includes only failed programs.
         
-        * Fixed `Issue #85 <https://github.com/julien6387/supvisors/issues/85>`_.
-          When using ``#`` in the ``address_list`` program rule of the **Supvisors** rules file, a subset of nodes can optionally be defined.
+        * Fixed [Issue #85](https://github.com/julien6387/supvisors/issues/85).
+          When using `#` in the `address_list` program rule of the **Supvisors** rules file, a subset of nodes can optionally be defined.
         
-        * Fixed `Issue #84 <https://github.com/julien6387/supvisors/issues/84>`_.
+        * Fixed [Issue #84](https://github.com/julien6387/supvisors/issues/84).
           In the **Supvisors** rules file, program rules can be defined using both model reference and attributes.
         
         * The Web UI uses the default starting strategy of the configuration file.
         
         * The layout of Web UI statistics sections has been rearranged.
         
-        * Fixed CSS style missing for ``CHECKING`` node state in tables.
+        * Fixed CSS style missing for `CHECKING` node state in tables.
         
         * Star added to the node box of the *Master* instance on the main page.
         
         * Type annotations are added progressively in source code.
         
-        * Start switching from ``unittest`` to ``pytest``.
+        * Start switching from `unittest` to `pytest`.
         
-        * Logs (especially ``debug`` and ``trace``) updated to remove printed objects.
+        * Logs (especially `debug` and `trace`) updated to remove printed objects.
         
         * Documentation updated.
         
         
-        0.4 (2021-02-14)
-        ----------------
+        ## 0.4 (2021-02-14)
         
         * Auto-refresh button added to all pages.
         
         * Web UI Main page reworked by adding a subdivision of application in node boxes.
         
-        * Fixed exception when exiting using ``Ctrl+c`` from shell.
+        * Fixed exception when exiting using `Ctrl+c` from shell.
         
         * Fixed exception when rules files is not provided.
         
         * Documentation updated.
         
         
-        0.3 (2020-12-29)
-        ----------------
+        ## 0.3 (2020-12-29)
         
-        * Fixed `Issue #81 <https://github.com/julien6387/supvisors/issues/81>`_.
-          When **Supvisors** logfile is set to ``AUTO``, **Supvisors** uses the same logger as **Supervisor**.
+        * Fixed [Issue #81](https://github.com/julien6387/supvisors/issues/81).
+          When **Supvisors** logfile is set to `AUTO`, **Supvisors** uses the same logger as **Supervisor**.
         
-        * Fixed `Issue #79 <https://github.com/julien6387/supvisors/issues/79>`_.
-          When ``FATAL`` or ``UNKNOWN`` Process state is forced by **Supvisors**, ``spawnerr`` was missing in the listener payload.
+        * Fixed [Issue #79](https://github.com/julien6387/supvisors/issues/79).
+          When `FATAL` or `UNKNOWN` Process state is forced by **Supvisors**, `spawnerr` was missing in the listener payload.
         
-        * Useless folder ``rsc_ref`` deleted.
+        * Useless folder `rsc_ref` deleted.
         
-        * ``design`` folder moved to a dedicated *GitHub* repository.
+        * `design` folder moved to a dedicated *GitHub* repository.
         
         * 100% coverage reached in unit tests.
         
         * Documentation updated.
         
         
-        0.2 (2020-12-14)
-        ----------------
+        ## 0.2 (2020-12-14)
         
         * Migration to **Python 3.6**.
           Versions of dependencies are refreshed, more particularly **Supervisor 4.2.1**.
         
         * CSS of Web UI updated / simplified.
         
-        * New action added to Host Process page of WebUI: ``tail -f stderr`` button.
+        * New action added to Host Process page of WebUI: `tail -f stderr` button.
         
         * New information actions added to Application page of WebUI:
         
-            * ``description`` field.
-            * ``clear logs``, ``tail -f stdout``, ``tail -f stderr`` buttons.
+            * `description` field.
+            * `clear logs`, `tail -f stdout`, `tail -f stderr` buttons.
         
-        * Fixed `Issue #75 <https://github.com/julien6387/supvisors/issues/75>`_.
-          **Supvisors** takes into account the ``username`` and the ``password`` of ``inet_http_server`` in the ``supervisord`` section.
+        * Fixed [Issue #75](https://github.com/julien6387/supvisors/issues/75).
+          **Supvisors** takes into account the `username` and the `password` of `inet_http_server` in the `supervisord` section.
         
-        * Fixed `Issue #17 <https://github.com/julien6387/supvisors/issues/17>`_.
+        * Fixed [Issue #17](https://github.com/julien6387/supvisors/issues/17).
           The user selections on the web UI are passed to the URL.
         
-        * Fixed `Issue #72 <https://github.com/julien6387/supvisors/issues/72>`_.
+        * Fixed [Issue #72](https://github.com/julien6387/supvisors/issues/72).
           The extra arguments are shared between all **Supvisors** instances.
         
-        * ``README.rst`` replaced with ``README.md``.
+        * `README.rst` replaced with `README.md`.
         
         * Coverage improved in tests.
         
         * Docs target added to Travis-CI.
         
         * Documentation formatting issues fixed.
         
         
-        0.1 (2017-08-11)
-        ----------------
+        ## 0.1 (2017-08-11)
         
         Initial release.
         
 Platform: CentOS 8.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `supvisors-0.8/supvisors.egg-info/SOURCES.txt` & `supvisors-0.9/supvisors.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,27 +38,29 @@
 supvisors/viewprocaddress.py
 supvisors/viewsupstatus.py
 supvisors/viewsupvisors.py
 supvisors/webutils.py
 supvisors.egg-info/PKG-INFO
 supvisors.egg-info/SOURCES.txt
 supvisors.egg-info/dependency_links.txt
+supvisors.egg-info/entry_points.txt
 supvisors.egg-info/namespace_packages.txt
 supvisors.egg-info/not-zip-safe
 supvisors.egg-info/requires.txt
 supvisors.egg-info/top_level.txt
 supvisors/client/__init__.py
 supvisors/client/subscriber.py
 supvisors/tests/__init__.py
 supvisors/tests/base.py
 supvisors/tests/configurations.py
 supvisors/tests/conftest.py
 supvisors/tests/test_address.py
 supvisors/tests/test_addressmapper.py
 supvisors/tests/test_application.py
+supvisors/tests/test_breed.py
 supvisors/tests/test_commander.py
 supvisors/tests/test_context.py
 supvisors/tests/test_infosource.py
 supvisors/tests/test_initializer.py
 supvisors/tests/test_listener.py
 supvisors/tests/test_mainloop.py
 supvisors/tests/test_options.py
```

### Comparing `supvisors-0.8/LICENSE` & `supvisors-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/README.md` & `supvisors-0.9/README.md`

 * *Files identical despite different names*

### Comparing `supvisors-0.8/setup.py` & `supvisors-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 xml_valid_require = ['lxml >= 4.6.2']
 
 testing_extras = ['pytest >= 2.5.2', 'pytest-cov']
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
     README = open(os.path.join(here, 'README.md')).read()
-    CHANGES = open(os.path.join(here, 'CHANGES.rst')).read()
+    CHANGES = open(os.path.join(here, 'CHANGES.md')).read()
 except:
     README = """Supvisors is a control system for distributed applications over multiple Supervisor instances. """
     CHANGES = ''
 
 CLASSIFIERS = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 5 - Production/Stable",
@@ -80,8 +80,10 @@
                     'xml_valid': xml_valid_require,
                     'all': ip_require + statistics_require + xml_valid_require,
                     'testing': testing_extras},
     include_package_data=True,
     zip_safe=False,
     namespace_packages=['supvisors'],
     test_suite="supvisors.tests",
+    entry_points={'console_scripts': ['supvisorsctl = supvisors.supvisorsctl:main',
+                                      'supvisors_breed = supvisors.tools.breed:main']}
 )
```

### Comparing `supvisors-0.8/PKG-INFO` & `supvisors-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: supvisors
-Version: 0.8
+Version: 0.9
 Summary: A Control System for Distributed Applications
 Home-page: https://github.com/julien6387/supvisors
 Author: Julien Le Cléach
 Author-email: julien.6387.dev@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/julien6387/supvisors/archive/0.8.tar.gz
+Download-URL: https://github.com/julien6387/supvisors/archive/0.9.tar.gz
 Description: # **Supvisors**
         [![PyPI version][pypi-image]][pypi-url] [![Build Status][ci-image]][ci-url] [![Coverage Status][coveralls-image]][coveralls-url] [![Documentation Status][docs-image]][docs-url]
         
         
         **Supvisors** is a Control System for Distributed Applications, based on
         multiple instances of Supervisor.
         
@@ -105,45 +105,77 @@
         [coveralls-image]: https://coveralls.io/repos/github/julien6387/supvisors/badge.svg?branch=master
         [coveralls-url]: https://coveralls.io/github/julien6387/supvisors?branch=master
         
         [docs-image]: https://readthedocs.org/projects/supvisors/badge/?version=master
         [docs-url]: https://supvisors.readthedocs.io/en/master
         
         
-        Change Log
-        ==========
+        # Change Log
         
-        0.8 (2021-08-22)
-        ----------------
+        ## 0.9 (2021-08-31)
         
-        * Fixed exception in ``INITIALIZATION`` state when the *Master* declared by other nodes is not RUNNING yet and
+        * Enable the hash '#' for the `addresses` of a non-distributed application.
+        
+        * Add `supvisorsctl` to pally the lack of support of `supervisorctl` when used with `--serverurl URL` option.
+          See related [Supervisor Issue #1455](https://github.com/Supervisor/supervisor/issues/1455).
+        
+        * Provide `breed.py` as a binary of **Supvisors**: `supvisors_breed`.
+          The script only considers group duplication as it is fully valid to include multiple times a program definition
+          in several groups.
+        
+        * Move the contents of the `[supvisors]` section into the `[rpcinterface:supvisors]` section and benefit from the
+          configuration structure provided by Supervisor. The `[supvisors]` section itself is thus obsolete.
+        
+        * Remove deprecated support of `pattern` elements.
+        
+        * Fixed issue when using the Web UI Application page from a previous launch.
+        
+        * Invert the stop sequence logic, starting from the greatest ``stop_sequence`` number to the lowest one.
+        
+        * When ``stop_sequence`` is not set in the rules files, it is defaulted to the ``start_sequence`` value.
+          With the new stop sequence logic, the stop sequence is by default exactly the opposite of the start sequence.
+        
+        * Fixed Nodes column width for `supervisorctl application_rules`.
+        
+        * `CHANGES.rst` replaced with `CHANGES.md`.
+        
+        * 'Scenario 3' has been added to the **Supvisors** use cases.
+        
+        * A 'Gathering' configuration has been added to the **Supvisors** use cases. It combines all uses cases.
+        
+        * Update documentation.
+        
+        
+        ## 0.8 (2021-08-22)
+        
+        * Fixed exception in `INITIALIZATION` state when the *Master* declared by other nodes is not RUNNING yet and
           the *core nodes* are RUNNING.
         
         * Fixed exception when program rules and extra arguments are tested against a program unknown to the local Supervisor.
         
         * Fixed issue about program patterns that were applicable to all elements. The scope of program patterns is now limited
           to their owner application.
         
         * Fixed issue with infinite tries of application restart when the process cannot be started due to a lack of resources
-          and ``RESTART_APPLICATION`` is set on the program in the **Supvisors** rules file.
+          and `RESTART_APPLICATION` is set on the program in the **Supvisors** rules file.
         
         * Fixed issue about application state not updated after a node has become silent.
         
-        * Fixed issue when choosing a node in ``Starter``. Apply the requests that have not been satisfied yet for
+        * Fixed issue when choosing a node in `Starter`. Apply the requests that have not been satisfied yet for
           non-distributed applications.
         
         * Logic for application major / minor failures reviewed.
         
         * Simplify the insertion of applications to start or stop in Commander jobs.
         
         * In the rules file, support for application patterns has been added.
         
-        * In the rules file, ``pattern`` elements are **deprecated** and are replaced by ``program`` elements with a ``pattern``
-          attribute instead of a ``name`` attribute.
-          Support for ``pattern`` elements will be removed in the next version of **Supvisors**.
+        * In the rules file, `pattern` elements are **deprecated** and are replaced by `program` elements with a `pattern`
+          attribute instead of a `name` attribute.
+          Support for `pattern` elements will be removed in the next version of **Supvisors**.
         
         * Node aliases have been added to the rules file.
         
         * Add the current node to all pages of Web UI to be aware of the node that displays the page.
         
         * The Web UI is updated to handle a large list of applications, nodes, processor cores and network interfaces.
         
@@ -154,226 +186,219 @@
           has raised a failure.
         
         * In the Application page of the Web UI, default starting strategy is the starting strategy defined in the rules file
           for the application considered.
         
         * In the Application ang Process page, the detailed process statistics can be deselected.
         
-        * Titles added to the output of :program:`supervisorctl` ``address_status`` and ``application_info``.
+        * Titles added to the output of :program:`supervisorctl` `address_status` and `application_info`.
         
-        * The XML schema has been moved to a separate file ``rules.xsd``.
+        * The XML schema has been moved to a separate file `rules.xsd`.
         
         * Remove dependency to *netifaces* as *psutil* provides the function.
         
-        * Scenario 2 has been added to the **Supvisors** use cases.
+        * 'Scenario 2' has been added to the **Supvisors** use cases.
         
-        * A script ``breed.py`` has been added to the install package.
+        * A script `breed.py` has been added to the install package.
           It can be used to duplicate the applications based on a template configuration and more particularly used to prepare
           the Scenario 2 of the **Supvisors** use cases.
         
         * Update documentation.
         
         
-        0.7 (2021-08-15)
-        ----------------
+        ## 0.7 (2021-08-15)
         
-        * Fixed `Issue #92 <https://github.com/julien6387/supvisors/issues/92>`_.
+        * Fixed [Issue #92](https://github.com/julien6387/supvisors/issues/92).
           The *Master* drives the state of all **Supvisors** instances and a simplified state machine has been assigned
           to non-master **Supvisors** instances. The loss of the *Master* instance is managed in all relevant states.
         
-        * Fixed issue about applications that would be started automatically whereas their ``start_sequence`` is 0.
+        * Fixed issue about applications that would be started automatically whereas their `start_sequence` is 0.
           The regression has been introduced during the implementation of applications repair in **Supvisors 0.6**.
         
         * Enable stop sequence on *Unmanaged* applications.
         
         * In the application navigation menu of the Web UI, add a red light to applications having raised a failure.
         
-        * New application rules ``distributed`` and ``addresses`` added to the **Supvisors** rules file.
+        * New application rules `distributed` and `addresses` added to the **Supvisors** rules file.
           Non-distributed applications have all their processes started on the same node chosen in accordance with the
-          ``addresses`` and the ``starting_strategy``.
+          `addresses` and the `starting_strategy`.
         
         * Starting strategy added to the application rules.
         
-        * Fixed issue when choosing a node in ``Starter``. The starting strategies considers the current load of the nodes
+        * Fixed issue when choosing a node in `Starter`. The starting strategies considers the current load of the nodes
           and includes the requests that have not been satisfied yet.
         
-        * Fixed issue with infinite process restart when the process crashes and ``RESTART_PROCESS`` is set on the program
-          in the **Supvisors** rules file. When the process crashes, only the *Supervisor* ``autorestart`` applies.
-          The **Supvisors** ``RESTART_PROCESS`` applies only when the node becomes inactive.
+        * Fixed issue with infinite process restart when the process crashes and `RESTART_PROCESS` is set on the program
+          in the **Supvisors** rules file. When the process crashes, only the *Supervisor* `autorestart` applies.
+          The **Supvisors** `RESTART_PROCESS` applies only when the node becomes inactive.
         
         * Fixed exception when forcing the state on a process that is unknown to the local Supervisor.
         
-        * Promote the ``RESTART_PROCESS`` into ``RESTART_APPLICATION`` if the application is stopped.
+        * Promote the `RESTART_PROCESS` into `RESTART_APPLICATION` if the application is stopped.
         
-        * For the *Master* election, give a priority to nodes declared in the ``forced_synchro_if`` option if used.
+        * For the *Master* election, give a priority to nodes declared in the `forced_synchro_if` option if used.
         
-        * When using the ``forced_synchro_if`` option and when ``auto_fence`` is activated, do not isolate nodes as long as
-          ``synchro_timeout`` has not passed.
+        * When using the `forced_synchro_if` option and when `auto_fence` is activated, do not isolate nodes as long as
+          `synchro_timeout` has not passed.
         
-        * In the ``INITALIZATION`` state, skip the synchronization phase upon notification of a known *Master* and adopt it.
+        * In the `INITALIZATION` state, skip the synchronization phase upon notification of a known *Master* and adopt it.
         
-        * Add reciprocity to isolation even if ``auto_fence`` is not activated.
+        * Add reciprocity to isolation even if `auto_fence` is not activated.
         
         * In the process description of the Web UI Application page, add information about the node name.
           In particular, it is useful to know where the process was running when it is stopped.
         
         * Start adding use cases to documentation, inspired by real examples.
-          Scenario 1 has been added.
+          'Scenario 1' has been added.
         
         * Documentation updated.
         
         
-        0.6 (2021-08-01)
-        ----------------
+        ## 0.6 (2021-08-01)
         
         * Applications that are not declared in the rules file are not *managed*.
           *Unmanaged* applications have no start/stop sequence, no state and status (always STOPPED) and **Supvisors**
           does not raise a conflict if multiple instances are running over multiple nodes.
         
         * Improve **Supvisors** stability when dealing with remote programs undefined locally.
         
-        * Add expand / shrink actions to applications to the ``ProcAddressView`` of the Web UI.
+        * Add expand / shrink actions to applications to the `ProcAddressView` of the Web UI.
         
-        * Upon authorization of a new node in **Supvisors**, back to ``DEPLOYMENT`` state to repair applications.
+        * Upon authorization of a new node in **Supvisors**, back to `DEPLOYMENT` state to repair applications.
         
-        * Add RPC ``change_log_level`` to dynamically change the **Supvisors** logger level.
+        * Add RPC `change_log_level` to dynamically change the **Supvisors** logger level.
         
         * Application state is evaluated only against the starting sequence of its processes.
         
-        * Fixed blocking issue when *Master* is stopped while in ``DEPLOYMENT`` state.
+        * Fixed blocking issue when *Master* is stopped while in `DEPLOYMENT` state.
         
-        * Fixed issue with applications that would not fully stop when using the ``STOP_APPLICATION`` starting failure strategy.
+        * Fixed issue with applications that would not fully stop when using the `STOP_APPLICATION` starting failure strategy.
         
-        * Fixed issue related to `Issue #85 <https://github.com/julien6387/supvisors/issues/85>`_.
-          An exception was raised when the program ``procnum`` was greater than the list of applicable nodes.
+        * Fixed issue related to [Issue #85](https://github.com/julien6387/supvisors/issues/85).
+          An exception was raised when the program `procnum` was greater than the list of applicable nodes.
         
-        * Fixed `Issue #91 <https://github.com/julien6387/supvisors/issues/91>`_.
+        * Fixed [Issue #91](https://github.com/julien6387/supvisors/issues/91).
           Fix CSS style on the process tables in HTML.
         
-        * Fixed `Issue #90 <https://github.com/julien6387/supvisors/issues/90>`_.
-          The **Supvisors** *Master* node drives the transition to ``OPERATION``.
+        * Fixed [Issue #90](https://github.com/julien6387/supvisors/issues/90).
+          The **Supvisors** *Master* node drives the transition to `OPERATION`.
         
-        * In the Web UI, set the process state color to ``FATAL`` when the process has exited unexpectedly.
+        * In the Web UI, set the process state color to `FATAL` when the process has exited unexpectedly.
         
-        * Change the default expected loading to ``0`` in the program rules.
+        * Change the default expected loading to `0` in the program rules.
         
-        * Python ``Enum`` used for enumerations (not available in Python 2.7).
+        * Python `Enum` used for enumerations (not available in Python 2.7).
         
-        * Remove ``supvisors_shortcuts`` from source code to get rid of IDE warnings.
+        * Remove `supvisors_shortcuts` from source code to get rid of IDE warnings.
         
-        * All unit tests updated from ``unittest`` to ``pytest``.
+        * All unit tests updated from `unittest` to `pytest`.
         
         * Include this Change Log to documentation.
         
         * Documentation updated.
         
         
-        0.5 (2021-03-01)
-        ----------------
+        ## 0.5 (2021-03-01)
         
-        * New option ``force_synchro_if`` to force the end of the synchronization phase when a subset of nodes are active.
+        * New option `force_synchro_if` to force the end of the synchronization phase when a subset of nodes are active.
         
-        * New starting strategy ``LOCAL`` added to command the starting of an application on the local node only.
+        * New starting strategy `LOCAL` added to command the starting of an application on the local node only.
         
-        * Fixed `Issue #87 <https://github.com/julien6387/supvisors/issues/87>`_.
+        * Fixed [Issue #87](https://github.com/julien6387/supvisors/issues/87).
           Under particular circumstances, **Supvisors** could have multiple *Master* nodes.
         
-        * Fixed `Issue #86 <https://github.com/julien6387/supvisors/issues/86>`_.
+        * Fixed [Issue #86](https://github.com/julien6387/supvisors/issues/86).
           The starting and stopping sequences may fail and block when a sub-sequence includes only failed programs.
         
-        * Fixed `Issue #85 <https://github.com/julien6387/supvisors/issues/85>`_.
-          When using ``#`` in the ``address_list`` program rule of the **Supvisors** rules file, a subset of nodes can optionally be defined.
+        * Fixed [Issue #85](https://github.com/julien6387/supvisors/issues/85).
+          When using `#` in the `address_list` program rule of the **Supvisors** rules file, a subset of nodes can optionally be defined.
         
-        * Fixed `Issue #84 <https://github.com/julien6387/supvisors/issues/84>`_.
+        * Fixed [Issue #84](https://github.com/julien6387/supvisors/issues/84).
           In the **Supvisors** rules file, program rules can be defined using both model reference and attributes.
         
         * The Web UI uses the default starting strategy of the configuration file.
         
         * The layout of Web UI statistics sections has been rearranged.
         
-        * Fixed CSS style missing for ``CHECKING`` node state in tables.
+        * Fixed CSS style missing for `CHECKING` node state in tables.
         
         * Star added to the node box of the *Master* instance on the main page.
         
         * Type annotations are added progressively in source code.
         
-        * Start switching from ``unittest`` to ``pytest``.
+        * Start switching from `unittest` to `pytest`.
         
-        * Logs (especially ``debug`` and ``trace``) updated to remove printed objects.
+        * Logs (especially `debug` and `trace`) updated to remove printed objects.
         
         * Documentation updated.
         
         
-        0.4 (2021-02-14)
-        ----------------
+        ## 0.4 (2021-02-14)
         
         * Auto-refresh button added to all pages.
         
         * Web UI Main page reworked by adding a subdivision of application in node boxes.
         
-        * Fixed exception when exiting using ``Ctrl+c`` from shell.
+        * Fixed exception when exiting using `Ctrl+c` from shell.
         
         * Fixed exception when rules files is not provided.
         
         * Documentation updated.
         
         
-        0.3 (2020-12-29)
-        ----------------
+        ## 0.3 (2020-12-29)
         
-        * Fixed `Issue #81 <https://github.com/julien6387/supvisors/issues/81>`_.
-          When **Supvisors** logfile is set to ``AUTO``, **Supvisors** uses the same logger as **Supervisor**.
+        * Fixed [Issue #81](https://github.com/julien6387/supvisors/issues/81).
+          When **Supvisors** logfile is set to `AUTO`, **Supvisors** uses the same logger as **Supervisor**.
         
-        * Fixed `Issue #79 <https://github.com/julien6387/supvisors/issues/79>`_.
-          When ``FATAL`` or ``UNKNOWN`` Process state is forced by **Supvisors**, ``spawnerr`` was missing in the listener payload.
+        * Fixed [Issue #79](https://github.com/julien6387/supvisors/issues/79).
+          When `FATAL` or `UNKNOWN` Process state is forced by **Supvisors**, `spawnerr` was missing in the listener payload.
         
-        * Useless folder ``rsc_ref`` deleted.
+        * Useless folder `rsc_ref` deleted.
         
-        * ``design`` folder moved to a dedicated *GitHub* repository.
+        * `design` folder moved to a dedicated *GitHub* repository.
         
         * 100% coverage reached in unit tests.
         
         * Documentation updated.
         
         
-        0.2 (2020-12-14)
-        ----------------
+        ## 0.2 (2020-12-14)
         
         * Migration to **Python 3.6**.
           Versions of dependencies are refreshed, more particularly **Supervisor 4.2.1**.
         
         * CSS of Web UI updated / simplified.
         
-        * New action added to Host Process page of WebUI: ``tail -f stderr`` button.
+        * New action added to Host Process page of WebUI: `tail -f stderr` button.
         
         * New information actions added to Application page of WebUI:
         
-            * ``description`` field.
-            * ``clear logs``, ``tail -f stdout``, ``tail -f stderr`` buttons.
+            * `description` field.
+            * `clear logs`, `tail -f stdout`, `tail -f stderr` buttons.
         
-        * Fixed `Issue #75 <https://github.com/julien6387/supvisors/issues/75>`_.
-          **Supvisors** takes into account the ``username`` and the ``password`` of ``inet_http_server`` in the ``supervisord`` section.
+        * Fixed [Issue #75](https://github.com/julien6387/supvisors/issues/75).
+          **Supvisors** takes into account the `username` and the `password` of `inet_http_server` in the `supervisord` section.
         
-        * Fixed `Issue #17 <https://github.com/julien6387/supvisors/issues/17>`_.
+        * Fixed [Issue #17](https://github.com/julien6387/supvisors/issues/17).
           The user selections on the web UI are passed to the URL.
         
-        * Fixed `Issue #72 <https://github.com/julien6387/supvisors/issues/72>`_.
+        * Fixed [Issue #72](https://github.com/julien6387/supvisors/issues/72).
           The extra arguments are shared between all **Supvisors** instances.
         
-        * ``README.rst`` replaced with ``README.md``.
+        * `README.rst` replaced with `README.md`.
         
         * Coverage improved in tests.
         
         * Docs target added to Travis-CI.
         
         * Documentation formatting issues fixed.
         
         
-        0.1 (2017-08-11)
-        ----------------
+        ## 0.1 (2017-08-11)
         
         Initial release.
         
 Platform: CentOS 8.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

