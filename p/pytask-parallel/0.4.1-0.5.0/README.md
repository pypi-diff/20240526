# Comparing `tmp/pytask_parallel-0.4.1.tar.gz` & `tmp/pytask_parallel-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask_parallel-0.4.1.tar", last modified: Fri Jan 12 15:30:24 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytask_parallel-0.4.1.tar` & `pytask_parallel-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.249300 pytask_parallel-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.245300 pytask_parallel-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.245300 pytask_parallel-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.245300 pytask_parallel-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-01-12 15:30:24.249300 pytask_parallel-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 15:30:24.249300 pytask_parallel-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.245300 pytask_parallel-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.249300 pytask_parallel-0.4.1/src/pytask_parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16742 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:16.000000 pytask_parallel-0.4.1/src/pytask_parallel/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:30:24.249300 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 15:30:23.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-12 15:30:24.000000 pytask_parallel-0.4.1/src/pytask_parallel.egg-info/top_level.txt
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/_version.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/backends.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/build.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/config.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/execute.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/logging.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/nodes.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/py.typed
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/typing.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/utils.py
+-rw-r--r--   0        0        0    10275 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/src/pytask_parallel/wrappers.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/README.md
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 pytask_parallel-0.5.0/PKG-INFO
```

### Comparing `pytask_parallel-0.4.1/LICENSE` & `pytask_parallel-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.4.1/src/pytask_parallel/build.py` & `pytask_parallel-0.5.0/src/pytask_parallel/build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Extend the build command."""
+
 from __future__ import annotations
 
 import click
 from pytask import EnumChoice
 from pytask import hookimpl
-from pytask_parallel.backends import PARALLEL_BACKENDS_DEFAULT
+
 from pytask_parallel.backends import ParallelBackend
 
 
 @hookimpl
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend the command line interface."""
     additional_parameters = [
@@ -21,11 +22,11 @@
             metavar="[INTEGER|auto]",
             default=1,
         ),
         click.Option(
             ["--parallel-backend"],
             type=EnumChoice(ParallelBackend),
             help="Backend for the parallelization.",
-            default=PARALLEL_BACKENDS_DEFAULT,
+            default=ParallelBackend.NONE,
         ),
     ]
     cli.commands["build"].params.extend(additional_parameters)
```

