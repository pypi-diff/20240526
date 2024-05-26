# Comparing `tmp/moulti-1.8.1.tar.gz` & `tmp/moulti-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moulti-1.8.1.tar", last modified: Sun May 12 17:06:45 2024, max compression
+gzip compressed data, was "moulti-1.9.0.tar", last modified: Sun May 19 20:23:53 2024, max compression
```

## Comparing `moulti-1.8.1.tar` & `moulti-1.9.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.938383 moulti-1.8.1/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.8.1/LICENSE
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-12 17:06:45.938383 moulti-1.8.1/PKG-INFO
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3869 2024-05-05 16:06:31.000000 moulti-1.8.1/README.md
--rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.8.1/pyproject.toml
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-05-12 17:06:45.938383 moulti-1.8.1/setup.cfg
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1655 2024-05-12 17:04:03.000000 moulti-1.8.1/setup.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.930383 moulti-1.8.1/src/
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)       76 2024-05-12 17:04:03.000000 moulti-1.8.1/src/moulti/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.8.1/src/moulti/__main__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.8.1/src/moulti/ansi.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/ansible/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-28 14:10:17.000000 moulti-1.8.1/src/moulti/ansible/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7153 2024-05-01 20:47:59.000000 moulti-1.8.1/src/moulti/ansible/moulti.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    26354 2024-05-03 01:53:49.000000 moulti-1.8.1/src/moulti/app.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2841 2024-04-20 13:43:17.000000 moulti-1.8.1/src/moulti/askpass.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7490 2024-05-09 00:09:29.000000 moulti-1.8.1/src/moulti/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     3856 2024-05-04 21:51:51.000000 moulti-1.8.1/src/moulti/diff.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.8.1/src/moulti/helpers.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     1798 2024-05-02 17:34:34.000000 moulti-1.8.1/src/moulti/pipeline.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.8.1/src/moulti/precli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.8.1/src/moulti/protocol.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      177 2024-04-23 20:39:30.000000 moulti-1.8.1/src/moulti/widgets/__init__.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/abstractquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.8.1/src/moulti/widgets/abstractquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2024-04-23 18:32:39.000000 moulti-1.8.1/src/moulti/widgets/abstractquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2794 2024-04-23 17:32:01.000000 moulti-1.8.1/src/moulti/widgets/abstractquestion/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/abstractstep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.8.1/src/moulti/widgets/abstractstep/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      699 2024-04-23 18:32:38.000000 moulti-1.8.1/src/moulti/widgets/abstractstep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     4594 2024-04-23 21:17:23.000000 moulti-1.8.1/src/moulti/widgets/abstractstep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/buttonquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.8.1/src/moulti/widgets/buttonquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.8.1/src/moulti/widgets/buttonquestion/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.8.1/src/moulti/widgets/buttonquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.8.1/src/moulti/widgets/cli.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/collapsiblestep/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 17:16:59.000000 moulti-1.8.1/src/moulti/widgets/collapsiblestep/__init__.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 18:32:37.000000 moulti-1.8.1/src/moulti/widgets/collapsiblestep/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2805 2024-04-24 21:39:15.000000 moulti-1.8.1/src/moulti/widgets/collapsiblestep/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/divider/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 20:39:30.000000 moulti-1.8.1/src/moulti/widgets/divider/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1614 2024-04-23 20:39:30.000000 moulti-1.8.1/src/moulti/widgets/divider/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)      813 2024-04-24 21:40:25.000000 moulti-1.8.1/src/moulti/widgets/divider/tui.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.934383 moulti-1.8.1/src/moulti/widgets/inputquestion/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.8.1/src/moulti/widgets/inputquestion/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.8.1/src/moulti/widgets/inputquestion/cli.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-04-23 21:17:23.000000 moulti-1.8.1/src/moulti/widgets/inputquestion/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.8.1/src/moulti/widgets/moulticonsole.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.8.1/src/moulti/widgets/moultilog.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.8.1/src/moulti/widgets/quitdialog.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.938383 moulti-1.8.1/src/moulti/widgets/step/
--rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.8.1/src/moulti/widgets/step/__init__.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4550 2024-04-23 20:13:13.000000 moulti-1.8.1/src/moulti/widgets/step/cli.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     7353 2024-04-28 00:47:55.000000 moulti-1.8.1/src/moulti/widgets/step/tui.py
--rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.8.1/src/moulti/widgets/stepcontainer.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.8.1/src/moulti/widgets/tui.py
--rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.8.1/src/moulti/widgets/vertscroll.py
-drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-12 17:06:45.938383 moulti-1.8.1/src/moulti.egg-info/
--rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/PKG-INFO
--rw-r--r--   0 xavier    (1000) xavier    (1000)     1636 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/SOURCES.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/dependency_links.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       83 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/entry_points.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)       44 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/requires.txt
--rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-05-12 17:06:45.000000 moulti-1.8.1/src/moulti.egg-info/top_level.txt
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1066 2024-02-16 15:24:09.000000 moulti-1.9.0/LICENSE
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-19 20:23:53.834688 moulti-1.9.0/PKG-INFO
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3869 2024-05-18 21:22:35.000000 moulti-1.9.0/README.md
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.830687 moulti-1.9.0/examples/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7240 2024-05-19 18:37:57.000000 moulti-1.9.0/examples/moulti-functions.bash
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      627 2024-03-01 22:04:07.000000 moulti-1.9.0/pyproject.toml
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       38 2024-05-19 20:23:53.834688 moulti-1.9.0/setup.cfg
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1706 2024-05-19 20:22:47.000000 moulti-1.9.0/setup.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.830687 moulti-1.9.0/src/
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.830687 moulti-1.9.0/src/moulti/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)       76 2024-05-19 20:22:51.000000 moulti-1.9.0/src/moulti/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       29 2024-02-26 18:39:57.000000 moulti-1.9.0/src/moulti/__main__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     7781 2024-03-10 14:34:42.000000 moulti-1.9.0/src/moulti/ansi.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/ansible/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)        0 2024-04-28 14:10:17.000000 moulti-1.9.0/src/moulti/ansible/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7153 2024-05-01 20:47:59.000000 moulti-1.9.0/src/moulti/ansible/moulti.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    26354 2024-05-03 01:53:49.000000 moulti-1.9.0/src/moulti/app.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2841 2024-04-20 13:43:17.000000 moulti-1.9.0/src/moulti/askpass.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7490 2024-05-09 00:09:29.000000 moulti-1.9.0/src/moulti/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     3856 2024-05-04 21:51:51.000000 moulti-1.9.0/src/moulti/diff.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1213 2024-04-18 01:55:09.000000 moulti-1.9.0/src/moulti/helpers.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     1798 2024-05-02 17:34:34.000000 moulti-1.9.0/src/moulti/pipeline.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      820 2024-03-08 01:07:28.000000 moulti-1.9.0/src/moulti/precli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)    11647 2024-03-31 10:37:10.000000 moulti-1.9.0/src/moulti/protocol.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      177 2024-04-23 20:39:30.000000 moulti-1.9.0/src/moulti/widgets/__init__.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/abstractquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:32.000000 moulti-1.9.0/src/moulti/widgets/abstractquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      609 2024-04-23 18:32:39.000000 moulti-1.9.0/src/moulti/widgets/abstractquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2794 2024-04-23 17:32:01.000000 moulti-1.9.0/src/moulti/widgets/abstractquestion/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/abstractstep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-15 22:08:39.000000 moulti-1.9.0/src/moulti/widgets/abstractstep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      699 2024-04-23 18:32:38.000000 moulti-1.9.0/src/moulti/widgets/abstractstep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     4594 2024-04-23 21:17:23.000000 moulti-1.9.0/src/moulti/widgets/abstractstep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/buttonquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.9.0/src/moulti/widgets/buttonquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2347 2024-02-17 01:04:31.000000 moulti-1.9.0/src/moulti/widgets/buttonquestion/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     6868 2024-03-17 03:27:04.000000 moulti-1.9.0/src/moulti/widgets/buttonquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      408 2024-02-16 19:52:22.000000 moulti-1.9.0/src/moulti/widgets/cli.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/collapsiblestep/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 17:16:59.000000 moulti-1.9.0/src/moulti/widgets/collapsiblestep/__init__.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      749 2024-04-23 18:32:37.000000 moulti-1.9.0/src/moulti/widgets/collapsiblestep/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2805 2024-04-24 21:39:15.000000 moulti-1.9.0/src/moulti/widgets/collapsiblestep/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/divider/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-04-23 20:39:30.000000 moulti-1.9.0/src/moulti/widgets/divider/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1614 2024-04-23 20:39:30.000000 moulti-1.9.0/src/moulti/widgets/divider/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)      813 2024-04-24 21:40:25.000000 moulti-1.9.0/src/moulti/widgets/divider/tui.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/inputquestion/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:52.000000 moulti-1.9.0/src/moulti/widgets/inputquestion/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2897 2024-02-17 01:06:38.000000 moulti-1.9.0/src/moulti/widgets/inputquestion/cli.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2197 2024-04-23 21:17:23.000000 moulti-1.9.0/src/moulti/widgets/inputquestion/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4431 2024-03-10 13:06:07.000000 moulti-1.9.0/src/moulti/widgets/moulticonsole.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     3865 2024-03-09 04:48:36.000000 moulti-1.9.0/src/moulti/widgets/moultilog.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     2288 2024-02-21 01:21:22.000000 moulti-1.9.0/src/moulti/widgets/quitdialog.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti/widgets/step/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        0 2024-02-16 17:31:46.000000 moulti-1.9.0/src/moulti/widgets/step/__init__.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4550 2024-04-23 20:13:13.000000 moulti-1.9.0/src/moulti/widgets/step/cli.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     7353 2024-04-28 00:47:55.000000 moulti-1.9.0/src/moulti/widgets/step/tui.py
+-rw-rw-r--   0 xavier    (1000) xavier    (1000)     2854 2024-04-18 01:55:09.000000 moulti-1.9.0/src/moulti/widgets/stepcontainer.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1786 2024-02-21 22:35:11.000000 moulti-1.9.0/src/moulti/widgets/tui.py
+-rw-r--r--   0 xavier    (1000) xavier    (1000)      356 2024-04-10 22:30:03.000000 moulti-1.9.0/src/moulti/widgets/vertscroll.py
+drwxrwxr-x   0 xavier    (1000) xavier    (1000)        0 2024-05-19 20:23:53.834688 moulti-1.9.0/src/moulti.egg-info/
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     4894 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/PKG-INFO
+-rw-r--r--   0 xavier    (1000) xavier    (1000)     1667 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/SOURCES.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        1 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/dependency_links.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       83 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/entry_points.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)       44 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/requires.txt
+-rw-r--r--   0 xavier    (1000) xavier    (1000)        7 2024-05-19 20:23:53.000000 moulti-1.9.0/src/moulti.egg-info/top_level.txt
```

### Comparing `moulti-1.8.1/LICENSE` & `moulti-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/PKG-INFO` & `moulti-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.8.1
+Version: 1.9.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible,ansible,diff
 Classifier: Environment :: Console :: Curses
@@ -32,22 +32,22 @@
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
 Not convinced yet? What if the output of your Ansible playbooks looked like this?
 
-![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.svg?20240518)
 
 Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 By the way, Moulti can also display unified diff files:
 
-![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.svg?20240518)
 
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
```

### Comparing `moulti-1.8.1/README.md` & `moulti-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
 Not convinced yet? What if the output of your Ansible playbooks looked like this?
 
-![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.svg?20240518)
 
 Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 By the way, Moulti can also display unified diff files:
 
-![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.svg?20240518)
 
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
```

### Comparing `moulti-1.8.1/pyproject.toml` & `moulti-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/setup.py` & `moulti-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 short_description += 'lines emitted by your scripts to visual, collapsible blocks called steps.'
 
 with open('README.md', 'r') as readme:
 	long_description = readme.read()
 
 setup(
 	name='moulti',
-	version='1.8.1',
+	version='1.9.0',
 	description=short_description,
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Xavier G.',
 	author_email='xavier.moulti@kindwolf.org',
 	url='https://github.com/xavierog/moulti',
 	packages=[
@@ -46,8 +46,11 @@
 	install_requires=['textual>=0.53', 'pyperclip', 'argcomplete', 'unidiff'],
 	entry_points={
 		'console_scripts': [
 			'moulti = moulti.precli:main',
 			'moulti-askpass = moulti.askpass:main',
 		]
 	},
+	scripts=[
+		'examples/moulti-functions.bash',
+	],
 )
```

### Comparing `moulti-1.8.1/src/moulti/ansi.py` & `moulti-1.9.0/src/moulti/ansi.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/ansible/moulti.py` & `moulti-1.9.0/src/moulti/ansible/moulti.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/app.py` & `moulti-1.9.0/src/moulti/app.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/askpass.py` & `moulti-1.9.0/src/moulti/askpass.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/cli.py` & `moulti-1.9.0/src/moulti/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/diff.py` & `moulti-1.9.0/src/moulti/diff.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/helpers.py` & `moulti-1.9.0/src/moulti/helpers.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/pipeline.py` & `moulti-1.9.0/src/moulti/pipeline.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/precli.py` & `moulti-1.9.0/src/moulti/precli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/protocol.py` & `moulti-1.9.0/src/moulti/protocol.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/abstractquestion/cli.py` & `moulti-1.9.0/src/moulti/widgets/abstractquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/abstractquestion/tui.py` & `moulti-1.9.0/src/moulti/widgets/abstractquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/abstractstep/cli.py` & `moulti-1.9.0/src/moulti/widgets/abstractstep/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/abstractstep/tui.py` & `moulti-1.9.0/src/moulti/widgets/abstractstep/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/buttonquestion/cli.py` & `moulti-1.9.0/src/moulti/widgets/buttonquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/buttonquestion/tui.py` & `moulti-1.9.0/src/moulti/widgets/buttonquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/collapsiblestep/cli.py` & `moulti-1.9.0/src/moulti/widgets/collapsiblestep/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/collapsiblestep/tui.py` & `moulti-1.9.0/src/moulti/widgets/collapsiblestep/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/divider/cli.py` & `moulti-1.9.0/src/moulti/widgets/divider/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/divider/tui.py` & `moulti-1.9.0/src/moulti/widgets/divider/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/inputquestion/cli.py` & `moulti-1.9.0/src/moulti/widgets/inputquestion/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/inputquestion/tui.py` & `moulti-1.9.0/src/moulti/widgets/inputquestion/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/moulticonsole.py` & `moulti-1.9.0/src/moulti/widgets/moulticonsole.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/moultilog.py` & `moulti-1.9.0/src/moulti/widgets/moultilog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/quitdialog.py` & `moulti-1.9.0/src/moulti/widgets/quitdialog.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/step/cli.py` & `moulti-1.9.0/src/moulti/widgets/step/cli.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/step/tui.py` & `moulti-1.9.0/src/moulti/widgets/step/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/stepcontainer.py` & `moulti-1.9.0/src/moulti/widgets/stepcontainer.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti/widgets/tui.py` & `moulti-1.9.0/src/moulti/widgets/tui.py`

 * *Files identical despite different names*

### Comparing `moulti-1.8.1/src/moulti.egg-info/PKG-INFO` & `moulti-1.9.0/src/moulti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moulti
-Version: 1.8.1
+Version: 1.9.0
 Summary: Moulti is a CLI-driven Terminal User Interface (TUI) that enables you to assign the numerous lines emitted by your scripts to visual, collapsible blocks called steps.
 Home-page: https://github.com/xavierog/moulti
 Author: Xavier G.
 Author-email: xavier.moulti@kindwolf.org
 License: MIT
 Keywords: cli,tui,curses,terminal,multiplex,script,output,steps,textual,collapsible,ansible,diff
 Classifier: Environment :: Console :: Curses
@@ -32,22 +32,22 @@
 
 ![Moulti demo: Debian upgrade (Animated PNG)](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-demo-debian-upgrade.png?20240218)
 
 Interested? [Run this demo in a container using docker or podman](https://hub.docker.com/r/xavierong/moulti-demo)
 
 Not convinced yet? What if the output of your Ansible playbooks looked like this?
 
-![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.png?20240505)
+![Moulti: Ansible playbook output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-ansible.svg?20240518)
 
 Moulti is a tool meant for people who write and execute shell scripts and/or Ansible playbooks.
 Specifically, if you find yourself scrolling up your terminal to ensure everything went fine while your script is still running, then Moulti is made for you.
 
 By the way, Moulti can also display unified diff files:
 
-![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.png?20240505)
+![Moulti: unified diff output](https://xavier.kindwolf.org/p/moulti/doc/img/moulti-diff.svg?20240518)
 
 ## How?
 
 Synopsis:
 
 1. Start a Moulti instance: `moulti init`
 2. Add a step: `moulti step add step_name --title='some clever title here'`
```

### Comparing `moulti-1.8.1/src/moulti.egg-info/SOURCES.txt` & `moulti-1.9.0/src/moulti.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+examples/moulti-functions.bash
 src/moulti/__init__.py
 src/moulti/__main__.py
 src/moulti/ansi.py
 src/moulti/app.py
 src/moulti/askpass.py
 src/moulti/cli.py
 src/moulti/diff.py
```

