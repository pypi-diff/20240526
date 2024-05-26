# Comparing `tmp/pygenda-0.3.2.tar.gz` & `tmp/pygenda-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenda-0.3.2.tar", last modified: Thu May 16 20:25:28 2024, max compression
+gzip compressed data, was "pygenda-0.3.3.tar", last modified: Sun May 26 08:27:50 2024, max compression
```

## Comparing `pygenda-0.3.2.tar` & `pygenda-0.3.3.tar`

### file list

```diff
@@ -1,65 +1,102 @@
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.682020 pygenda-0.3.2/
--rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.3.2/COPYING
--rw-------   0 matt      (1000) users      (100)      275 2023-12-30 00:19:21.000000 pygenda-0.3.2/MANIFEST.in
--rw-------   0 matt      (1000) users      (100)     1015 2024-05-16 20:25:28.682020 pygenda-0.3.2/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     6363 2023-12-30 00:19:21.000000 pygenda-0.3.2/README.md
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.667019 pygenda-0.3.2/csrc/
--rw-------   0 matt      (1000) users      (100)      814 2023-12-30 00:19:21.000000 pygenda-0.3.2/csrc/CMakeLists.txt
--rw-------   0 matt      (1000) users      (100)     3043 2023-12-30 00:19:21.000000 pygenda-0.3.2/csrc/pygenda_clipboard.c
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.675020 pygenda-0.3.2/pygenda/
--rwx------   0 matt      (1000) users      (100)      823 2024-01-04 12:29:50.000000 pygenda-0.3.2/pygenda/__main__.py
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.676020 pygenda-0.3.2/pygenda/app/
--rw-------   0 matt      (1000) users      (100)      369 2023-12-30 00:19:21.000000 pygenda-0.3.2/pygenda/app/pygenda.desktop
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.678020 pygenda-0.3.2/pygenda/css/
--rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/disc+loop+star.svg
--rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/disc+loop.svg
--rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/disc+star.svg
--rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/disc.svg
--rw-------   0 matt      (1000) users      (100)     3876 2023-12-30 00:19:21.000000 pygenda-0.3.2/pygenda/css/gemini.css
--rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/loop+star.svg
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/loop.svg
--rw-------   0 matt      (1000) users      (100)    16437 2024-05-16 19:11:36.000000 pygenda-0.3.2/pygenda/css/pygenda.css
--rw-------   0 matt      (1000) users      (100)      103 2023-10-06 15:06:24.000000 pygenda-0.3.2/pygenda/css/raspberrypi.css
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.2/pygenda/css/star.svg
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.678020 pygenda-0.3.2/pygenda/locale/
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.666020 pygenda-0.3.2/pygenda/locale/en_US/
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.679020 pygenda-0.3.2/pygenda/locale/en_US/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)      536 2024-05-07 21:14:12.000000 pygenda-0.3.2/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.666020 pygenda-0.3.2/pygenda/locale/fr/
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.680019 pygenda-0.3.2/pygenda/locale/fr/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)    10493 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.666020 pygenda-0.3.2/pygenda/locale/nl/
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.680019 pygenda-0.3.2/pygenda/locale/nl/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)    10366 2024-05-10 21:19:03.000000 pygenda-0.3.2/pygenda/locale/nl/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)    14753 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/locale/pygenda.pot
--rw-------   0 matt      (1000) users      (100)    83718 2024-05-16 19:11:44.000000 pygenda-0.3.2/pygenda/pygenda_calendar.py
--rw-------   0 matt      (1000) users      (100)     5805 2023-12-30 00:19:21.000000 pygenda-0.3.2/pygenda/pygenda_config.py
--rw-------   0 matt      (1000) users      (100)    11782 2024-05-04 14:34:56.000000 pygenda-0.3.2/pygenda/pygenda_dialog_entryprops.py
--rw-------   0 matt      (1000) users      (100)    75600 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/pygenda_dialog_event.py
--rw-------   0 matt      (1000) users      (100)     3447 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/pygenda_dialog_find.py
--rw-------   0 matt      (1000) users      (100)     9450 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/pygenda_dialog_import.py
--rw-------   0 matt      (1000) users      (100)    15266 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/pygenda_dialog_todo.py
--rw-------   0 matt      (1000) users      (100)     4656 2024-01-09 10:40:12.000000 pygenda-0.3.2/pygenda/pygenda_entryinfo.py
--rw-------   0 matt      (1000) users      (100)    46290 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/pygenda_gui.py
--rw-------   0 matt      (1000) users      (100)    11647 2024-05-04 14:36:15.000000 pygenda-0.3.2/pygenda/pygenda_util.py
--rw-------   0 matt      (1000) users      (100)      300 2024-05-16 19:12:31.000000 pygenda-0.3.2/pygenda/pygenda_version.py
--rw-------   0 matt      (1000) users      (100)    16272 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/pygenda_view.py
--rw-------   0 matt      (1000) users      (100)    27322 2024-05-08 13:50:17.000000 pygenda-0.3.2/pygenda/pygenda_view_todo.py
--rw-------   0 matt      (1000) users      (100)    22946 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/pygenda_view_week.py
--rw-------   0 matt      (1000) users      (100)    29080 2024-03-01 19:43:53.000000 pygenda-0.3.2/pygenda/pygenda_view_year.py
--rw-------   0 matt      (1000) users      (100)    22109 2023-12-30 00:19:21.000000 pygenda-0.3.2/pygenda/pygenda_widgets.py
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.682020 pygenda-0.3.2/pygenda/ui/
--rw-------   0 matt      (1000) users      (100)    45184 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/ui/dialog_event.ui
--rw-------   0 matt      (1000) users      (100)     5147 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/ui/dialog_find.ui
--rw-------   0 matt      (1000) users      (100)    14665 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/ui/dialog_todo.ui
--rw-------   0 matt      (1000) users      (100)    33513 2024-02-25 09:30:13.000000 pygenda-0.3.2/pygenda/ui/main.ui
--rw-------   0 matt      (1000) users      (100)     3889 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/ui/view_week.ui
--rw-------   0 matt      (1000) users      (100)     5928 2024-01-01 08:53:19.000000 pygenda-0.3.2/pygenda/ui/view_year.ui
-drwx------   0 matt      (1000) users      (100)        0 2024-05-16 20:25:28.676020 pygenda-0.3.2/pygenda.egg-info/
--rw-------   0 matt      (1000) users      (100)     1015 2024-05-16 20:25:28.000000 pygenda-0.3.2/pygenda.egg-info/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     1290 2024-05-16 20:25:28.000000 pygenda-0.3.2/pygenda.egg-info/SOURCES.txt
--rw-------   0 matt      (1000) users      (100)        1 2024-05-16 20:25:28.000000 pygenda-0.3.2/pygenda.egg-info/dependency_links.txt
--rw-------   0 matt      (1000) users      (100)       67 2024-05-16 20:25:28.000000 pygenda-0.3.2/pygenda.egg-info/requires.txt
--rw-------   0 matt      (1000) users      (100)        8 2024-05-16 20:25:28.000000 pygenda-0.3.2/pygenda.egg-info/top_level.txt
--rw-------   0 matt      (1000) users      (100)       38 2024-05-16 20:25:28.682020 pygenda-0.3.2/setup.cfg
--rwx------   0 matt      (1000) users      (100)     3892 2024-01-05 22:31:04.000000 pygenda-0.3.2/setup.py
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.218362 pygenda-0.3.3/
+-rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.3.3/COPYING
+-rw-r--r--   0 matt      (1000) users      (100)     1230 2024-05-26 08:27:50.218362 pygenda-0.3.3/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     6459 2024-05-26 08:16:44.000000 pygenda-0.3.3/README.md
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.188362 pygenda-0.3.3/csrc/
+-rw-------   0 matt      (1000) users      (100)       79 2023-12-30 00:19:21.000000 pygenda-0.3.3/csrc/.gitignore
+-rw-------   0 matt      (1000) users      (100)      814 2024-05-19 07:51:55.000000 pygenda-0.3.3/csrc/CMakeLists.txt
+-rw-------   0 matt      (1000) users      (100)     3043 2023-12-30 00:19:21.000000 pygenda-0.3.3/csrc/pygenda_clipboard.c
+-rw-------   0 matt      (1000) users      (100)      338 2024-05-26 08:16:44.000000 pygenda-0.3.3/description.md
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.191362 pygenda-0.3.3/docs/
+-rw-------   0 matt      (1000) users      (100)     4279 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/CalDAV.md
+-rw-------   0 matt      (1000) users      (100)     4343 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/Contributing.md
+-rw-------   0 matt      (1000) users      (100)     5798 2024-05-26 08:21:49.000000 pygenda-0.3.3/docs/Development.md
+-rw-------   0 matt      (1000) users      (100)     4521 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/Evolution_Data_Server.md
+-rw-------   0 matt      (1000) users      (100)     3624 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/Usage.md
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.193362 pygenda-0.3.3/docs/config-examples/
+-rw-------   0 matt      (1000) users      (100)      873 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/config-examples/README.md
+-rw-------   0 matt      (1000) users      (100)     2532 2023-07-06 18:45:26.000000 pygenda-0.3.3/docs/config-examples/backgrounds.css
+-rw-------   0 matt      (1000) users      (100)     6205 2023-03-31 11:03:09.000000 pygenda-0.3.3/docs/config-examples/darkmode.css
+-rw-------   0 matt      (1000) users      (100)     8329 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/config-examples/defaults.ini
+-rw-------   0 matt      (1000) users      (100)      455 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/config-examples/gemini.ini
+-rw-------   0 matt      (1000) users      (100)    12600 2024-05-26 08:16:44.000000 pygenda-0.3.3/docs/known_issues.md
+-rw-------   0 matt      (1000) users      (100)     7315 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/quickstart-debianlike.md
+-rw-------   0 matt      (1000) users      (100)    10867 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/quickstart-geminipda.md
+-rw-------   0 matt      (1000) users      (100)     9294 2024-05-19 07:51:55.000000 pygenda-0.3.3/docs/quickstart-postmarketOS.md
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.196362 pygenda-0.3.3/docs/screenshots/
+-rw-------   0 matt      (1000) users      (100)    17045 2023-12-30 00:19:21.000000 pygenda-0.3.3/docs/screenshots/todo_view.png
+-rw-------   0 matt      (1000) users      (100)    16198 2023-12-30 00:19:21.000000 pygenda-0.3.3/docs/screenshots/week_view.png
+-rw-------   0 matt      (1000) users      (100)    23745 2023-12-30 00:19:21.000000 pygenda-0.3.3/docs/screenshots/year_view.png
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.205362 pygenda-0.3.3/pygenda/
+-rwx------   0 matt      (1000) users      (100)      823 2024-01-04 12:29:50.000000 pygenda-0.3.3/pygenda/__main__.py
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.206362 pygenda-0.3.3/pygenda/app/
+-rw-------   0 matt      (1000) users      (100)      369 2023-12-30 00:19:21.000000 pygenda-0.3.3/pygenda/app/pygenda.desktop
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.209362 pygenda-0.3.3/pygenda/css/
+-rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/disc+loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/disc+loop.svg
+-rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/disc+star.svg
+-rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/disc.svg
+-rw-------   0 matt      (1000) users      (100)     3915 2024-05-26 08:16:44.000000 pygenda-0.3.3/pygenda/css/gemini.css
+-rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/loop.svg
+-rw-------   0 matt      (1000) users      (100)    16437 2024-05-26 08:16:44.000000 pygenda-0.3.3/pygenda/css/pygenda.css
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.3.3/pygenda/css/star.svg
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.209362 pygenda-0.3.3/pygenda/locale/
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.185362 pygenda-0.3.3/pygenda/locale/en_US/
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.210362 pygenda-0.3.3/pygenda/locale/en_US/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)      536 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)     1379 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/locale/en_US/LC_MESSAGES/pygenda.po
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.185362 pygenda-0.3.3/pygenda/locale/fr/
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.211362 pygenda-0.3.3/pygenda/locale/fr/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)    10493 2024-05-25 17:12:29.000000 pygenda-0.3.3/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)    16931 2024-05-26 08:21:55.000000 pygenda-0.3.3/pygenda/locale/fr/LC_MESSAGES/pygenda.po
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.186362 pygenda-0.3.3/pygenda/locale/nl/
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.211362 pygenda-0.3.3/pygenda/locale/nl/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)    10366 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/locale/nl/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)    16867 2024-05-26 08:21:55.000000 pygenda-0.3.3/pygenda/locale/nl/LC_MESSAGES/pygenda.po
+-rw-------   0 matt      (1000) users      (100)    14754 2024-05-26 08:21:55.000000 pygenda-0.3.3/pygenda/locale/pygenda.pot
+-rw-------   0 matt      (1000) users      (100)     1105 2024-05-25 07:25:21.000000 pygenda-0.3.3/pygenda/mypy.ini
+-rw-------   0 matt      (1000) users      (100)    83718 2024-05-25 07:11:31.000000 pygenda-0.3.3/pygenda/pygenda_calendar.py
+-rw-------   0 matt      (1000) users      (100)     5805 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_config.py
+-rw-------   0 matt      (1000) users      (100)    11782 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_dialog_entryprops.py
+-rw-------   0 matt      (1000) users      (100)    75600 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_dialog_event.py
+-rw-------   0 matt      (1000) users      (100)     3447 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_dialog_find.py
+-rw-------   0 matt      (1000) users      (100)     9450 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_dialog_import.py
+-rw-------   0 matt      (1000) users      (100)    15266 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_dialog_todo.py
+-rw-------   0 matt      (1000) users      (100)     4656 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_entryinfo.py
+-rw-------   0 matt      (1000) users      (100)    46586 2024-05-26 08:16:44.000000 pygenda-0.3.3/pygenda/pygenda_gui.py
+-rw-------   0 matt      (1000) users      (100)    11647 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_util.py
+-rw-------   0 matt      (1000) users      (100)      300 2024-05-26 08:23:51.000000 pygenda-0.3.3/pygenda/pygenda_version.py
+-rw-------   0 matt      (1000) users      (100)    16272 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_view.py
+-rw-------   0 matt      (1000) users      (100)    27322 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_view_todo.py
+-rw-------   0 matt      (1000) users      (100)    22946 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_view_week.py
+-rw-------   0 matt      (1000) users      (100)    29080 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_view_year.py
+-rw-------   0 matt      (1000) users      (100)    22109 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/pygenda_widgets.py
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.213362 pygenda-0.3.3/pygenda/ui/
+-rw-------   0 matt      (1000) users      (100)    45184 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/dialog_event.ui
+-rw-------   0 matt      (1000) users      (100)     5147 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/dialog_find.ui
+-rw-------   0 matt      (1000) users      (100)    14665 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/dialog_todo.ui
+-rw-------   0 matt      (1000) users      (100)    33513 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/main.ui
+-rw-------   0 matt      (1000) users      (100)     3889 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/view_week.ui
+-rw-------   0 matt      (1000) users      (100)     5928 2024-05-19 07:51:55.000000 pygenda-0.3.3/pygenda/ui/view_year.ui
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.218362 pygenda-0.3.3/pygenda.egg-info/
+-rw-r--r--   0 matt      (1000) users      (100)     1230 2024-05-26 08:27:50.000000 pygenda-0.3.3/pygenda.egg-info/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     2164 2024-05-26 08:27:50.000000 pygenda-0.3.3/pygenda.egg-info/SOURCES.txt
+-rw-------   0 matt      (1000) users      (100)        1 2024-05-26 08:27:50.000000 pygenda-0.3.3/pygenda.egg-info/dependency_links.txt
+-rw-------   0 matt      (1000) users      (100)       59 2024-05-26 08:27:50.000000 pygenda-0.3.3/pygenda.egg-info/requires.txt
+-rw-------   0 matt      (1000) users      (100)        8 2024-05-26 08:27:50.000000 pygenda-0.3.3/pygenda.egg-info/top_level.txt
+-rw-------   0 matt      (1000) users      (100)     1177 2024-05-26 08:24:19.000000 pygenda-0.3.3/pyproject.toml
+-rw-------   0 matt      (1000) users      (100)       38 2024-05-26 08:27:50.218362 pygenda-0.3.3/setup.cfg
+-rwx------   0 matt      (1000) users      (100)     3950 2024-05-26 08:16:44.000000 pygenda-0.3.3/setup_old.py
+drwx------   0 matt      (1000) users      (100)        0 2024-05-26 08:27:50.216362 pygenda-0.3.3/test/
+-rwx------   0 matt      (1000) users      (100)    15171 2023-12-30 00:19:21.000000 pygenda-0.3.3/test/maketest_example.py
+-rwx------   0 matt      (1000) users      (100)     1274 2023-03-31 11:03:09.000000 pygenda-0.3.3/test/maketest_large.py
+-rw-------   0 matt      (1000) users      (100)       83 2022-01-30 22:37:16.000000 pygenda-0.3.3/test/test00_empty.ics
+-rw-------   0 matt      (1000) users      (100)     1731 2024-05-19 07:51:55.000000 pygenda-0.3.3/test/test01_small.ics
+-rw-------   0 matt      (1000) users      (100)    13193 2023-12-30 00:19:21.000000 pygenda-0.3.3/test/test02_repeats.ics
+-rw-------   0 matt      (1000) users      (100)     2944 2023-12-30 00:19:21.000000 pygenda-0.3.3/test/test03_errors.ics
+-rw-------   0 matt      (1000) users      (100)    15407 2024-05-19 07:51:55.000000 pygenda-0.3.3/test/test04_dst.ics
+-rwx------   0 matt      (1000) users      (100)    19964 2024-05-19 07:51:55.000000 pygenda-0.3.3/test/test_entries.py
+-rwx------   0 matt      (1000) users      (100)    53498 2024-05-19 07:51:55.000000 pygenda-0.3.3/test/test_import_paste.py
+-rwx------   0 matt      (1000) users      (100)    25466 2024-05-19 07:51:55.000000 pygenda-0.3.3/test/test_ongoing.py
+-rwx------   0 matt      (1000) users      (100)   124411 2024-05-25 07:11:34.000000 pygenda-0.3.3/test/test_repeats.py
```

### Comparing `pygenda-0.3.2/COPYING` & `pygenda-0.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/PKG-INFO` & `pygenda-0.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.3.2
+Version: 0.3.3
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
-Home-page: https://github.com/semiprime/pygenda
-Author: Matthew Lewis
-Author-email: pygenda@semiprime.com
-License: GPLv3 only
-Platform: UNKNOWN
+Author-email: Matthew Lewis <pygenda@semiprime.com>
+Project-URL: Homepage, https://github.com/semiprime/pygenda
+Keywords: calendar,agenda,todolist,diary,pda,psion,geminipda,linux-mobile
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.5
+Description-Content-Type: text/markdown
 License-File: COPYING
+Requires-Dist: PyGObject
+Requires-Dist: python-dateutil
+Requires-Dist: icalendar
+Requires-Dist: tzlocal!=2.*
+Requires-Dist: num2words
 
 Pygenda is a calendar/agenda application written in Python3/GTK3. The UI is inspired by the Agenda programs on the Psion Series 3 and Series 5 range of keyboard PDAs, with the aim of being suitable for devices such as Planet Computers' Gemini (running Linux).
 
 For more information/latest source, see https://github.com/semiprime/pygenda
-
```

### Comparing `pygenda-0.3.2/README.md` & `pygenda-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,21 @@
 directly from the root directory of the project (containing this
 readme), with the command:
 
 	python3 -m pygenda
 
 Better/recommended: install the Python module with (for example)...
 
-	./setup.py develop --user
+	pip3 install --editable . --user
 
-(You can uninstall the module with `pip3 uninstall pygenda`.)
+Or, for older versions of pip/Python:
+
+    ./setup_old.py develop --user
+
+(In either case you can uninstall the module with `pip3 uninstall pygenda`.)
 
 Now you can now run Pygenda from anywhere with:
 
 	python3 -m pygenda
 
 There are a few command-line options, which you can view using:
```

### Comparing `pygenda-0.3.2/csrc/CMakeLists.txt` & `pygenda-0.3.3/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/csrc/pygenda_clipboard.c` & `pygenda-0.3.3/csrc/pygenda_clipboard.c`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/__main__.py` & `pygenda-0.3.3/pygenda/__main__.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/css/gemini.css` & `pygenda-0.3.3/pygenda/css/gemini.css`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,18 @@
 	padding:2px;
 }
 
 #yearview_labeldate {
 	padding:2px;
 }
 
+.yearview_daycell {
+	font-size:9pt;
+}
+
 .zoom0 #yearview_datecontent, .zoom0 #yearview_labeldate {
 	font-size:14pt;
 }
 
 .zoom1 #yearview_datecontent, .zoom1 #yearview_labeldate {
 	font-size:15.5pt;
 }
```

### Comparing `pygenda-0.3.2/pygenda/css/pygenda.css` & `pygenda-0.3.3/pygenda/css/pygenda.css`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 	background-color:rgba(210,210,210,0.4);
 	border-right:solid #ddd 1px;
 	border-bottom:solid #ddd 1px;
 }
 
 .yearview_daycell {
 	font-family:'DejaVu Sans Condensed';
-	font-size:8pt;
+	font-size:7pt;
 	background-color:rgba(255,255,255,0.7);
 	border-right:solid black 1px;
 	border-bottom:solid black 1px;
 	padding:1px;
 }
 
 .yearview_leftofdaycell {
```

### Comparing `pygenda-0.3.2/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo` & `pygenda-0.3.3/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/locale/fr/LC_MESSAGES/pygenda.mo` & `pygenda-0.3.3/pygenda/locale/fr/LC_MESSAGES/pygenda.mo`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/locale/nl/LC_MESSAGES/pygenda.mo` & `pygenda-0.3.3/pygenda/locale/nl/LC_MESSAGES/pygenda.mo`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/locale/pygenda.pot` & `pygenda-0.3.3/pygenda/locale/pygenda.pot`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 #
 
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-07 23:00+0200\n"
+"POT-Creation-Date: 2024-05-25 19:07+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -392,51 +392,51 @@
 msgid "New To-do"
 msgstr ""
 
 #: pygenda_dialog_todo.py:168
 msgid "Edit To-do"
 msgstr ""
 
-#: pygenda_gui.py:951
+#: pygenda_gui.py:962
 msgid "Delete Entry"
 msgstr ""
 
-#: pygenda_gui.py:957
+#: pygenda_gui.py:968
 msgid "Delete all repeats:\n“{:s}”?"
 msgstr ""
 
-#: pygenda_gui.py:959
+#: pygenda_gui.py:970
 msgid "Delete entry:\n“{:s}”?"
 msgstr ""
 
-#: pygenda_gui.py:987 ui/main.ui:656
+#: pygenda_gui.py:998 ui/main.ui:656
 msgid "Go To"
 msgstr ""
 
-#: pygenda_gui.py:999
+#: pygenda_gui.py:1010
 msgid "Go"
 msgstr ""
 
-#: pygenda_gui.py:1037
+#: pygenda_gui.py:1048
 msgid "Source code & documentation: "
 msgstr ""
 
-#: pygenda_gui.py:1042
+#: pygenda_gui.py:1053
 msgid ""
 "A calendar/agenda application written in Python/GTK3. The UI is inspired by "
 "the Agenda apps on the Psion Series 3 and Series 5 PDAs.\n"
 "WARNING: This is in-development code, released for testing and feedback. "
 "There will be bugs; please report them to: pygenda@semiprime.com."
 msgstr ""
 
-#: pygenda_gui.py:1043
+#: pygenda_gui.py:1054
 msgid "Thanks for testing &amp; feedback"
 msgstr ""
 
-#: pygenda_gui.py:1044
+#: pygenda_gui.py:1055
 # This information is be shown in the credits pane of the "About" dialog.
 # Translators are encouraged to add their own name here, and may add a
 # website/email too. Pseudonyms and anonymity are also welcome.
 msgid "translator-credits"
 msgstr ""
 
 #: pygenda_view_todo.py:42
```

### Comparing `pygenda-0.3.2/pygenda/pygenda_calendar.py` & `pygenda-0.3.3/pygenda/pygenda_calendar.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_config.py` & `pygenda-0.3.3/pygenda/pygenda_config.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_dialog_entryprops.py` & `pygenda-0.3.3/pygenda/pygenda_dialog_entryprops.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_dialog_event.py` & `pygenda-0.3.3/pygenda/pygenda_dialog_event.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_dialog_find.py` & `pygenda-0.3.3/pygenda/pygenda_dialog_find.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_dialog_import.py` & `pygenda-0.3.3/pygenda/pygenda_dialog_import.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_dialog_todo.py` & `pygenda-0.3.3/pygenda/pygenda_dialog_todo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_entryinfo.py` & `pygenda-0.3.3/pygenda/pygenda_entryinfo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_gui.py` & `pygenda-0.3.3/pygenda/pygenda_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,15 +435,15 @@
     @classmethod
     def _init_clipboard(cls) -> None:
         # Load clipboard helper library if available, or set to None
         try:
             libclip_file = '{:s}/libpygenda_clipboard.so'.format(ospath.dirname(__file__))
             cls._lib_clip = ctypes.CDLL(libclip_file)
         except:
-            print('Warning: Failed to load clipboard library', file=stderr)
+            print('Notice: Clipboard library not found, using fallback', file=stderr)
 
 
     @classmethod
     def _init_date_format(cls) -> None:
         # Initialise date formatting strings from config
         cls.date_order = cls._date_order_from_config()
 
@@ -873,51 +873,49 @@
 
 
     @classmethod
     def cut_request(cls, *args) -> bool:
         # Handler to implement "cut" from GUI, e.g. cut clicked in menu
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en and 'SUMMARY' in en:
-            if cls._lib_clip is None:
-                # Don't do fallback - might lead to unexpected data loss
-                print('Warning: No clipboard library, cut not available', file=stderr)
-            elif 'RRULE' in en: # repeating entry
+            if 'RRULE' in en: # repeating entry
                 # Need to think about how to implement this from UI side.
                 # Problem: Does user expect single occurrence to be cut, or all?
                 # Maybe bring up dialog "Cut single occurrence, or all repeats?"
                 # Then, do we do the came for Copying repeating entries?
                 # How do we adapt repeats when moved to a different date?
                 print('Warning: Cutting repeating entries not implemented', file=stderr)
-            else:
-                txtbuf = bytes(en['SUMMARY'], 'utf-8')
-                calbuf = en.to_ical()
-                cls._lib_clip.set_cb(ctypes.create_string_buffer(txtbuf),ctypes.create_string_buffer(calbuf))
-                Calendar.delete_entry(en)
-                cls.view_redraw(en_changes=True)
+                return True
+            cls._put_entry_on_clipboard(en)
+            Calendar.delete_entry(en)
+            cls.view_redraw(en_changes=True)
         return True # don't propagate event
 
 
     @classmethod
     def copy_request(cls, *args) -> bool:
         # Handler to implement "copy" from GUI, e.g. copy clicked in menu
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en and 'SUMMARY' in en:
-            if cls._lib_clip is None:
-                print('Warning: No clipboard library, fallback to text copy', file=stderr)
-                cb = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
-                txt = en['SUMMARY']
-                cb.set_text(txt, -1)
-            else:
-                txtbuf = bytes(en['SUMMARY'], 'utf-8')
-                calbuf = en.to_ical()
-                cls._lib_clip.set_cb(ctypes.create_string_buffer(txtbuf),ctypes.create_string_buffer(calbuf))
+            cls._put_entry_on_clipboard(en)
         return True # don't propagate event
 
 
     @classmethod
+    def _put_entry_on_clipboard(cls, en:Union[iEvent,iTodo]) -> None:
+        calbuf = en.to_ical()
+        if cls._lib_clip is None:
+            cb = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
+            cb.set_text(calbuf.decode('utf-8'), -1)
+        else:
+            txtbuf = bytes(en['SUMMARY'], 'utf-8')
+            cls._lib_clip.set_cb(ctypes.create_string_buffer(txtbuf),ctypes.create_string_buffer(calbuf))
+
+
+    @classmethod
     def paste_request(cls, *args) -> bool:
         # Handler to implement "paste" from GUI, e.g. paste clicked in menu
         cb = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
 
         # First, we try requesting a 'text/calendar' type from the clipboard
         sdat = cb.wait_for_contents(Gdk.Atom.intern('text/calendar', False))
         try:
@@ -925,14 +923,27 @@
             en = ical.walk()[0]
             cls.views[cls._view_idx].paste_entry(en)
             cls.view_redraw(en_changes=True)
         except:
             # Fallback: request plain text from clipboard
             txt = cb.wait_for_text()
             if txt: # might be None
+                if cls._lib_clip is None:
+                    # "Text" might be ical data, let's check...
+                    try:
+                        ical = iCalendar.from_ical(txt)
+                        en = ical.walk()[0]
+                        cls.views[cls._view_idx].paste_entry(en)
+                        cls.view_redraw(en_changes=True)
+                        return True
+                    except:
+                        pass
+                # We got text. Either clipboard library is present, or
+                # there was an exception trying to treat it as ical data.
+                # So, let's just treat it as plain text...
                 txt = cls._sanitise_pasted_text(txt)
                 # Type of entry created depends on View, so call View paste fn
                 if txt:
                     cls.views[cls._view_idx].paste_text(txt)
         return True # don't propagate event
```

### Comparing `pygenda-0.3.2/pygenda/pygenda_util.py` & `pygenda-0.3.3/pygenda/pygenda_util.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_view.py` & `pygenda-0.3.3/pygenda/pygenda_view.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_view_todo.py` & `pygenda-0.3.3/pygenda/pygenda_view_todo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_view_week.py` & `pygenda-0.3.3/pygenda/pygenda_view_week.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_view_year.py` & `pygenda-0.3.3/pygenda/pygenda_view_year.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/pygenda_widgets.py` & `pygenda-0.3.3/pygenda/pygenda_widgets.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/dialog_event.ui` & `pygenda-0.3.3/pygenda/ui/dialog_event.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/dialog_find.ui` & `pygenda-0.3.3/pygenda/ui/dialog_find.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/dialog_todo.ui` & `pygenda-0.3.3/pygenda/ui/dialog_todo.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/main.ui` & `pygenda-0.3.3/pygenda/ui/main.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/view_week.ui` & `pygenda-0.3.3/pygenda/ui/view_week.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda/ui/view_year.ui` & `pygenda-0.3.3/pygenda/ui/view_year.ui`

 * *Files identical despite different names*

### Comparing `pygenda-0.3.2/pygenda.egg-info/PKG-INFO` & `pygenda-0.3.3/pygenda.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.3.2
+Version: 0.3.3
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
-Home-page: https://github.com/semiprime/pygenda
-Author: Matthew Lewis
-Author-email: pygenda@semiprime.com
-License: GPLv3 only
-Platform: UNKNOWN
+Author-email: Matthew Lewis <pygenda@semiprime.com>
+Project-URL: Homepage, https://github.com/semiprime/pygenda
+Keywords: calendar,agenda,todolist,diary,pda,psion,geminipda,linux-mobile
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.5
+Description-Content-Type: text/markdown
 License-File: COPYING
+Requires-Dist: PyGObject
+Requires-Dist: python-dateutil
+Requires-Dist: icalendar
+Requires-Dist: tzlocal!=2.*
+Requires-Dist: num2words
 
 Pygenda is a calendar/agenda application written in Python3/GTK3. The UI is inspired by the Agenda programs on the Psion Series 3 and Series 5 range of keyboard PDAs, with the aim of being suitable for devices such as Planet Computers' Gemini (running Linux).
 
 For more information/latest source, see https://github.com/semiprime/pygenda
-
```

### Comparing `pygenda-0.3.2/setup.py` & `pygenda-0.3.3/setup_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# setup.py for Pygenda
+# setup_old.py for Pygenda
 #
 # Copyright (C) 2022,2023 Matthew Lewis
 #
 # This file is part of Pygenda.
 #
 # Pygenda is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -16,14 +16,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 #
 
+# This is an old setup script for those who need it.
+
 # Example usage:
 #   ./setup.py install [--user]
 #   ./setup.py develop [--user]
 #   ./setup.py sdist
 #   ./setup.py bdist_wheel --plat-name=[linux-x86_64|linux-aarch64]
```

