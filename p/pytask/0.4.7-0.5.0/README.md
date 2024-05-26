# Comparing `tmp/pytask-0.4.7.tar.gz` & `tmp/pytask-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask-0.4.7.tar", last modified: Tue Mar 19 19:21:44 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytask-0.4.7.tar` & `pytask-0.5.0.tar`

### file list

```diff
@@ -1,95 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.936469 pytask-0.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.924469 pytask-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.924469 pytask-0.4.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.924469 pytask-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-19 19:21:40.000000 pytask-0.4.7/.github/workflows/update-plugin-list.yml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-19 19:21:40.000000 pytask-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-19 19:21:40.000000 pytask-0.4.7/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-19 19:21:40.000000 pytask-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-19 19:21:40.000000 pytask-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-03-19 19:21:44.936469 pytask-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-03-19 19:21:40.000000 pytask-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-19 19:21:40.000000 pytask-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:21:44.936469 pytask-0.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.920468 pytask-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.932469 pytask-0.4.7/src/_pytask/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 19:21:44.000000 pytask-0.4.7/src/_pytask/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    23994 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/capture_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/click.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/collect_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    21435 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/collect_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/dag_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/debugging.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/live.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.932469 pytask-0.4.7/src/_pytask/mark/
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/mark/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/mark/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/mark/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/mark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/node_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/outcomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/persist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/skipping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/task_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-03-19 19:21:40.000000 pytask-0.4.7/src/_pytask/warnings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.932469 pytask-0.4.7/src/pytask/
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-03-19 19:21:40.000000 pytask-0.4.7/src/pytask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-19 19:21:40.000000 pytask-0.4.7/src/pytask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-19 19:21:40.000000 pytask-0.4.7/src/pytask/path.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:40.000000 pytask-0.4.7/src/pytask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-19 19:21:40.000000 pytask-0.4.7/src/pytask/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:21:44.936469 pytask-0.4.7/src/pytask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-19 19:21:44.000000 pytask-0.4.7/src/pytask.egg-info/top_level.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/__init__.py
+-rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/_hashlib.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/_inspect.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/_version.py
+-rw-r--r--   0        0        0    11286 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/build.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/cache.py
+-rw-r--r--   0        0        0    24944 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/capture.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/capture_utils.py
+-rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/clean.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/cli.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/click.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/coiled_utils.py
+-rw-r--r--   0        0        0    21120 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/collect.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/collect_command.py
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/collect_utils.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/compat.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/config.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/config_utils.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/console.py
+-rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/dag.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/dag_command.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/dag_utils.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/data_catalog.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/database.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/database_utils.py
+-rw-r--r--   0        0        0    14129 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/debugging.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/exceptions.py
+-rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/execute.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/git.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/hookspecs.py
+-rw-r--r--   0        0        0    11247 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/live.py
+-rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/logging.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/logging_utils.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/mark_utils.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/models.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/node_protocols.py
+-rw-r--r--   0        0        0    12160 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/nodes.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/outcomes.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/parameters.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/path.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/persist.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/pluginmanager.py
+-rw-r--r--   0        0        0    10056 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/profile.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/provisional.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/provisional_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/py.typed
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/reports.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/session.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/shared.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/skipping.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/task.py
+-rw-r--r--   0        0        0    13443 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/task_utils.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/traceback.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/tree_util.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/typing.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/warnings.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/warnings_utils.py
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/mark/__init__.py
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/mark/expression.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 pytask-0.5.0/src/_pytask/mark/structures.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pytask-0.5.0/src/pytask/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pytask-0.5.0/src/pytask/__main__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pytask-0.5.0/src/pytask/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytask-0.5.0/src/pytask/py.typed
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pytask-0.5.0/src/pytask/tree_util.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pytask-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pytask-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 pytask-0.5.0/README.md
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 pytask-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 pytask-0.5.0/PKG-INFO
```

### Comparing `pytask-0.4.7/LICENSE` & `pytask-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask-0.4.7/PKG-INFO` & `pytask-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytask
-Version: 0.4.7
-Summary: In its highest aspirations, pytask tries to be pytest as a build system.
-Author-email: Tobias Raabe <raabe@posteo.de>
-License: MIT
+Version: 0.5.0
+Summary: pytask is a workflow management system that facilitates reproducible data analyses.
 Project-URL: Changelog, https://pytask-dev.readthedocs.io/en/stable/changes.html
 Project-URL: Documentation, https://pytask-dev.readthedocs.io/en/stable
 Project-URL: Github, https://github.com/pytask-dev/pytask
 Project-URL: Homepage, https://pytask-dev.readthedocs.io/en/stable
 Project-URL: Tracker, https://github.com/pytask-dev/pytask/issues
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: win32
+Author-email: Tobias Raabe <raabe@posteo.de>
+License: MIT
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -25,50 +22,56 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: attrs>=21.3
 Requires-Dist: click
 Requires-Dist: click-default-group
 Requires-Dist: networkx>=2.4
 Requires-Dist: optree>=0.9
 Requires-Dist: packaging
-Requires-Dist: pluggy>=1
+Requires-Dist: pluggy>=1.3.0
 Requires-Dist: rich
 Requires-Dist: sqlalchemy>=2
-Requires-Dist: tomli>=1; python_version < "3.11"
-Requires-Dist: typing-extensions; python_version < "3.9"
-Provides-Extra: all
-Requires-Dist: universal-pathlib<0.2; python_version < "3.12" and extra == "all"
+Requires-Dist: tomli>=1; python_version < '3.11'
+Requires-Dist: typing-extensions; python_version < '3.9'
+Requires-Dist: universal-pathlib>=0.2.2
 Provides-Extra: docs
-Requires-Dist: furo; extra == "docs"
-Requires-Dist: ipython; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-click; extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
-Requires-Dist: sphinx-design>=0.3; extra == "docs"
-Requires-Dist: sphinx-toolbox; extra == "docs"
-Requires-Dist: sphinxext-opengraph; extra == "docs"
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: ipython; extra == 'docs'
+Requires-Dist: matplotlib; extra == 'docs'
+Requires-Dist: myst-nb; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Requires-Dist: sphinx-click; extra == 'docs'
+Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-design>=0.3; extra == 'docs'
+Requires-Dist: sphinx-toolbox; extra == 'docs'
+Requires-Dist: sphinxext-opengraph; extra == 'docs'
+Provides-Extra: plugin-list
+Requires-Dist: httpx; extra == 'plugin-list'
+Requires-Dist: tabulate[widechars]; extra == 'plugin-list'
+Requires-Dist: tqdm; extra == 'plugin-list'
 Provides-Extra: test
-Requires-Dist: deepdiff; extra == "test"
-Requires-Dist: nbmake; extra == "test"
-Requires-Dist: pexpect; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: pytest-xdist; extra == "test"
-Requires-Dist: syrupy; extra == "test"
-Requires-Dist: aiohttp; extra == "test"
-Requires-Dist: requests; extra == "test"
+Requires-Dist: aiohttp; extra == 'test'
+Requires-Dist: coiled; extra == 'test'
+Requires-Dist: deepdiff; extra == 'test'
+Requires-Dist: nbmake; extra == 'test'
+Requires-Dist: pexpect; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-xdist; extra == 'test'
+Requires-Dist: syrupy; extra == 'test'
+Provides-Extra: typing
+Requires-Dist: mypy>=1.9.0; extra == 'typing'
+Requires-Dist: nbqa[mypy]>=1.8.5; extra == 'typing'
+Description-Content-Type: text/markdown
 
 <a href="https://pytask-dev.readthedocs.io/en/stable">
     <p align="center">
         <img src="https://raw.githubusercontent.com/pytask-dev/pytask/main/docs/source/_static/images/pytask_w_text.png" width=50% alt="pytask">
     </p>
 </a>
```

#### html2text {}

```diff
@@ -1,44 +1,46 @@
-Metadata-Version: 2.1 Name: pytask Version: 0.4.7 Summary: In its highest
-aspirations, pytask tries to be pytest as a build system. Author-email: Tobias
-Raabe
-posteo.de> License: MIT Project-URL: Changelog, https://pytask-
-dev.readthedocs.io/en/stable/changes.html Project-URL: Documentation, https://
-pytask-dev.readthedocs.io/en/stable Project-URL: Github, https://github.com/
-pytask-dev/pytask Project-URL: Homepage, https://pytask-dev.readthedocs.io/en/
-stable Project-URL: Tracker, https://github.com/pytask-dev/pytask/issues
-Platform: unix Platform: linux Platform: osx Platform: win32 Classifier:
-Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
-Development :: Build Tools Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: attrs>=21.3 Requires-Dist:
-click Requires-Dist: click-default-group Requires-Dist: networkx>=2.4 Requires-
-Dist: optree>=0.9 Requires-Dist: packaging Requires-Dist: pluggy>=1 Requires-
+Metadata-Version: 2.3 Name: pytask Version: 0.5.0 Summary: pytask is a workflow
+management system that facilitates reproducible data analyses. Project-URL:
+Changelog, https://pytask-dev.readthedocs.io/en/stable/changes.html Project-
+URL: Documentation, https://pytask-dev.readthedocs.io/en/stable Project-URL:
+Github, https://github.com/pytask-dev/pytask Project-URL: Homepage, https://
+pytask-dev.readthedocs.io/en/stable Project-URL: Tracker, https://github.com/
+pytask-dev/pytask/issues Author-email: Tobias Raabe
+posteo.de> License: MIT License-File: LICENSE Classifier: Development Status ::
+4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: POSIX Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.8 Requires-Dist: attrs>=21.3 Requires-Dist: click
+Requires-Dist: click-default-group Requires-Dist: networkx>=2.4 Requires-Dist:
+optree>=0.9 Requires-Dist: packaging Requires-Dist: pluggy>=1.3.0 Requires-
 Dist: rich Requires-Dist: sqlalchemy>=2 Requires-Dist: tomli>=1; python_version
-< "3.11" Requires-Dist: typing-extensions; python_version < "3.9" Provides-
-Extra: all Requires-Dist: universal-pathlib<0.2; python_version < "3.12" and
-extra == "all" Provides-Extra: docs Requires-Dist: furo; extra == "docs"
-Requires-Dist: ipython; extra == "docs" Requires-Dist: myst-parser; extra ==
-"docs" Requires-Dist: nbsphinx; extra == "docs" Requires-Dist: sphinx; extra ==
-"docs" Requires-Dist: sphinx-click; extra == "docs" Requires-Dist: sphinx-
-copybutton; extra == "docs" Requires-Dist: sphinx-design>=0.3; extra == "docs"
-Requires-Dist: sphinx-toolbox; extra == "docs" Requires-Dist: sphinxext-
-opengraph; extra == "docs" Provides-Extra: test Requires-Dist: deepdiff; extra
-== "test" Requires-Dist: nbmake; extra == "test" Requires-Dist: pexpect; extra
-== "test" Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov;
-extra == "test" Requires-Dist: pytest-xdist; extra == "test" Requires-Dist:
-syrupy; extra == "test" Requires-Dist: aiohttp; extra == "test" Requires-Dist:
-requests; extra == "test"
+< '3.11' Requires-Dist: typing-extensions; python_version < '3.9' Requires-
+Dist: universal-pathlib>=0.2.2 Provides-Extra: docs Requires-Dist: furo; extra
+== 'docs' Requires-Dist: ipython; extra == 'docs' Requires-Dist: matplotlib;
+extra == 'docs' Requires-Dist: myst-nb; extra == 'docs' Requires-Dist: myst-
+parser; extra == 'docs' Requires-Dist: sphinx; extra == 'docs' Requires-Dist:
+sphinx-click; extra == 'docs' Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-design>=0.3; extra == 'docs' Requires-Dist: sphinx-
+toolbox; extra == 'docs' Requires-Dist: sphinxext-opengraph; extra == 'docs'
+Provides-Extra: plugin-list Requires-Dist: httpx; extra == 'plugin-list'
+Requires-Dist: tabulate[widechars]; extra == 'plugin-list' Requires-Dist: tqdm;
+extra == 'plugin-list' Provides-Extra: test Requires-Dist: aiohttp; extra ==
+'test' Requires-Dist: coiled; extra == 'test' Requires-Dist: deepdiff; extra ==
+'test' Requires-Dist: nbmake; extra == 'test' Requires-Dist: pexpect; extra ==
+'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-cov; extra
+== 'test' Requires-Dist: pytest-xdist; extra == 'test' Requires-Dist: syrupy;
+extra == 'test' Provides-Extra: typing Requires-Dist: mypy>=1.9.0; extra ==
+'typing' Requires-Dist: nbqa[mypy]>=1.8.5; extra == 'typing' Description-
+Content-Type: text/markdown
                                    _[_p_y_t_a_s_k_]
 ______________________________________________________________________ [![PyPI]
 (https://img.shields.io/pypi/v/pytask?color=blue)](https://pypi.org/project/
 pytask) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 pytask)](https://pypi.org/project/pytask) [![image](https://img.shields.io/
 conda/vn/conda-forge/pytask.svg)](https://anaconda.org/conda-forge/pytask) [!
 [image](https://img.shields.io/conda/pn/conda-forge/pytask.svg)](https://
```

### Comparing `pytask-0.4.7/README.md` & `pytask-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytask-0.4.7/pyproject.toml` & `pytask-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,169 @@
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = ["setuptools>=64", "setuptools_scm>=8"]
-
-[tool.setuptools_scm]
-version_file = "src/_pytask/_version.py"
-
 [project]
 name = "pytask"
-description = "In its highest aspirations, pytask tries to be pytest as a build system."
+description = "pytask is a workflow management system that facilitates reproducible data analyses."
 requires-python = ">=3.8"
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Environment :: Console",
-  "Intended Audience :: Science/Research",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: MacOS :: MacOS X",
-  "Operating System :: Microsoft :: Windows",
-  "Operating System :: POSIX",
-  "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Topic :: Scientific/Engineering",
-  "Topic :: Software Development :: Build Tools",
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Build Tools",
 ]
 dynamic = ["version"]
 dependencies = [
-  "attrs>=21.3",
-  "click",
-  "click-default-group",
-  "networkx>=2.4",
-  "optree>=0.9",
-  "packaging",
-  "pluggy>=1",
-  "rich",
-  "sqlalchemy>=2",
-  'tomli>=1; python_version < "3.11"',
-  'typing-extensions; python_version < "3.9"',
+    "attrs>=21.3",
+    "click",
+    "click-default-group",
+    "networkx>=2.4",
+    "optree>=0.9",
+    "packaging",
+    "pluggy>=1.3.0",
+    "rich",
+    "sqlalchemy>=2",
+    'tomli>=1; python_version < "3.11"',
+    'typing-extensions; python_version < "3.9"',
+    "universal-pathlib>=0.2.2",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.license]
 text = "MIT"
 
 [[project.authors]]
 name = "Tobias Raabe"
 email = "raabe@posteo.de"
 
 [project.optional-dependencies]
-all = ['universal-pathlib<0.2; python_version<"3.12"']
 docs = [
-  "furo",
-  "ipython",
-  "myst-parser",
-  "nbsphinx",
-  "sphinx",
-  "sphinx-click",
-  "sphinx-copybutton",
-  "sphinx-design>=0.3",
-  "sphinx-toolbox",
-  "sphinxext-opengraph",
+    "furo",
+    "ipython",
+    "matplotlib",
+    "myst-parser",
+    "myst-nb",
+    "sphinx",
+    "sphinx-click",
+    "sphinx-copybutton",
+    "sphinx-design>=0.3",
+    "sphinx-toolbox",
+    "sphinxext-opengraph",
 ]
+plugin-list = ["httpx", "tabulate[widechars]", "tqdm"]
 test = [
-  "deepdiff",
-  "nbmake",
-  "pexpect",
-  "pytest",
-  "pytest-cov",
-  "pytest-xdist",
-  "syrupy",
-  # For HTTPPath tests.
-  "aiohttp",
-  "requests",
+    "deepdiff",
+    "nbmake",
+    "pexpect",
+    "pytest",
+    "pytest-cov",
+    "pytest-xdist",
+    "syrupy",
+    "aiohttp",      # For HTTPPath tests.
+    "coiled",
 ]
+typing = ["mypy>=1.9.0", "nbqa[mypy]>=1.8.5"]
 
 [project.urls]
 Changelog = "https://pytask-dev.readthedocs.io/en/stable/changes.html"
 Documentation = "https://pytask-dev.readthedocs.io/en/stable"
 Github = "https://github.com/pytask-dev/pytask"
 Homepage = "https://pytask-dev.readthedocs.io/en/stable"
 Tracker = "https://github.com/pytask-dev/pytask/issues"
 
 [project.scripts]
 pytask = "pytask:cli"
 
-[tool.setuptools]
-include-package-data = true
-zip-safe = false
-platforms = ["unix", "linux", "osx", "win32"]
-license-files = ["LICENSE"]
-
-[tool.setuptools.package-dir]
-"" = "src"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-namespaces = false
+[build-system]
+requires = ["hatchling", "hatch_vcs"]
+build-backend = "hatchling.build"
+
+[tool.rye]
+managed = true
+dev-dependencies = ["tox-uv>=1.7.0"]
+
+[tool.rye.scripts]
+clean-docs = { cmd = "rm -rf docs/build" }
+build-docs = { cmd = "sphinx-build -b html docs/source docs/build" }
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/_pytask/_version.py"
+
+[tool.hatch.build.targets.sdist]
+exclude = ["tests"]
+only-packages = true
+
+[tool.hatch.build.targets.wheel]
+only-include = ["src"]
+sources = ["src"]
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.metadata]
+allow-direct-references = true
 
 [tool.ruff]
 target-version = "py38"
-select = ["ALL"]
 fix = true
+unsafe-fixes = true
+extend-include = ["*.ipynb"]
+
+[tool.ruff.lint]
+select = ["ALL"]
 ignore = [
-    "FBT",  # flake8-boolean-trap
-    "I",  # ignore isort
-    "TRY",  # ignore tryceratops.
-    # Others.
-    "ANN101",  # type annotating self
-    "ANN102",  # type annotating cls
-    "ANN401",  # flake8-annotate typing.Any
-    "COM812",  # Comply with ruff-format.
-    "ISC001",  # Comply with ruff-format.
+    "ANN101",
+    "ANN102",
+    "ANN401", # flake8-annotate typing.Any
+    "COM812", # Comply with ruff-format.
+    "ISC001", # Comply with ruff-format.
+    "FBT",
     "PD901",  # Avoid generic df for dataframes.
-    "S101",  # raise errors for asserts.
-    "S603",  # Call check with subprocess.run.
-    "S607",  # Call subprocess.run with partial executable path.
-    "SLF001",  # access private members.
+    "S101",   # raise errors for asserts.
+    "S603",   # Call check with subprocess.run.
+    "S607",   # Call subprocess.run with partial executable path.
+    "SLF001", # access private members.
 ]
 
-
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "src/_pytask/_hashlib.py" = ["ALL"]
 "src/_pytask/capture.py" = ["PGH003"]
 "src/_pytask/hookspecs.py" = ["ARG001"]
 "src/_pytask/outcomes.py" = ["N818"]
 "src/_pytask/dag.py" = ["B023"]
 "tests/test_capture.py" = ["T201", "PT011"]
 "tests/*" = ["ANN", "D", "FBT", "PLR2004", "S101"]
 "tests/test_jupyter/*" = ["INP001"]
 "scripts/*" = ["D", "INP001"]
 "docs/source/conf.py" = ["D401", "INP001"]
 "docs_src/*" = ["ARG001", "D", "INP001", "S301"]
 "docs_src/*/*.py" = ["FA100", "FA102", "PLR2004", "TCH"]
-"docs/source/how_to_guides/functional_interface*" = ["B018", "D", "INP", "ARG005"]
+"docs/source/how_to_guides/functional_interface*" = [
+    "B018",
+    "D",
+    "INP",
+    "ARG005",
+]
 "docs_src/how_to_guides/using_task_returns_*_task.py" = ["ARG005", "E731"]
-"docs_src/how_to_guides/writing_custom_nodes_*.py" = ["S301"]
 
+[tool.ruff.lint.isort]
+force-single-line = true
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.pytest.ini_options]
 testpaths = ["src", "tests"]
 markers = [
     "wip: Tests that are work-in-progress.",
     "unit: Flag for unit tests which target mainly a single function.",
@@ -164,37 +181,37 @@
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
-
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = ["click_default_group", "networkx"]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = ["_pytask.coiled_utils"]
+disable_error_code = ["import-not-found"]
+
+[[tool.mypy.overrides]]
 module = ["_pytask.hookspecs"]
 disable_error_code = ["empty-body"]
 
 [tool.codespell]
 skip = "*.js,*/termynal.css"
 
 [tool.refurb]
 python_version = "3.8"
 
-[tool.check-manifest]
-ignore = ["src/_pytask/_version.py"]
-
 [tool.coverage.report]
 exclude_also = [
     "pragma: no cover",
     "if TYPE_CHECKING.*:",
     "\\.\\.\\.",
     "def __repr__",
 ]
```

### Comparing `pytask-0.4.7/src/_pytask/_hashlib.py` & `pytask-0.5.0/src/_pytask/_hashlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,9 +228,9 @@
     if isinstance(value, (tuple, list)):
         value = "".join(str(hash_value(i)) for i in value)
     if isinstance(value, Path):
         value = str(value)
     if isinstance(value, str):
         value = value.encode()
     if isinstance(value, bytes):
-        return str(hashlib.sha256(value).hexdigest())
+        return hashlib.sha256(value).hexdigest()
     return hash(value)
```

### Comparing `pytask-0.4.7/src/_pytask/_inspect.py` & `pytask-0.5.0/src/_pytask/_inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import functools
 import sys
 import types
 from typing import Any
 from typing import Callable
 from typing import Mapping
 
-
 __all__ = ["get_annotations"]
 
 
 if sys.version_info >= (3, 10):  # pragma: no cover
     from inspect import get_annotations
 else:  # pragma: no cover
 
@@ -103,15 +102,15 @@
             raise TypeError(msg)
 
         if ann is None:
             return {}
 
         if not isinstance(ann, dict):
             msg = f"{obj!r}.__annotations__ is neither a dict nor None"
-            raise ValueError(msg)
+            raise ValueError(msg)  # noqa: TRY004
 
         if not ann:
             return {}
 
         if not eval_str:
             return dict(ann)
```

### Comparing `pytask-0.4.7/src/_pytask/build.py` & `pytask-0.5.0/src/_pytask/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """Implement the build command."""
+
 from __future__ import annotations
 
 import json
 import sys
 from contextlib import suppress
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Literal
-from typing import TYPE_CHECKING
 
 import click
+
 from _pytask.capture_utils import CaptureMethod
 from _pytask.capture_utils import ShowCapture
 from _pytask.click import ColoredCommand
 from _pytask.config_utils import find_project_root_and_config
 from _pytask.config_utils import read_config
 from _pytask.console import console
+from _pytask.dag import create_dag
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.exceptions import ExecutionError
 from _pytask.exceptions import ResolvingDependenciesError
 from _pytask.outcomes import ExitCode
 from _pytask.path import HashPathCache
 from _pytask.pluginmanager import get_plugin_manager
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.shared import parse_paths
 from _pytask.shared import to_list
-from _pytask.traceback import remove_internal_traceback_frames_from_exc_info
-from rich.traceback import Traceback
-
+from _pytask.traceback import Traceback
 
 if TYPE_CHECKING:
-    from _pytask.node_protocols import PTask
     from typing import NoReturn
 
+    from _pytask.node_protocols import PTask
+
 
 @hookimpl(tryfirst=True)
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend the command line interface."""
     cli.add_command(build_command)
 
 
@@ -59,15 +61,15 @@
 @hookimpl
 def pytask_unconfigure(session: Session) -> None:
     """Save calculated file hashes to file."""
     path = session.config["root"] / ".pytask" / "file_hashes.json"
     path.write_text(json.dumps(HashPathCache._cache))
 
 
-def build(  # noqa: C901, PLR0912, PLR0913, PLR0915
+def build(  # noqa: C901, PLR0912, PLR0913
     *,
     capture: Literal["fd", "no", "sys", "tee-sys"] | CaptureMethod = CaptureMethod.FD,
     check_casing_of_paths: bool = True,
     config: Path | None = None,
     database_url: str = "",
     debug_pytask: bool = False,
     disable_warnings: bool = False,
@@ -76,28 +78,28 @@
     | str = "file",
     expression: str = "",
     force: bool = False,
     ignore: Iterable[str] = (),
     marker_expression: str = "",
     max_failures: float = float("inf"),
     n_entries_in_table: int = 15,
-    paths: str | Path | Iterable[str | Path] = (),
+    paths: Path | Iterable[Path] = (),
     pdb: bool = False,
     pdb_cls: str = "",
     s: bool = False,
     show_capture: Literal["no", "stdout", "stderr", "all"]
     | ShowCapture = ShowCapture.ALL,
     show_errors_immediately: bool = False,
     show_locals: bool = False,
     show_traceback: bool = True,
     sort_table: bool = True,
     stop_after_first_failure: bool = False,
     strict_markers: bool = False,
     tasks: Callable[..., Any] | PTask | Iterable[Callable[..., Any] | PTask] = (),
-    task_files: str | Iterable[str] = "task_*.py",
+    task_files: Iterable[str] = ("task_*.py",),
     trace: bool = False,
     verbose: int = 1,
     **kwargs: Any,
 ) -> Session:
     """Run pytask.
 
     This is the main command to run pytask which usually receives kwargs from the
@@ -221,21 +223,20 @@
         if "command" not in raw_config:
             raw_config["command"] = "build"
             # Add defaults from cli.
             from _pytask.cli import DEFAULTS_FROM_CLI
 
             raw_config = {**DEFAULTS_FROM_CLI, **raw_config}
 
-            raw_config["paths"] = parse_paths(raw_config.get("paths"))
+            raw_config["paths"] = parse_paths(raw_config["paths"])
 
             if raw_config["config"] is not None:
                 raw_config["config"] = Path(raw_config["config"]).resolve()
                 raw_config["root"] = raw_config["config"].parent
             else:
-                raw_config["paths"] = parse_paths(raw_config["paths"])
                 (
                     raw_config["root"],
                     raw_config["config"],
                 ) = find_project_root_and_config(raw_config["paths"])
 
             if raw_config["config"] is not None:
                 config_from_file = read_config(raw_config["config"])
@@ -251,39 +252,35 @@
                 raw_config = {**raw_config, **config_from_file}
 
         config_ = pm.hook.pytask_configure(pm=pm, raw_config=raw_config)
 
         session = Session.from_config(config_)
 
     except (ConfigurationError, Exception):
-        exc_info = remove_internal_traceback_frames_from_exc_info(sys.exc_info())
-        traceback = Traceback.from_exception(*exc_info)
-        console.print(traceback)
+        console.print(Traceback(sys.exc_info()))
         session = Session(exit_code=ExitCode.CONFIGURATION_FAILED)
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_dag(session=session)
+            session.dag = create_dag(session=session)
             session.hook.pytask_execute(session=session)
 
         except CollectionError:
             session.exit_code = ExitCode.COLLECTION_FAILED
 
         except ResolvingDependenciesError:
             session.exit_code = ExitCode.DAG_FAILED
 
         except ExecutionError:
             session.exit_code = ExitCode.FAILED
 
         except Exception:  # noqa: BLE001
-            exc_info = remove_internal_traceback_frames_from_exc_info(sys.exc_info())
-            traceback = Traceback.from_exception(*exc_info)
-            console.print(traceback)
+            console.print(Traceback(sys.exc_info()))
             session.exit_code = ExitCode.FAILED
 
         session.hook.pytask_unconfigure(session=session)
     return session
 
 
 @click.command(cls=ColoredCommand, name="build")
```

### Comparing `pytask-0.4.7/src/_pytask/cache.py` & `pytask-0.5.0/src/_pytask/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Contains a cache."""
+
 from __future__ import annotations
 
 import functools
 import hashlib
 import inspect
 from inspect import FullArgSpec
 from typing import Any
 from typing import Callable
 
-from _pytask._hashlib import hash_value
 from attrs import define
 from attrs import field
 
+from _pytask._hashlib import hash_value
+
 
 @define
 class CacheInfo:
     hits: int = 0
     misses: int = 0
```

### Comparing `pytask-0.4.7/src/_pytask/capture.py` & `pytask-0.5.0/src/_pytask/capture.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,40 +18,47 @@
   <https://eli.thegreenplace.net/2015/redirecting-all-kinds-of-stdout-in-python>`_.
 - `The capture module in pytest
   <https://github.com/pytest-dev/pytest/blob/main/src/_pytest/capture.py>`_.
 - `The debugging module in pytest
   <https://github.com/pytest-dev/pytest/blob/main/src/_pytest/debugging.py>`_.
 
 """
+
 from __future__ import annotations
 
+import abc
 import contextlib
-import functools
 import io
 import os
 import sys
 from io import UnsupportedOperation
 from tempfile import TemporaryFile
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import AnyStr
-from typing import final
+from typing import BinaryIO
 from typing import Generator
 from typing import Generic
 from typing import Iterator
+from typing import NamedTuple
 from typing import TextIO
-from typing import TYPE_CHECKING
+from typing import final
 
 import click
+from typing_extensions import Self
+
 from _pytask.capture_utils import CaptureMethod
 from _pytask.capture_utils import ShowCapture
 from _pytask.click import EnumChoice
 from _pytask.pluginmanager import hookimpl
 from _pytask.shared import convert_to_enum
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
     from _pytask.node_protocols import PTask
 
 
 @hookimpl
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Add CLI options for capturing output."""
     additional_parameters = [
@@ -137,30 +144,37 @@
         super().__init__()
 
     def write(self, s: str) -> int:
         super().write(s)
         return self._other.write(s)
 
 
-class DontReadFromInput:
+class DontReadFromInput(TextIO):
     """Class to disable reading from stdin while capturing is activated."""
 
-    encoding = None
+    @property
+    def encoding(self) -> str:
+        return sys.__stdin__.encoding
 
-    def read(self, *_args: Any) -> None:
+    def read(self, size: int = -1) -> str:  # noqa: ARG002
         msg = (
             "pytask: reading from stdin while output is captured! Consider using `-s`."
         )
         raise OSError(msg)
 
     readline = read
-    readlines = read
-    __next__ = read
 
-    def __iter__(self) -> DontReadFromInput:
+    def __next__(self) -> str:
+        return self.readline()
+
+    def readlines(self, hint: int | None = -1) -> list[str]:  # noqa: ARG002
+        msg = "reading from stdin while output is captured!  Consider using `-s`."
+        raise OSError(msg)
+
+    def __iter__(self) -> Iterator[str]:
         return self
 
     def fileno(self) -> int:
         msg = "redirected stdin is pseudofile, has no fileno()"
         raise UnsupportedOperation(msg)
 
     def flush(self) -> None:
@@ -172,87 +186,149 @@
 
     def close(self) -> None:
         pass
 
     def readable(self) -> bool:
         return False
 
-    def seek(self, offset: int) -> int:  # noqa: ARG002
+    def seek(self, offset: int, whence: int = 0) -> int:  # noqa: ARG002
         msg = "Redirected stdin is pseudofile, has no seek(int)."
         raise UnsupportedOperation(msg)
 
     def seekable(self) -> bool:
         return False
 
     def tell(self) -> int:
         msg = "Redirected stdin is pseudofile, has no tell()."
         raise UnsupportedOperation(msg)
 
-    def truncate(self, size: int) -> None:  # noqa: ARG002
+    def truncate(self, size: int | None = None) -> int:  # noqa: ARG002
         msg = "Cannot truncate stdin."
         raise UnsupportedOperation(msg)
 
-    def write(self, *args: Any) -> None:  # noqa: ARG002
+    def write(self, data: str) -> int:  # noqa: ARG002
         msg = "Cannot write to stdin."
         raise UnsupportedOperation(msg)
 
     def writelines(self, *args: Any) -> None:  # noqa: ARG002
         msg = "Cannot write to stdin."
         raise UnsupportedOperation(msg)
 
     def writable(self) -> bool:
         return False
 
-    @property
-    def buffer(self) -> DontReadFromInput:
+    def __enter__(self) -> Self:
         return self
 
+    def __exit__(
+        self,
+        type: type[BaseException] | None,  # noqa: A002
+        value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> None:
+        pass
+
+    @property
+    def buffer(self) -> BinaryIO:
+        # The str/bytes doesn't actually matter in this type, so OK to fake.
+        return self  # type: ignore[return-value]
+
 
 # Capture classes.
 
 
+class CaptureBase(abc.ABC, Generic[AnyStr]):
+    EMPTY_BUFFER: AnyStr
+
+    @abc.abstractmethod
+    def __init__(self, fd: int) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def start(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def done(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def suspend(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def resume(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def writeorg(self, data: AnyStr) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def snap(self) -> AnyStr:
+        raise NotImplementedError
+
+
 patchsysdict = {0: "stdin", 1: "stdout", 2: "stderr"}
 """dict[int, str]: Map file descriptors to their names."""
 
 
-class NoCapture:
+class NoCapture(CaptureBase[str]):
     """Dummy class when capturing is disabled."""
 
-    EMPTY_BUFFER = None
-    __init__ = start = done = suspend = resume = lambda *_args: None
+    EMPTY_BUFFER = ""
+
+    def __init__(self, fd: int) -> None:
+        pass
+
+    def start(self) -> None:
+        pass
 
+    def done(self) -> None:
+        pass
 
-class SysCaptureBinary:
+    def suspend(self) -> None:
+        pass
+
+    def resume(self) -> None:
+        pass
+
+    def snap(self) -> str:
+        return ""
+
+    def writeorg(self, data: str) -> None:
+        pass
+
+
+class SysCaptureBase(CaptureBase[AnyStr]):
     """Capture IO to/from Python's buffer for stdin, stdout, and stderr.
 
     Instead of :class:`SysCapture`, this class produces bytes instead of text.
 
     """
 
-    EMPTY_BUFFER = b""
-
-    def __init__(  # type: ignore
+    def __init__(
         self,
         fd: int,
-        tmpfile=None,  # noqa: ANN001
+        tmpfile: TextIO | None = None,
         *,
         tee: bool = False,
     ) -> None:
         name = patchsysdict[fd]
-        self._old = getattr(sys, name)
+        self._old: TextIO = getattr(sys, name)
         self.name = name
         if tmpfile is None:
             if name == "stdin":
                 tmpfile = DontReadFromInput()
             else:
                 tmpfile = CaptureIO() if not tee else TeeCaptureIO(self._old)
         self.tmpfile = tmpfile
         self._state = "initialized"
 
-    def repr(self, class_name: str) -> str:  # noqa: A003
+    def repr(self, class_name: str) -> str:
         return "<{} {} _old={} _state={!r} tmpfile={!r}>".format(
             class_name,
             self.name,
             hasattr(self, "_old") and repr(self._old) or "<UNSET>",
             self._state,
             self.tmpfile,
         )
@@ -274,22 +350,14 @@
         )
 
     def start(self) -> None:
         self._assert_state("start", ("initialized",))
         setattr(sys, self.name, self.tmpfile)
         self._state = "started"
 
-    def snap(self) -> str:
-        self._assert_state("snap", ("started", "suspended"))
-        self.tmpfile.seek(0)
-        res = self.tmpfile.buffer.read()
-        self.tmpfile.seek(0)
-        self.tmpfile.truncate()
-        return res
-
     def done(self) -> None:
         self._assert_state("done", ("initialized", "started", "suspended", "done"))
         if self._state == "done":
             return
         setattr(sys, self.name, self._old)
         del self._old
         self.tmpfile.close()
@@ -303,51 +371,63 @@
     def resume(self) -> None:
         self._assert_state("resume", ("started", "suspended"))
         if self._state == "started":
             return
         setattr(sys, self.name, self.tmpfile)
         self._state = "started"
 
-    def writeorg(self, data: str) -> None:
+
+class SysCaptureBinary(SysCaptureBase[bytes]):
+    EMPTY_BUFFER = b""
+
+    def snap(self) -> bytes:
+        self._assert_state("snap", ("started", "suspended"))
+        self.tmpfile.seek(0)
+        res = self.tmpfile.buffer.read()
+        self.tmpfile.seek(0)
+        self.tmpfile.truncate()
+        return res
+
+    def writeorg(self, data: bytes) -> None:
         self._assert_state("writeorg", ("started", "suspended"))
         self._old.flush()
         self._old.buffer.write(data)
         self._old.buffer.flush()
 
 
-class SysCapture(SysCaptureBinary):
+class SysCapture(SysCaptureBase[str]):
     """Capture IO to/from Python's buffer for stdin, stdout, and stderr.
 
     Instead of :class:`SysCaptureBinary`, this class produces text instead of bytes.
 
     """
 
-    EMPTY_BUFFER = ""  # type: ignore[assignment]
+    EMPTY_BUFFER = ""
 
     def snap(self) -> str:
+        self._assert_state("snap", ("started", "suspended"))
+        assert isinstance(self.tmpfile, CaptureIO)
         res = self.tmpfile.getvalue()
         self.tmpfile.seek(0)
         self.tmpfile.truncate()
         return res
 
     def writeorg(self, data: str) -> None:
         self._assert_state("writeorg", ("started", "suspended"))
         self._old.write(data)
         self._old.flush()
 
 
-class FDCaptureBinary:
+class FDCaptureBase(CaptureBase[AnyStr]):
     """Capture IO to/from a given OS-level file descriptor.
 
     snap() produces `bytes`.
 
     """
 
-    EMPTY_BUFFER = b""
-
     def __init__(self, targetfd: int) -> None:
         self.targetfd = targetfd
 
         try:
             os.fstat(targetfd)
         except OSError:
             # FD capturing is conceptually simple -- create a temporary file, redirect
@@ -365,32 +445,32 @@
             os.dup2(self.targetfd_invalid, targetfd)
         else:
             self.targetfd_invalid = None
         self.targetfd_save = os.dup(targetfd)
 
         if targetfd == 0:
             self.tmpfile = open(os.devnull, encoding="utf-8")  # noqa: SIM115, PTH123
-            self.syscapture = SysCapture(targetfd)
+            self.syscapture: CaptureBase[str] = SysCapture(targetfd)
         else:
             self.tmpfile = EncodedFile(
                 TemporaryFile(buffering=0),
                 encoding="utf-8",
                 errors="replace",
                 newline="",
                 write_through=True,
             )
             if targetfd in patchsysdict:
                 self.syscapture = SysCapture(targetfd, self.tmpfile)
             else:
-                self.syscapture = NoCapture()
+                self.syscapture = NoCapture(targetfd)
 
         self._state = "initialized"
 
     def __repr__(self) -> str:
-        return "<{} {} oldfd={} _state={!r} tmpfile={!r}>".format(
+        return "<{} {} oldfd={} _state={!r} tmpfile={!r}>".format(  # noqa: UP032
             self.__class__.__name__,
             self.targetfd,
             self.targetfd_save,
             self._state,
             self.tmpfile,
         )
 
@@ -404,22 +484,14 @@
     def start(self) -> None:
         """Start capturing on targetfd using memorized tmpfile."""
         self._assert_state("start", ("initialized",))
         os.dup2(self.tmpfile.fileno(), self.targetfd)
         self.syscapture.start()
         self._state = "started"
 
-    def snap(self) -> bytes:
-        self._assert_state("snap", ("started", "suspended"))
-        self.tmpfile.seek(0)
-        res = self.tmpfile.buffer.read()
-        self.tmpfile.seek(0)
-        self.tmpfile.truncate()
-        return res
-
     def done(self) -> None:
         """Stop capturing.
 
         Stop capturing, restore streams, return original capture file, seeked to
         position zero.
 
         """
@@ -448,103 +520,84 @@
         self._assert_state("resume", ("started", "suspended"))
         if self._state == "started":
             return
         self.syscapture.resume()
         os.dup2(self.tmpfile.fileno(), self.targetfd)
         self._state = "started"
 
+
+class FDCaptureBinary(FDCaptureBase[bytes]):
+    """Capture IO to/from a given OS-level file descriptor.
+
+    snap() produces `bytes`.
+    """
+
+    EMPTY_BUFFER = b""
+
+    def snap(self) -> bytes:
+        self._assert_state("snap", ("started", "suspended"))
+        self.tmpfile.seek(0)
+        res = self.tmpfile.buffer.read()
+        self.tmpfile.seek(0)
+        self.tmpfile.truncate()
+        return res
+
     def writeorg(self, data: bytes) -> None:
         """Write to original file descriptor."""
         self._assert_state("writeorg", ("started", "suspended"))
         os.write(self.targetfd_save, data)
 
 
-class FDCapture(FDCaptureBinary):
+class FDCapture(FDCaptureBase[str]):
     """Capture IO to/from a given OS-level file descriptor.
 
     snap() produces text.
 
     """
 
-    # Ignore type because it doesn't match the type in the superclass (bytes).
-    EMPTY_BUFFER = ""  # type: ignore
+    EMPTY_BUFFER = ""
 
-    # Ignore type because it doesn't match the type in the superclass (bytes).
-    def snap(self) -> str:  # type: ignore
+    def snap(self) -> str:
         self._assert_state("snap", ("started", "suspended"))
         self.tmpfile.seek(0)
         res = self.tmpfile.read()
         self.tmpfile.seek(0)
         self.tmpfile.truncate()
         return res
 
-    # Ignore type because it doesn't match the type in the superclass (bytes).
-    def writeorg(self, data: str) -> None:  # type: ignore
+    def writeorg(self, data: str) -> None:
         """Write to original file descriptor."""
-        super().writeorg(data.encode("utf-8"))
+        self._assert_state("writeorg", ("started", "suspended"))
+        # Will be fixed by pytest. Use encoding of original stream
+        os.write(self.targetfd_save, data.encode("utf-8"))
 
 
 # MultiCapture
 
 
-@final
-@functools.total_ordering
-class CaptureResult(Generic[AnyStr]):
-    """The result of :meth:`MultiCapture.readouterr` which wraps stdout and stderr.
-
-    This class was a namedtuple, but due to mypy limitation [0]_ it could not be made
-    generic, so was replaced by a regular class which tries to emulate the pertinent
-    parts of a namedtuple. If the mypy limitation is ever lifted, can make it a
-    namedtuple again (https://github.com/python/mypy/issues/685).
-
-    """
-
-    __slots__ = ("out", "err")
-
-    def __init__(self, out: AnyStr, err: AnyStr) -> None:
-        self.out: AnyStr = out
-        self.err: AnyStr = err
-
-    def __len__(self) -> int:
-        return 2
-
-    def __iter__(self) -> Iterator[AnyStr]:
-        return iter((self.out, self.err))
-
-    def __getitem__(self, item: int) -> AnyStr:
-        return tuple(self)[item]
-
-    def _replace(
-        self, *, out: AnyStr | None = None, err: AnyStr | None = None
-    ) -> CaptureResult[AnyStr]:
-        return CaptureResult(
-            out=self.out if out is None else out, err=self.err if err is None else err
-        )
-
-    def count(self, value: AnyStr) -> int:
-        return tuple(self).count(value)
-
-    def index(self, value: int) -> int:
-        return tuple(self).index(value)
+# Generic NamedTuple only supported since Python 3.11.
+if sys.version_info >= (3, 11) or TYPE_CHECKING:
 
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, (CaptureResult, tuple)):
-            return NotImplemented
-        return tuple(self) == tuple(other)
-
-    def __hash__(self) -> int:
-        return hash(tuple(self))
-
-    def __lt__(self, other: object) -> bool:
-        if not isinstance(other, (CaptureResult, tuple)):
-            return NotImplemented
-        return tuple(self) < tuple(other)
+    @final
+    class CaptureResult(NamedTuple, Generic[AnyStr]):
+        """A class for capture results."""
+
+        out: AnyStr
+        err: AnyStr
+
+else:
+    import collections
+
+    class CaptureResult(
+        collections.namedtuple("CaptureResult", ["out", "err"]),  # noqa: PYI024
+        Generic[AnyStr],
+    ):
+        """A class for capture results."""
 
-    def __repr__(self) -> str:
-        return f"CaptureResult(out={self.out!r}, err={self.err!r})"
+        __slots__ = ()
 
 
 class MultiCapture(Generic[AnyStr]):
     """The class which manages the buffers connected to each stream.
 
     The class is instantiated with buffers for ``stdin``, ``stdout`` and ``stderr``.
     Then, the instance provides convenient methods to control all buffers at once, like
@@ -553,24 +606,24 @@
     """
 
     _state = None
     _in_suspended = False
 
     def __init__(
         self,
-        in_: FDCapture | SysCapture | None,
-        out: FDCapture | SysCapture | None,
-        err: FDCapture | SysCapture | None,
+        in_: CaptureBase[AnyStr] | None,
+        out: CaptureBase[AnyStr] | None,
+        err: CaptureBase[AnyStr] | None,
     ) -> None:
-        self.in_ = in_
-        self.out = out
-        self.err = err
+        self.in_: CaptureBase[AnyStr] | None = in_
+        self.out: CaptureBase[AnyStr] | None = out
+        self.err: CaptureBase[AnyStr] | None = err
 
     def __repr__(self) -> str:
-        return (
+        return (  # noqa: UP032
             "<MultiCapture out={!r} err={!r} in_={!r} _state={!r} "
             "_in_suspended={!r}>"
         ).format(
             self.out,
             self.err,
             self.in_,
             self._state,
@@ -586,17 +639,17 @@
         if self.err:
             self.err.start()
 
     def pop_outerr_to_orig(self) -> tuple[AnyStr, AnyStr]:
         """Pop current snapshot out/err capture and flush to orig streams."""
         out, err = self.readouterr()
         if out:
-            self.out.writeorg(out)  # type: ignore
+            self.out.writeorg(out)  # type: ignore[union-attr]
         if err:
-            self.err.writeorg(err)  # type: ignore
+            self.err.writeorg(err)  # type: ignore[union-attr]
         return out, err
 
     def suspend_capturing(self, in_: bool = False) -> None:
         self._state = "suspended"
         if self.out:
             self.out.suspend()
         if self.err:
@@ -631,15 +684,16 @@
     def is_started(self) -> bool:
         """Whether actively capturing -- not suspended or stopped."""
         return self._state == "started"
 
     def readouterr(self) -> CaptureResult[AnyStr]:
         out = self.out.snap() if self.out else ""
         err = self.err.snap() if self.err else ""
-        return CaptureResult(out, err)  # type: ignore
+        # Will be fixed by pytest. This type error is real, need to fix.
+        return CaptureResult(out, err)  # type: ignore[arg-type]
 
 
 def _get_multicapture(method: CaptureMethod) -> MultiCapture[str]:
     """Set up the MultiCapture class with the passed method.
 
     For each valid method, the function instantiates the :class:`MultiCapture` class
     with the specified buffers for ``stdin``, ``stdout``, and ``stderr``.
@@ -676,15 +730,15 @@
     """
 
     def __init__(self, method: CaptureMethod) -> None:
         self._method = method
         self._capturing: MultiCapture[str] | None = None
 
     def __repr__(self) -> str:
-        return ("<CaptureManager _method={!r} _capturing={!r}>").format(
+        return ("<CaptureManager _method={!r} _capturing={!r}>").format(  # noqa: UP032
             self._method, self._capturing
         )
 
     def is_capturing(self) -> bool:
         return self._method != "no"
 
     def start_capturing(self) -> None:
@@ -720,47 +774,47 @@
         self.resume()
 
         try:
             yield
         finally:
             self.suspend(in_=False)
 
-        out, err = self.read()
-        if out:
-            task.report_sections.append((when, "stdout", out))
-        if err:
-            task.report_sections.append((when, "stderr", err))
+            out, err = self.read()
+            if out:
+                task.report_sections.append((when, "stdout", out))
+            if err:
+                task.report_sections.append((when, "stderr", err))
 
     # Hooks
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task_setup(self, task: PTask) -> Generator[None, None, None]:
         """Capture output during setup."""
         with self.task_capture("setup", task):
-            yield
+            return (yield)
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task(self, task: PTask) -> Generator[None, None, None]:
         """Capture output during execution."""
         with self.task_capture("call", task):
-            yield
+            return (yield)
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task_teardown(self, task: PTask) -> Generator[None, None, None]:
         """Capture output during teardown."""
         with self.task_capture("teardown", task):
-            yield
+            return (yield)
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_collect_log(self) -> Generator[None, None, None]:
         """Suspend capturing at the end of the collection.
 
         This hook needs to be here as long as the collection has no proper capturing. If
         ``pdb.set_trace`` stops the collection, continuation in ``do_continue`` enables
         the capture manager. Then, the collection status will be captured and displayed
         in the output of the first task.
 
         Here, we stop the capture manager before logging the final collection status.
 
         """
         self.suspend(in_=True)
-        yield
+        return (yield)
```

### Comparing `pytask-0.4.7/src/_pytask/clean.py` & `pytask-0.5.0/src/_pytask/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Add a command to clean the project from files unknown to pytask."""
+
 from __future__ import annotations
 
 import enum
 import itertools
 import shutil
 import sys
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
 from typing import Iterable
-from typing import TYPE_CHECKING
 
 import click
+from attrs import define
+
 from _pytask.click import ColoredCommand
 from _pytask.click import EnumChoice
 from _pytask.console import console
 from _pytask.exceptions import CollectionError
 from _pytask.git import get_all_files
 from _pytask.git import get_root
 from _pytask.git import is_git_installed
@@ -27,16 +30,14 @@
 from _pytask.path import relative_to
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.shared import to_list
 from _pytask.traceback import Traceback
 from _pytask.tree_util import tree_leaves
-from attrs import define
-
 
 if TYPE_CHECKING:
     from typing import NoReturn
 
 
 class _CleanMode(enum.Enum):
     DRY_RUN = "dry-run"
```

### Comparing `pytask-0.4.7/src/_pytask/cli.py` & `pytask-0.5.0/src/_pytask/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Implements the command line interface."""
+
 from __future__ import annotations
 
 from typing import Any
 
 import click
-from _pytask.click import ColoredGroup
-from _pytask.pluginmanager import storage
 from packaging.version import parse as parse_version
 
+from _pytask.click import ColoredGroup
+from _pytask.pluginmanager import storage
 
 _CONTEXT_SETTINGS: dict[str, Any] = {
     "help_option_names": ("-h", "--help"),
     "show_default": True,
 }
```

### Comparing `pytask-0.4.7/src/_pytask/click.py` & `pytask-0.5.0/src/_pytask/click.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Contains code related to click."""
+
 from __future__ import annotations
 
 import inspect
 from enum import Enum
 from gettext import gettext as _
 from gettext import ngettext
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import ClassVar
-from typing import TYPE_CHECKING
 
 import click
-from _pytask import __version__ as version
-from _pytask.console import console
 from click import Choice
 from click import Command
 from click import Context
 from click import Parameter
 from click.parser import split_opt
 from click_default_group import DefaultGroup
 from rich.highlighter import RegexHighlighter
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 
+from _pytask import __version__ as version
+from _pytask.console import console
+
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 
 __all__ = ["ColoredCommand", "ColoredGroup", "EnumChoice"]
```

### Comparing `pytask-0.4.7/src/_pytask/collect.py` & `pytask-0.5.0/src/_pytask/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 """Implement functionality to collect tasks."""
+
 from __future__ import annotations
 
 import inspect
 import itertools
 import os
 import sys
 import time
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
 from typing import Iterable
-from typing import TYPE_CHECKING
 
+from rich.text import Text
+from upath import UPath
+
+from _pytask.coiled_utils import Function
+from _pytask.coiled_utils import extract_coiled_function_kwargs
 from _pytask.collect_utils import create_name_of_python_node
 from _pytask.collect_utils import parse_dependencies_from_task_function
 from _pytask.collect_utils import parse_products_from_task_function
 from _pytask.config import IS_FILE_SYSTEM_CASE_SENSITIVE
 from _pytask.console import console
 from _pytask.console import create_summary_panel
 from _pytask.console import get_file
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import NodeNotCollectedError
 from _pytask.mark import MarkGenerator
 from _pytask.mark_utils import get_all_marks
 from _pytask.mark_utils import has_mark
 from _pytask.node_protocols import PNode
 from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
+from _pytask.nodes import DirectoryNode
 from _pytask.nodes import PathNode
 from _pytask.nodes import PythonNode
 from _pytask.nodes import Task
 from _pytask.nodes import TaskWithoutPath
 from _pytask.outcomes import CollectionOutcome
 from _pytask.outcomes import count_outcomes
 from _pytask.path import find_case_sensitive_path
 from _pytask.path import import_path
 from _pytask.path import shorten_path
 from _pytask.pluginmanager import hookimpl
 from _pytask.reports import CollectionReport
 from _pytask.shared import find_duplicates
 from _pytask.shared import to_list
+from _pytask.shared import unwrap_task_function
 from _pytask.task_utils import COLLECTED_TASKS
 from _pytask.task_utils import task as task_decorator
 from _pytask.typing import is_task_function
-from rich.text import Text
-
-try:
-    from upath import UPath
-except ImportError:  # pragma: no cover
-
-    class UPath:  # type: ignore[no-redef]
-        ...
-
 
 if TYPE_CHECKING:
-    from _pytask.session import Session
     from _pytask.models import NodeInfo
+    from _pytask.session import Session
 
 
 @hookimpl
 def pytask_collect(session: Session) -> bool:
     """Collect tasks."""
     session.collection_start = time.time()
 
@@ -300,80 +300,71 @@
             msg = (
                 "The task cannot have mixed priorities. Do not apply "
                 "'@pytask.mark.try_first' and '@pytask.mark.try_last' at the same time."
             )
             raise ValueError(msg)
 
         path_nodes = Path.cwd() if path is None else path.parent
+
+        # Collect dependencies and products.
         dependencies = parse_dependencies_from_task_function(
             session, path, name, path_nodes, obj
         )
         products = parse_products_from_task_function(
             session, path, name, path_nodes, obj
         )
 
         markers = get_all_marks(obj)
-        collection_id = obj.pytask_meta._id if hasattr(obj, "pytask_meta") else None
-        after = obj.pytask_meta.after if hasattr(obj, "pytask_meta") else []
 
-        # Get the underlying function to avoid having different states of the function,
-        # e.g. due to pytask_meta, in different layers of the wrapping.
-        unwrapped = inspect.unwrap(obj)
+        if hasattr(obj, "pytask_meta"):
+            attributes = {
+                **obj.pytask_meta.attributes,
+                "collection_id": obj.pytask_meta._id,
+                "after": obj.pytask_meta.after,
+                "is_generator": obj.pytask_meta.is_generator,
+            }
+        else:
+            attributes = {"collection_id": None, "after": [], "is_generator": False}
+
+        unwrapped = unwrap_task_function(obj)
+        if isinstance(unwrapped, Function):
+            attributes["coiled_kwargs"] = extract_coiled_function_kwargs(unwrapped)
+            unwrapped = unwrap_task_function(unwrapped.function)
 
         if path is None:
             return TaskWithoutPath(
                 name=name,
                 function=unwrapped,
                 depends_on=dependencies,
                 produces=products,
                 markers=markers,
-                attributes={"collection_id": collection_id, "after": after},
+                attributes=attributes,
             )
         return Task(
             base_name=name,
             path=path,
             function=unwrapped,
             depends_on=dependencies,
             produces=products,
             markers=markers,
-            attributes={"collection_id": collection_id, "after": after},
+            attributes=attributes,
         )
     if isinstance(obj, PTask):
         return obj
     return None
 
 
-_TEMPLATE_ERROR: str = """\
-The provided path of the dependency/product is
-
-{}
-
-, but the path of the file on disk is
-
-{}
-
-Case-sensitive file systems would raise an error because the upper and lower case \
-format of the paths does not match.
-
-Please, align the names to ensure reproducibility on case-sensitive file systems \
-(often Linux or macOS) or disable this error with 'check_casing_of_paths = false' in \
-the pyproject.toml file.
-
-Hint: If parts of the path preceding your project directory are not properly \
-formatted, check whether you need to call `.resolve()` on `SRC`, `BLD` or other paths \
-created from the `__file__` attribute of a module.
-"""
-
-
 _TEMPLATE_ERROR_DIRECTORY: str = """\
 The path '{path}' points to a directory, although only files are allowed."""
 
 
 @hookimpl(trylast=True)
-def pytask_collect_node(session: Session, path: Path, node_info: NodeInfo) -> PNode:  # noqa: C901, PLR0912
+def pytask_collect_node(  # noqa: C901, PLR0912
+    session: Session, path: Path, node_info: NodeInfo
+) -> PNode | PProvisionalNode:
     """Collect a node of a task as a :class:`pytask.PNode`.
 
     Strings are assumed to be paths. This might be a strict assumption, but since this
     hook is executed at last and possible errors will be shown, it seems reasonable and
     unproblematic.
 
     ``trylast=True`` might be necessary if other plugins try to parse strings themselves
@@ -385,14 +376,29 @@
         The path helps if the path of the node is given relative to the task. The path
         either points to the parent directory of the task module or to the current
         working directory for tasks defined in the REPL or in Jupyter notebooks.
 
     """
     node = node_info.value
 
+    if isinstance(node, DirectoryNode):
+        if node.root_dir is None:
+            node.root_dir = path
+        if (
+            not node.name
+            or node.name == node.root_dir.joinpath(node.pattern).as_posix()
+        ):
+            short_root_dir = shorten_path(
+                node.root_dir, session.config["paths"] or (session.config["root"],)
+            )
+            node.name = Path(short_root_dir, node.pattern).as_posix()
+
+    if isinstance(node, PProvisionalNode):
+        return node
+
     if isinstance(node, PythonNode):
         node.node_info = node_info
         if not node.name:
             node.name = create_name_of_python_node(node_info)
         return node
 
     if isinstance(node, PPathNode) and not node.path.is_absolute():
@@ -419,17 +425,19 @@
         isinstance(node, PPathNode)
         and not isinstance(node.path, UPath)
         and node.path.is_dir()
     ):
         raise ValueError(_TEMPLATE_ERROR_DIRECTORY.format(path=node.path))
 
     if isinstance(node, PNode):
+        if not node.name:
+            node.name = create_name_of_python_node(node_info)
         return node
 
-    if isinstance(node, UPath):
+    if isinstance(node, UPath):  # pragma: no cover
         if not node.protocol:
             node = Path(node)
         else:
             return PathNode(name=node.name, path=node)
 
     if isinstance(node, Path):
         if not node.is_absolute():
@@ -440,15 +448,15 @@
         node = Path(os.path.normpath(node))
         _raise_error_if_casing_of_path_is_wrong(
             node, session.config["check_casing_of_paths"]
         )
         name = shorten_path(node, session.config["paths"] or (session.config["root"],))
 
         if isinstance(node, Path) and node.is_dir():
-            raise ValueError(_TEMPLATE_ERROR_DIRECTORY.format(path=path))
+            raise ValueError(_TEMPLATE_ERROR_DIRECTORY.format(path=node))
 
         return PathNode(name=name, path=node)
 
     # Allowing a PythonNode as a return is a poor fallback, because it cannot be used.
     # Probably, the user made a mistake like writing a custom node that does not
     # strictly follow the protocol or some other misspecification.
     if node_info.arg_name == "return":
@@ -460,14 +468,36 @@
         )
         raise ValueError(msg)
 
     node_name = create_name_of_python_node(node_info)
     return PythonNode(value=node, name=node_name, node_info=node_info)
 
 
+_TEMPLATE_ERROR: str = """\
+The provided path of the dependency/product is
+
+{}
+
+, but the path of the file on disk is
+
+{}
+
+Case-sensitive file systems would raise an error because the upper and lower case \
+format of the paths does not match.
+
+Please, align the names to ensure reproducibility on case-sensitive file systems \
+(often Linux or macOS) or disable this error with 'check_casing_of_paths = false' in \
+your pytask configuration file.
+
+Hint: If parts of the path preceding your project directory are not properly \
+formatted, check whether you need to call `.resolve()` on `SRC`, `BLD` or other paths \
+created from the `__file__` attribute of a module.
+"""
+
+
 def _raise_error_if_casing_of_path_is_wrong(
     path: Path, check_casing_of_paths: bool
 ) -> None:
     """Raise an error if the path does not have the correct casing."""
     if (  # pragma: no cover
         not IS_FILE_SYSTEM_CASE_SENSITIVE
         and sys.platform == "win32"
```

### Comparing `pytask-0.4.7/src/_pytask/collect_command.py` & `pytask-0.5.0/src/_pytask/collect_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Contains the implementation of ``pytask collect``."""
+
 from __future__ import annotations
 
 import sys
 from collections import defaultdict
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 import click
+from rich.text import Text
+from rich.tree import Tree
+
 from _pytask.click import ColoredCommand
+from _pytask.console import FILE_ICON
+from _pytask.console import PYTHON_ICON
+from _pytask.console import TASK_ICON
 from _pytask.console import console
 from _pytask.console import create_url_style_for_path
-from _pytask.console import FILE_ICON
 from _pytask.console import format_node_name
 from _pytask.console import format_task_name
-from _pytask.console import PYTHON_ICON
-from _pytask.console import TASK_ICON
+from _pytask.dag import create_dag
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.exceptions import ResolvingDependenciesError
 from _pytask.mark import select_by_keyword
 from _pytask.mark import select_by_mark
 from _pytask.node_protocols import PPathNode
 from _pytask.node_protocols import PTask
@@ -26,17 +31,14 @@
 from _pytask.outcomes import ExitCode
 from _pytask.path import find_common_ancestor
 from _pytask.path import relative_to
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.tree_util import tree_leaves
-from rich.text import Text
-from rich.tree import Tree
-
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import NoReturn
 
 
 @hookimpl(tryfirst=True)
@@ -65,15 +67,15 @@
         session = Session(exit_code=ExitCode.CONFIGURATION_FAILED)
         console.print_exception()
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_dag(session=session)
+            session.dag = create_dag(session=session)
 
             tasks = _select_tasks_by_expressions_and_marker(session)
             task_with_path = [t for t in tasks if isinstance(t, PTaskWithPath)]
 
             common_ancestor = _find_common_ancestor_of_all_nodes(
                 task_with_path, session.config["paths"], session.config["nodes"]
             )
```

### Comparing `pytask-0.4.7/src/_pytask/compat.py` & `pytask-0.5.0/src/_pytask/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains functions to assess compatibility and optional dependencies."""
+
 from __future__ import annotations
 
 import shutil
 import sys
 import warnings
 from importlib import import_module
 from typing import TYPE_CHECKING
```

### Comparing `pytask-0.4.7/src/_pytask/config.py` & `pytask-0.5.0/src/_pytask/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Configure pytask."""
+
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 from _pytask.pluginmanager import hookimpl
 from _pytask.shared import parse_markers
 from _pytask.shared import parse_paths
 from _pytask.shared import to_list
 
 if TYPE_CHECKING:
@@ -76,34 +77,32 @@
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Parse the configuration."""
     config["root"].joinpath(".pytask").mkdir(exist_ok=True, parents=True)
 
     config["paths"] = parse_paths(config["paths"])
 
     config["markers"] = {
-        "depends_on": (
-            "Add dependencies to a task. See this tutorial for more information: "
-            "[link https://bit.ly/3JlxylS]https://bit.ly/3JlxylS[/]."
-        ),
-        "produces": (
-            "Add products to a task. See this tutorial for more information: "
-            "[link https://bit.ly/3JlxylS]https://bit.ly/3JlxylS[/]."
-        ),
         "try_first": "Try to execute a task a early as possible.",
         "try_last": "Try to execute a task a late as possible.",
         **config["markers"],
     }
 
     config["ignore"] = (
         to_list(config["ignore"])
         + _IGNORED_FILES_AND_FOLDERS
         + IGNORED_TEMPORARY_FILES_AND_FOLDERS
     )
 
-    config["task_files"] = to_list(config.get("task_files", "task_*.py"))
+    value = config.get("task_files", ["task_*.py"])
+    if not isinstance(value, (list, tuple)) or not all(
+        isinstance(p, str) for p in value
+    ):
+        msg = "'task_files' must be a list of patterns."
+        raise ValueError(msg)
+    config["task_files"] = value
 
     if config["stop_after_first_failure"]:
         config["max_failures"] = 1
 
     for name in ("check_casing_of_paths",):
         config[name] = bool(config.get(name, True))
```

### Comparing `pytask-0.4.7/src/_pytask/config_utils.py` & `pytask-0.5.0/src/_pytask/config_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Contains helper functions for the configuration."""
+
 from __future__ import annotations
 
 import os
 import sys
 from pathlib import Path
 from typing import Any
 from typing import Sequence
 
 import click
+
 from _pytask.shared import parse_paths
 
 if sys.version_info >= (3, 11):  # pragma: no cover
     import tomllib
 else:  # pragma: no cover
     import tomli as tomllib
 
@@ -136,8 +138,17 @@
     sections_ = sections.split(".")
 
     config = tomllib.loads(path.read_text(encoding="utf-8"))
 
     for section in sections_:
         config = config[section]
 
+    # Only convert paths when possible. Otherwise, we defer the error until the click
+    # takes over.
+    if (
+        "paths" in config
+        and isinstance(config["paths"], list)
+        and all(isinstance(p, str) for p in config["paths"])
+    ):
+        config["paths"] = [path.parent.joinpath(p).resolve() for p in config["paths"]]
+
     return config
```

### Comparing `pytask-0.4.7/src/_pytask/console.py` & `pytask-0.5.0/src/_pytask/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 """Contains the code to format output on the command line."""
+
 from __future__ import annotations
 
 import functools
 import inspect
 import os
 import sys
 from contextlib import suppress
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Literal
 from typing import Sequence
-from typing import TYPE_CHECKING
 
-from _pytask.node_protocols import PNode
-from _pytask.node_protocols import PPathNode
-from _pytask.node_protocols import PTaskWithPath
-from _pytask.path import shorten_path
 from rich.console import Console
 from rich.console import RenderableType
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.segment import Segment
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text
 from rich.theme import Theme
 from rich.tree import Tree
 
+from _pytask.node_protocols import PNode
+from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
+from _pytask.node_protocols import PTaskWithPath
+from _pytask.path import shorten_path
 
 if TYPE_CHECKING:
-    from _pytask.node_protocols import PTask
     from enum import Enum
+
+    from _pytask.node_protocols import PTask
     from _pytask.outcomes import CollectionOutcome
     from _pytask.outcomes import TaskOutcome
 
 
 __all__ = [
     "console",
     "create_summary_panel",
@@ -133,15 +136,17 @@
         return Text.assemble(
             Text(path + "::", style="dim"), Text(task_name, style=url_style)
         )
 
     return Text(task.name, style=url_style)
 
 
-def format_node_name(node: PNode, paths: Sequence[Path] = ()) -> Text:
+def format_node_name(
+    node: PNode | PProvisionalNode, paths: Sequence[Path] = ()
+) -> Text:
     """Format the name of a node."""
     if isinstance(node, PPathNode):
         if node.name != node.path.as_posix():
             return Text(node.name)
         name = shorten_path(node.path, paths)
         return Text(name)
```

### Comparing `pytask-0.4.7/src/_pytask/dag.py` & `pytask-0.5.0/src/_pytask/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,88 @@
-"""Contains code related to resolving dependencies."""
+"""Contains code related to the DAG."""
+
 from __future__ import annotations
 
 import itertools
 import sys
 from typing import TYPE_CHECKING
 
 import networkx as nx
+from rich.text import Text
+from rich.tree import Tree
+
 from _pytask.console import ARROW_DOWN_ICON
-from _pytask.console import console
 from _pytask.console import FILE_ICON
+from _pytask.console import TASK_ICON
+from _pytask.console import console
 from _pytask.console import format_node_name
 from _pytask.console import format_task_name
 from _pytask.console import render_to_string
-from _pytask.console import TASK_ICON
 from _pytask.exceptions import ResolvingDependenciesError
 from _pytask.mark import select_by_after_keyword
+from _pytask.mark import select_tasks_by_marks_and_expressions
 from _pytask.node_protocols import PNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
 from _pytask.nodes import PythonNode
-from _pytask.pluginmanager import hookimpl
 from _pytask.reports import DagReport
 from _pytask.shared import reduce_names_of_multiple_nodes
 from _pytask.tree_util import tree_map
-from rich.text import Text
-from rich.tree import Tree
 
 if TYPE_CHECKING:
     from pathlib import Path
+
     from _pytask.session import Session
 
 
-@hookimpl
-def pytask_dag(session: Session) -> bool | None:
+__all__ = ["create_dag", "create_dag_from_session"]
+
+
+def create_dag(session: Session) -> nx.DiGraph:
     """Create a directed acyclic graph (DAG) for the workflow."""
     try:
-        session.dag = session.hook.pytask_dag_create_dag(
-            session=session, tasks=session.tasks
-        )
-        session.hook.pytask_dag_modify_dag(session=session, dag=session.dag)
-
+        dag = create_dag_from_session(session)
     except Exception:  # noqa: BLE001
         report = DagReport.from_exception(sys.exc_info())
-        session.hook.pytask_dag_log(session=session, report=report)
+        _log_dag(report=report)
         session.dag_report = report
 
         raise ResolvingDependenciesError from None
+    return dag
 
-    else:
-        return True
 
+def create_dag_from_session(session: Session) -> nx.DiGraph:
+    """Create a DAG from a session."""
+    dag = _create_dag_from_tasks(tasks=session.tasks)
+    _check_if_dag_has_cycles(dag)
+    _check_if_tasks_have_the_same_products(dag, session.config["paths"])
+    dag = _modify_dag(session=session, dag=dag)
+    select_tasks_by_marks_and_expressions(session=session, dag=dag)
+    return dag
 
-@hookimpl
-def pytask_dag_create_dag(session: Session, tasks: list[PTask]) -> nx.DiGraph:
+
+def _create_dag_from_tasks(tasks: list[PTask]) -> nx.DiGraph:
     """Create the DAG from tasks, dependencies and products."""
 
-    def _add_dependency(dag: nx.DiGraph, task: PTask, node: PNode) -> None:
+    def _add_dependency(
+        dag: nx.DiGraph, task: PTask, node: PNode | PProvisionalNode
+    ) -> None:
         """Add a dependency to the DAG."""
         dag.add_node(node.signature, node=node)
         dag.add_edge(node.signature, task.signature)
 
         # If a node is a PythonNode wrapped in another PythonNode, it is a product from
         # another task that is a dependency in the current task. Thus, draw an edge
         # connecting the two nodes.
         if isinstance(node, PythonNode) and isinstance(node.value, PythonNode):
             dag.add_edge(node.value.signature, node.signature)
 
-    def _add_product(dag: nx.DiGraph, task: PTask, node: PNode) -> None:
+    def _add_product(
+        dag: nx.DiGraph, task: PTask, node: PNode | PProvisionalNode
+    ) -> None:
         """Add a product to the DAG."""
         dag.add_node(node.signature, node=node)
         dag.add_edge(task.signature, node.signature)
 
     dag = nx.DiGraph()
 
     for task in tasks:
@@ -83,23 +96,18 @@
         # connecting the two nodes.
         tree_map(
             lambda x: dag.add_edge(x.value.signature, x.signature)
             if isinstance(x, PythonNode) and isinstance(x.value, PythonNode)
             else None,
             task.depends_on,
         )
-
-    _check_if_dag_has_cycles(dag)
-    _check_if_tasks_have_the_same_products(dag, session.config["paths"])
-
     return dag
 
 
-@hookimpl
-def pytask_dag_modify_dag(session: Session, dag: nx.DiGraph) -> None:
+def _modify_dag(session: Session, dag: nx.DiGraph) -> nx.DiGraph:
     """Create dependencies between tasks when using ``@task(after=...)``."""
     temporary_id_to_task = {
         task.attributes["collection_id"]: task
         for task in session.tasks
         if "collection_id" in task.attributes
     }
     for task in session.tasks:
@@ -112,14 +120,15 @@
         elif isinstance(after, str):
             task_signature = task.signature
             signatures = select_by_after_keyword(session, after)
             signatures.discard(task_signature)
             for signature in signatures:
                 for successor in dag.successors(signature):
                     dag.add_edge(successor, task.signature)
+    return dag
 
 
 def _check_if_dag_has_cycles(dag: nx.DiGraph) -> None:
     """Check if DAG has cycles."""
     try:
         cycles = nx.algorithms.cycles.find_cycle(dag)
     except nx.NetworkXNoCycle:
@@ -142,15 +151,15 @@
     chain += [cycles[-1][1]]
 
     lines: list[str] = []
     for x in chain:
         node = dag.nodes[x].get("task") or dag.nodes[x].get("node")
         if isinstance(node, PTask):
             short_name = format_task_name(node, editor_url_scheme="no_link").plain
-        elif isinstance(node, PNode):
+        elif isinstance(node, (PNode, PProvisionalNode)):
             short_name = node.name
         lines.extend((short_name, "     " + ARROW_DOWN_ICON))
     # Join while removing last arrow.
     return "\n".join(lines[:-1])
 
 
 def _format_dictionary_to_tree(dict_: dict[str, list[str]], title: str) -> str:
@@ -187,16 +196,15 @@
         msg = (
             f"There are some tasks which produce the same output. See the following "
             f"tree which shows which products are produced by multiple tasks.\n\n{text}"
         )
         raise ResolvingDependenciesError(msg)
 
 
-@hookimpl
-def pytask_dag_log(report: DagReport) -> None:
+def _log_dag(report: DagReport) -> None:
     """Log errors which happened while resolving dependencies."""
     console.print()
     console.rule(
         Text("Failures during resolving dependencies", style="failed"), style="failed"
     )
     console.print()
     console.print(report)
```

### Comparing `pytask-0.4.7/src/_pytask/dag_command.py` & `pytask-0.5.0/src/_pytask/dag_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Contains the command and code for drawing the DAG."""
+
 from __future__ import annotations
 
 import enum
 import sys
 from pathlib import Path
 from typing import Any
 
 import click
 import networkx as nx
+from rich.text import Text
+
 from _pytask.click import ColoredCommand
 from _pytask.click import EnumChoice
 from _pytask.compat import check_for_optional_program
 from _pytask.compat import import_optional_dependency
 from _pytask.config_utils import find_project_root_and_config
 from _pytask.config_utils import read_config
 from _pytask.console import console
+from _pytask.dag import create_dag
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.exceptions import ResolvingDependenciesError
 from _pytask.outcomes import ExitCode
 from _pytask.pluginmanager import get_plugin_manager
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.shared import parse_paths
 from _pytask.shared import reduce_names_of_multiple_nodes
 from _pytask.shared import to_list
-from _pytask.traceback import remove_internal_traceback_frames_from_exc_info
-from rich.text import Text
-from rich.traceback import Traceback
+from _pytask.traceback import Traceback
 
 
 class _RankDirection(enum.Enum):
     TB = "TB"
     LR = "LR"
     BT = "BT"
     RL = "RL"
@@ -95,29 +97,28 @@
             import_optional_dependency("pygraphviz")
             check_for_optional_program(
                 session.config["layout"],
                 extra="The layout program is part of the graphviz package which you "
                 "can install with conda.",
             )
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_dag(session=session)
+            session.dag = create_dag(session=session)
             dag = _refine_dag(session)
             _write_graph(dag, session.config["output_path"], session.config["layout"])
 
         except CollectionError:  # pragma: no cover
             session.exit_code = ExitCode.COLLECTION_FAILED
 
         except ResolvingDependenciesError:  # pragma: no cover
             session.exit_code = ExitCode.DAG_FAILED
 
         except Exception:  # noqa: BLE001
             session.exit_code = ExitCode.FAILED
-            exc_info = remove_internal_traceback_frames_from_exc_info(sys.exc_info())
             console.print()
-            console.print(Traceback.from_exception(*exc_info))
+            console.print(Traceback(sys.exc_info()))
             console.rule(style="failed")
 
     session.hook.pytask_unconfigure(session=session)
     sys.exit(session.exit_code)
 
 
 def build_dag(raw_config: dict[str, Any]) -> nx.DiGraph:
@@ -150,24 +151,20 @@
         if "command" not in raw_config:
             raw_config["command"] = "dag"
             # Add defaults from cli.
             from _pytask.cli import DEFAULTS_FROM_CLI
 
             raw_config = {**DEFAULTS_FROM_CLI, **raw_config}
 
-            raw_config["paths"] = parse_paths(raw_config.get("paths"))
+            raw_config["paths"] = parse_paths(raw_config["paths"])
 
             if raw_config["config"] is not None:
                 raw_config["config"] = Path(raw_config["config"]).resolve()
                 raw_config["root"] = raw_config["config"].parent
             else:
-                if raw_config["paths"] is None:
-                    raw_config["paths"] = (Path.cwd(),)
-
-                raw_config["paths"] = parse_paths(raw_config["paths"])
                 (
                     raw_config["root"],
                     raw_config["config"],
                 ) = find_project_root_and_config(raw_config["paths"])
 
             if raw_config["config"] is not None:
                 config_from_file = read_config(raw_config["config"])
@@ -187,32 +184,25 @@
         session = Session.from_config(config)
 
     except (ConfigurationError, Exception):  # pragma: no cover
         console.print_exception()
         session = Session(exit_code=ExitCode.CONFIGURATION_FAILED)
 
     else:
-        try:
-            session.hook.pytask_log_session_header(session=session)
-            import_optional_dependency("pygraphviz")
-            check_for_optional_program(
-                session.config["layout"],
-                extra="The layout program is part of the graphviz package that you "
-                "can install with conda.",
-            )
-            session.hook.pytask_collect(session=session)
-            session.hook.pytask_dag(session=session)
-            session.hook.pytask_unconfigure(session=session)
-            dag = _refine_dag(session)
-
-        except Exception:
-            raise
-
-        else:
-            return dag
+        session.hook.pytask_log_session_header(session=session)
+        import_optional_dependency("pygraphviz")
+        check_for_optional_program(
+            session.config["layout"],
+            extra="The layout program is part of the graphviz package that you "
+            "can install with conda.",
+        )
+        session.hook.pytask_collect(session=session)
+        session.dag = create_dag(session=session)
+        session.hook.pytask_unconfigure(session=session)
+        return _refine_dag(session)
 
 
 def _refine_dag(session: Session) -> nx.DiGraph:
     """Refine the dag for plotting."""
     dag = _shorten_node_labels(session.dag, session.config["paths"])
     dag = _clean_dag(dag)
     dag = _style_dag(dag)
@@ -245,7 +235,9 @@
 
 
 def _write_graph(dag: nx.DiGraph, path: Path, layout: str) -> None:
     """Write the graph to disk."""
     path.parent.mkdir(exist_ok=True, parents=True)
     graph = nx.nx_agraph.to_agraph(dag)
     graph.draw(path, prog=layout)
+    console.print()
+    console.print(f"Written to {path}.")
```

### Comparing `pytask-0.4.7/src/_pytask/dag_utils.py` & `pytask-0.5.0/src/_pytask/dag_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Implement some capabilities to deal with the DAG."""
+
 from __future__ import annotations
 
 import itertools
+from typing import TYPE_CHECKING
 from typing import Generator
 from typing import Iterable
-from typing import TYPE_CHECKING
 
 import networkx as nx
-from _pytask.mark_utils import has_mark
 from attrs import define
 from attrs import field
 
+from _pytask.mark_utils import has_mark
+
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
 
 
 def descending_tasks(task_name: str, dag: nx.DiGraph) -> Generator[str, None, None]:
     """Yield only descending tasks."""
     for descendant in nx.descendants(dag, task_name):
@@ -86,17 +88,15 @@
 
         tasks = [
             dag.nodes[node]["task"] for node in dag.nodes if "task" in dag.nodes[node]
         ]
         priorities = _extract_priorities_from_tasks(tasks)
 
         task_signatures = {task.signature for task in tasks}
-        task_dict = {
-            name: nx.ancestors(dag, name) & task_signatures for name in task_signatures
-        }
+        task_dict = {s: nx.ancestors(dag, s) & task_signatures for s in task_signatures}
         task_dag = nx.DiGraph(task_dict).reverse()
 
         return cls(dag=task_dag, priorities=priorities)
 
     @classmethod
     def from_dag_and_sorter(
         cls, dag: nx.DiGraph, sorter: TopologicalSorter
```

### Comparing `pytask-0.4.7/src/_pytask/data_catalog.py` & `pytask-0.5.0/src/_pytask/data_catalog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Contains the implementation of a data catalog.
 
 The data catalog is an abstraction layer between users and nodes.
 
 """
+
 from __future__ import annotations
 
 import hashlib
 import inspect
 import pickle
+import re
 from pathlib import Path
 from typing import Any
 
+from attrs import define
+from attrs import field
+
 from _pytask.config_utils import find_project_root_and_config
 from _pytask.exceptions import NodeNotCollectedError
 from _pytask.models import NodeInfo
 from _pytask.node_protocols import PNode
 from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.nodes import PickleNode
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
-from attrs import define
-from attrs import field
-
 
 __all__ = ["DataCatalog"]
 
 
 def _get_parent_path_of_data_catalog_module(stacklevel: int = 2) -> Path:
     """Get the parent path of the module where the data catalog is defined."""
     stack = inspect.stack()
@@ -41,86 +44,92 @@
 
     Parameters
     ----------
     default_node
         A default node for loading and saving values. By default,
         :class:`~pytask.PickleNode` is used to serialize any Python object with the
         :mod:`pickle` module.
-    entries
-        A collection of entries in the catalog. Entries can be :class:`~pytask.PNode` or
-        a :class:`DataCatalog` itself for nesting catalogs.
     name
-        The name of the data catalog. Use it when you are working with multiple data
-        catalogs that store data under the same keys.
+        The name of the data catalog which can only contain letters, numbers, hyphens
+        and underscores. Use it when you are working with multiple data catalogs to
+        store data in different locations.
     path
         A path where automatically created files are stored. By default, it will be
         ``.pytask/data_catalogs/default``.
 
     """
 
     default_node: type[PNode] = PickleNode
-    entries: dict[str, PNode] = field(factory=dict)
-    name: str = "default"
+    name: str = field(default="default")
     path: Path | None = None
+    _entries: dict[str, PNode | PProvisionalNode] = field(factory=dict)
+    _instance_path: Path = field(factory=_get_parent_path_of_data_catalog_module)
     _session_config: dict[str, Any] = field(
         factory=lambda *x: {"check_casing_of_paths": True}  # noqa: ARG005
     )
-    _instance_path: Path = field(factory=_get_parent_path_of_data_catalog_module)
+
+    @name.validator
+    def _check(self, attribute: str, value: str) -> None:  # noqa: ARG002
+        _rich_traceback_omit = True
+        if not isinstance(value, str):
+            msg = "The name of a data catalog must be a string."
+            raise TypeError(msg)
+        if not re.match(r"[a-zA-Z0-9-_]+", value):
+            msg = (
+                "The name of a data catalog must be a string containing only letters, "
+                "numbers, hyphens, and underscores."
+            )
+            raise ValueError(msg)
 
     def __attrs_post_init__(self) -> None:
         root_path, _ = find_project_root_and_config((self._instance_path,))
         self._session_config["paths"] = (root_path,)
 
         if not self.path:
             self.path = root_path / ".pytask" / "data_catalogs" / self.name
 
         self.path.mkdir(parents=True, exist_ok=True)
 
-        self._initialize()
-
-    def _initialize(self) -> None:
-        """Initialize the data catalog with persisted nodes from previous runs."""
-        for path in self.path.glob("*-node.pkl"):  # type: ignore[union-attr]
+        # Initialize the data catalog with persisted nodes from previous runs.
+        for path in self.path.glob("*-node.pkl"):
             node = pickle.loads(path.read_bytes())  # noqa: S301
-            self.entries[node.name] = node
+            self._entries[node.name] = node
 
-    def __getitem__(self, name: str) -> PNode:
+    def __getitem__(self, name: str) -> PNode | PProvisionalNode:
         """Allow to access entries with the squared brackets syntax."""
-        if name not in self.entries:
+        if name not in self._entries:
             self.add(name)
-        return self.entries[name]
+        return self._entries[name]
 
-    def add(self, name: str, node: PNode | None = None) -> None:
+    def add(self, name: str, node: PNode | PProvisionalNode | Any = None) -> None:
         """Add an entry to the data catalog."""
-        assert isinstance(self.path, Path)
-
         if not isinstance(name, str):
             msg = "The name of a catalog entry must be a string."
             raise TypeError(msg)
 
         if node is None:
-            filename = str(hashlib.sha256(name.encode()).hexdigest())
+            filename = hashlib.sha256(name.encode()).hexdigest()
             if isinstance(self.default_node, PPathNode):
-                self.entries[name] = self.default_node(
+                self._entries[name] = self.default_node(
                     name=name, path=self.path / f"{filename}.pkl"
                 )
             else:
-                self.entries[name] = self.default_node(name=name)  # type: ignore[call-arg]
-            self.path.joinpath(f"{filename}-node.pkl").write_bytes(
-                pickle.dumps(self.entries[name])
+                self._entries[name] = self.default_node(name=name)  # type: ignore[call-arg]
+            self.path.joinpath(f"{filename}-node.pkl").write_bytes(  # type: ignore[union-attr]
+                pickle.dumps(self._entries[name])
             )
-        elif isinstance(node, PNode):
-            self.entries[name] = node
+        elif isinstance(node, (PNode, PProvisionalNode)):
+            self._entries[name] = node
         else:
             # Acquire the latest pluginmanager.
             session = Session(config=self._session_config, hook=storage.get().hook)
             collected_node = session.hook.pytask_collect_node(
                 session=session,
                 path=self._instance_path,
                 node_info=NodeInfo(
                     arg_name=name, path=(), value=node, task_path=None, task_name=""
                 ),
             )
             if collected_node is None:  # pragma: no cover
                 msg = f"{node!r} cannot be parsed."
                 raise NodeNotCollectedError(msg)
-            self.entries[name] = collected_node
+            self._entries[name] = collected_node
```

### Comparing `pytask-0.4.7/src/_pytask/database.py` & `pytask-0.5.0/src/_pytask/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Contains hooks related to the database."""
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
 
+from sqlalchemy.engine import make_url
+
 from _pytask.database_utils import create_database
 from _pytask.pluginmanager import hookimpl
-from sqlalchemy.engine import make_url
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Parse the configuration."""
     # Set default.
     if not config["database_url"]:
```

### Comparing `pytask-0.4.7/src/_pytask/database_utils.py` & `pytask-0.5.0/src/_pytask/database_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Contains utilities for the database."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from _pytask.dag_utils import node_and_neighbors
 from sqlalchemy import create_engine
 from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import mapped_column
 from sqlalchemy.orm import sessionmaker
 
+from _pytask.dag_utils import node_and_neighbors
+
 if TYPE_CHECKING:
     from _pytask.node_protocols import PNode
     from _pytask.node_protocols import PTask
     from _pytask.session import Session
 
 
 __all__ = [
@@ -63,22 +65,21 @@
     """Update the state for each node of a task in the database."""
     for name in node_and_neighbors(session.dag, task_signature):
         node = session.dag.nodes[name].get("task") or session.dag.nodes[name]["node"]
         hash_ = node.state()
         _create_or_update_state(task_signature, node.signature, hash_)
 
 
-def has_node_changed(task: PTask, node: PTask | PNode) -> bool:
+def has_node_changed(task: PTask, node: PTask | PNode, state: str | None) -> bool:
     """Indicate whether a single dependency or product has changed."""
     # If node does not exist, we receive None.
-    node_state = node.state()
-    if node_state is None:
+    if state is None:
         return True
 
     with DatabaseSession() as session:
         db_state = session.get(State, (task.signature, node.signature))
 
     # If the node is not in the database.
     if db_state is None:
         return True
 
-    return node_state != db_state.hash_
+    return state != db_state.hash_
```

### Comparing `pytask-0.4.7/src/_pytask/debugging.py` & `pytask-0.5.0/src/_pytask/debugging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """Contains everything related to debugging."""
+
 from __future__ import annotations
 
 import functools
 import pdb  # noqa: T100
 import sys
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import ClassVar
 from typing import Generator
-from typing import TYPE_CHECKING
 
 import click
+
 from _pytask.console import console
 from _pytask.node_protocols import PTask
 from _pytask.outcomes import Exit
 from _pytask.pluginmanager import hookimpl
 from _pytask.traceback import Traceback
 
 if TYPE_CHECKING:
-    from pluggy import PluginManager
-    from _pytask.session import Session
-    from types import TracebackType
     from types import FrameType
+    from types import TracebackType
+
+    from pluggy import PluginManager
+
     from _pytask.capture import CaptureManager
     from _pytask.live import LiveManager
+    from _pytask.session import Session
 
 
 @hookimpl
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend command line interface."""
     additional_parameters = [
         click.Option(
@@ -147,15 +151,15 @@
                 mod = sys.modules[modname]
 
                 # Handle --pdbcls=pdb:pdb.Pdb (useful e.g. with pdbpp).
                 parts = classname.split(".")
                 pdb_cls = getattr(mod, parts[0])
                 for part in parts[1:]:
                     pdb_cls = getattr(pdb_cls, part)
-            except Exception as exc:  # noqa: BLE001
+            except Exception as exc:
                 value = f"{modname}:{classname}"
                 msg = f"--pdbcls: could not import {value!r}: {exc}."
                 raise ValueError(msg) from exc
         else:
             import pdb  # noqa: T100
 
             pdb_cls = pdb.Pdb
@@ -305,22 +309,22 @@
         _pdb.set_trace(frame)
 
 
 class PdbDebugger:
     """Namespace for debugging."""
 
     @staticmethod
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task(
         session: Session, task: PTask
     ) -> Generator[None, None, None]:
         """Execute a task by wrapping the function with post-mortem debugger."""
         if isinstance(task, PTask):
             wrap_function_for_post_mortem_debugging(session, task)
-        yield
+        return (yield)
 
 
 def wrap_function_for_post_mortem_debugging(session: Session, task: PTask) -> None:
     """Wrap the function for post-mortem debugging."""
     task_function = task.function
 
     @functools.wraps(task_function)
@@ -365,22 +369,22 @@
     task.function = wrapper
 
 
 class PdbTrace:
     """Namespace for tracing."""
 
     @staticmethod
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task(
         session: Session, task: PTask
     ) -> Generator[None, None, None]:
         """Wrap the task function with a tracer."""
         if isinstance(task, PTask):
             wrap_function_for_tracing(session, task)
-        yield
+        return (yield)
 
 
 def wrap_function_for_tracing(session: Session, task: PTask) -> None:
     """Wrap the task function for tracing."""
     _pdb = PytaskPDB._init_pdb("runcall")
     task_function = task.function
```

### Comparing `pytask-0.4.7/src/_pytask/exceptions.py` & `pytask-0.5.0/src/_pytask/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains custom exceptions."""
+
 from __future__ import annotations
 
 
 class PytaskError(Exception):
     """Base exception for pytask which should be inherited by all other exceptions."""
```

### Comparing `pytask-0.4.7/src/_pytask/execute.py` & `pytask-0.5.0/src/_pytask/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """Contains hook implementations concerning the execution."""
+
 from __future__ import annotations
 
 import inspect
 import sys
 import time
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
+
+from rich.text import Text
 
 from _pytask.config import IS_FILE_SYSTEM_CASE_SENSITIVE
 from _pytask.console import console
 from _pytask.console import create_summary_panel
 from _pytask.console import create_url_style_for_task
 from _pytask.console import format_node_name
 from _pytask.console import format_strings_as_flat_tree
 from _pytask.console import unify_styles
+from _pytask.dag_utils import TopologicalSorter
 from _pytask.dag_utils import descending_tasks
 from _pytask.dag_utils import node_and_neighbors
-from _pytask.dag_utils import TopologicalSorter
 from _pytask.database_utils import has_node_changed
 from _pytask.database_utils import update_states_in_database
 from _pytask.exceptions import ExecutionError
 from _pytask.exceptions import NodeLoadError
 from _pytask.exceptions import NodeNotFoundError
 from _pytask.mark import Mark
 from _pytask.mark_utils import has_mark
 from _pytask.node_protocols import PNode
 from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
-from _pytask.outcomes import count_outcomes
 from _pytask.outcomes import Exit
 from _pytask.outcomes import SkippedUnchanged
 from _pytask.outcomes import TaskOutcome
 from _pytask.outcomes import WouldBeExecuted
+from _pytask.outcomes import count_outcomes
 from _pytask.pluginmanager import hookimpl
+from _pytask.provisional_utils import collect_provisional_products
 from _pytask.reports import ExecutionReport
 from _pytask.traceback import remove_traceback_from_exc_info
 from _pytask.tree_util import tree_leaves
 from _pytask.tree_util import tree_map
 from _pytask.tree_util import tree_structure
-from rich.text import Text
-
+from _pytask.typing import is_task_generator
 
 if TYPE_CHECKING:
     from _pytask.session import Session
 
 
 @hookimpl
 def pytask_post_parse(config: dict[str, Any]) -> None:
@@ -52,15 +56,15 @@
         config["pm"].register(ShowErrorsImmediatelyPlugin)
 
 
 @hookimpl
 def pytask_execute(session: Session) -> None:
     """Execute tasks."""
     session.hook.pytask_execute_log_start(session=session)
-    session.scheduler = session.hook.pytask_execute_create_scheduler(session=session)
+    session.scheduler = TopologicalSorter.from_dag(session.dag)
     session.hook.pytask_execute_build(session=session)
     session.hook.pytask_execute_log_end(
         session=session, reports=session.execution_reports
     )
 
 
 @hookimpl
@@ -68,20 +72,14 @@
     """Start logging."""
     session.execution_start = time.time()
 
     # New line to separate note on collected items from task statuses.
     console.print()
 
 
-@hookimpl(trylast=True)
-def pytask_execute_create_scheduler(session: Session) -> TopologicalSorter:
-    """Create a scheduler based on topological sorting."""
-    return TopologicalSorter.from_dag(session.dag)
-
-
 @hookimpl
 def pytask_execute_build(session: Session) -> bool | None:
     """Execute tasks."""
     if isinstance(session.scheduler, TopologicalSorter):
         while session.scheduler.is_active():
             task_name = session.scheduler.get_ready()[0]
             task = session.dag.nodes[task_name]["task"]
@@ -116,107 +114,128 @@
     session.hook.pytask_execute_task_process_report(session=session, report=report)
     session.hook.pytask_execute_task_log_end(session=session, task=task, report=report)
 
     return report
 
 
 @hookimpl(trylast=True)
-def pytask_execute_task_setup(session: Session, task: PTask) -> None:
+def pytask_execute_task_setup(session: Session, task: PTask) -> None:  # noqa: C901
     """Set up the execution of a task.
 
     1. Check whether all dependencies of a task are available.
     2. Create the directory where the product will be placed.
 
     """
     if has_mark(task, "would_be_executed"):
         raise WouldBeExecuted
 
     dag = session.dag
 
-    needs_to_be_executed = session.config["force"]
+    # Task generators are always executed since their states are not updated, but we
+    # skip the checks as well.
+    needs_to_be_executed = session.config["force"] or is_task_generator(task)
+
     if not needs_to_be_executed:
         predecessors = set(dag.predecessors(task.signature)) | {task.signature}
         for node_signature in node_and_neighbors(dag, task.signature):
             node = dag.nodes[node_signature].get("task") or dag.nodes[
                 node_signature
             ].get("node")
-            if node_signature in predecessors and not node.state():
+
+            # Skip provisional nodes that are products since they do not have a state.
+            if node_signature not in predecessors and isinstance(
+                node, PProvisionalNode
+            ):
+                continue
+
+            node_state = node.state()
+
+            if node_signature in predecessors and not node_state:
                 msg = f"{task.name!r} requires missing node {node.name!r}."
                 if IS_FILE_SYSTEM_CASE_SENSITIVE:
                     msg += (
                         "\n\n(Hint: Your file-system is case-sensitive. Check the "
                         "paths' capitalization carefully.)"
                     )
                 raise NodeNotFoundError(msg)
 
-            has_changed = has_node_changed(task=task, node=node)
+            has_changed = has_node_changed(task=task, node=node, state=node_state)
             if has_changed:
                 needs_to_be_executed = True
                 break
 
     if not needs_to_be_executed:
+        collect_provisional_products(session, task)
         raise SkippedUnchanged
 
     # Create directory for product if it does not exist. Maybe this should be a `setup`
     # method for the node classes.
     for product in dag.successors(task.signature):
         node = dag.nodes[product]["node"]
         if isinstance(node, PPathNode):
             node.path.parent.mkdir(parents=True, exist_ok=True)
 
 
-def _safe_load(node: PNode, task: PTask, is_product: bool) -> Any:
+def _safe_load(node: PNode | PProvisionalNode, task: PTask, *, is_product: bool) -> Any:
     try:
         return node.load(is_product=is_product)
-    except Exception as e:  # noqa: BLE001
+    except Exception as e:
         msg = f"Exception while loading node {node.name!r} of task {task.name!r}"
         raise NodeLoadError(msg) from e
 
 
 @hookimpl(trylast=True)
 def pytask_execute_task(session: Session, task: PTask) -> bool:
     """Execute task."""
     if session.config["dry_run"]:
         raise WouldBeExecuted
 
     parameters = inspect.signature(task.function).parameters
 
     kwargs = {}
     for name, value in task.depends_on.items():
-        kwargs[name] = tree_map(lambda x: _safe_load(x, task, False), value)
+        kwargs[name] = tree_map(lambda x: _safe_load(x, task, is_product=False), value)
 
     for name, value in task.produces.items():
         if name in parameters:
-            kwargs[name] = tree_map(lambda x: _safe_load(x, task, True), value)
+            kwargs[name] = tree_map(
+                lambda x: _safe_load(x, task, is_product=True), value
+            )
 
     out = task.execute(**kwargs)
 
     if "return" in task.produces:
         structure_out = tree_structure(out)
         structure_return = tree_structure(task.produces["return"])
+
         # strict must be false when none is leaf.
         if not structure_return.is_prefix(structure_out, strict=False):
             msg = (
                 f"The structure of the return annotation is not a subtree of the "
                 f"structure of the function return.\n\nFunction return: {structure_out}"
                 f"\n\nReturn annotation: {structure_return}"
             )
             raise ValueError(msg)
 
         nodes = tree_leaves(task.produces["return"])
         values = structure_return.flatten_up_to(out)
         for node, value in zip(nodes, values):
-            node.save(value)
+            if not isinstance(node, PProvisionalNode):
+                node.save(value)
 
     return True
 
 
-@hookimpl
+@hookimpl(trylast=True)
 def pytask_execute_task_teardown(session: Session, task: PTask) -> None:
-    """Check if :class:`_pytask.nodes.PathNode` are produced by a task."""
+    """Check if nodes are produced by a task."""
+    if is_task_generator(task):
+        return
+
+    collect_provisional_products(session, task)
     missing_nodes = [node for node in tree_leaves(task.produces) if not node.state()]
     if missing_nodes:
         paths = session.config["paths"]
         files = [format_node_name(i, paths).plain for i in missing_nodes]
         formatted = format_strings_as_flat_tree(
             files, "The task did not produce the following files:\n"
         )
```

### Comparing `pytask-0.4.7/src/_pytask/git.py` & `pytask-0.5.0/src/_pytask/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains all functions related to git."""
+
 from __future__ import annotations
 
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Any
```

### Comparing `pytask-0.4.7/src/_pytask/hookspecs.py` & `pytask-0.5.0/src/_pytask/hookspecs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Implement hook specifications or entry-points for pytask.
 
 At each of the entry-points, a plugin can register a hook implementation which receives
 the message send by the host and may send a response.
 
 """
+
 from __future__ import annotations
 
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 import pluggy
 
-
 if TYPE_CHECKING:
+    from pathlib import Path
+
+    import click
+    from pluggy import PluginManager
+
     from _pytask.models import NodeInfo
     from _pytask.node_protocols import PNode
-    import click
+    from _pytask.node_protocols import PProvisionalNode
     from _pytask.node_protocols import PTask
-    import networkx as nx
-    from pathlib import Path
-    from _pytask.session import Session
     from _pytask.outcomes import CollectionOutcome
     from _pytask.outcomes import TaskOutcome
     from _pytask.reports import CollectionReport
     from _pytask.reports import ExecutionReport
-    from _pytask.reports import DagReport
-    from pluggy import PluginManager
+    from _pytask.session import Session
 
 
 hookspec = pluggy.HookspecMarker("pytask")
 
 
 @hookspec(historic=True)
 def pytask_add_hooks(pm: PluginManager) -> None:
@@ -191,67 +192,29 @@
 
     """
 
 
 @hookspec(firstresult=True)
 def pytask_collect_node(
     session: Session, path: Path, node_info: NodeInfo
-) -> PNode | None:
+) -> PNode | PProvisionalNode | None:
     """Collect a node which is a dependency or a product of a task."""
 
 
 @hookspec(firstresult=True)
 def pytask_collect_log(
     session: Session, reports: list[CollectionReport], tasks: list[PTask]
 ) -> None:
     """Log errors occurring during the collection.
 
     This hook reports errors during the collection.
 
     """
 
 
-# Hooks for resolving dependencies.
-
-
-@hookspec(firstresult=True)
-def pytask_dag(session: Session) -> None:
-    """Create a DAG.
-
-    The main hook implementation which controls the resolution of dependencies and calls
-    subordinated hooks.
-
-    """
-
-
-@hookspec(firstresult=True)
-def pytask_dag_create_dag(session: Session, tasks: list[PTask]) -> nx.DiGraph:
-    """Create the DAG.
-
-    This hook creates the DAG from tasks, dependencies and products. The DAG can be used
-    by a scheduler to find an execution order.
-
-    """
-
-
-@hookspec
-def pytask_dag_modify_dag(session: Session, dag: nx.DiGraph) -> None:
-    """Modify the DAG.
-
-    This hook allows to make some changes to the DAG before it is validated and tasks
-    are selected.
-
-    """
-
-
-@hookspec
-def pytask_dag_log(session: Session, report: DagReport) -> None:
-    """Log errors during resolving dependencies."""
-
-
 # Hooks for running tasks.
 
 
 @hookspec(firstresult=True)
 def pytask_execute(session: Session) -> Any | None:
     """Loop over all tasks for the execution.
 
@@ -267,24 +230,14 @@
 
     This hook allows to provide a header with information before the execution starts.
 
     """
 
 
 @hookspec(firstresult=True)
-def pytask_execute_create_scheduler(session: Session) -> Any:
-    """Create a scheduler for the execution.
-
-    The scheduler provides information on which tasks are able to be executed. Its
-    foundation is likely a topological ordering of the tasks based on the DAG.
-
-    """
-
-
-@hookspec(firstresult=True)
 def pytask_execute_build(session: Session) -> Any:
     """Execute the build.
 
     This hook implements the main loop to execute tasks.
 
     """
```

### Comparing `pytask-0.4.7/src/_pytask/live.py` & `pytask-0.5.0/src/_pytask/live.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Contains code related to live objects."""
+
 from __future__ import annotations
 
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
 from typing import NamedTuple
-from typing import TYPE_CHECKING
 
 import click
-from _pytask.console import console
-from _pytask.console import format_task_name
-from _pytask.outcomes import CollectionOutcome
-from _pytask.outcomes import TaskOutcome
-from _pytask.pluginmanager import hookimpl
 from attrs import define
 from attrs import field
 from rich.box import ROUNDED
 from rich.live import Live
 from rich.status import Status
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text
 
+from _pytask.console import console
+from _pytask.console import format_task_name
+from _pytask.logging_utils import TaskExecutionStatus
+from _pytask.outcomes import CollectionOutcome
+from _pytask.outcomes import TaskOutcome
+from _pytask.pluginmanager import hookimpl
+
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
+    from _pytask.reports import CollectionReport
     from _pytask.reports import ExecutionReport
     from _pytask.session import Session
-    from _pytask.reports import CollectionReport
 
 
 @hookimpl
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend command line interface."""
     additional_parameters = [
         click.Option(
@@ -65,22 +69,21 @@
         )
         config["pm"].register(live_execution, "live_execution")
 
     live_collection = LiveCollection(live_manager=live_manager)
     config["pm"].register(live_collection, "live_collection")
 
 
-@hookimpl(hookwrapper=True)
+@hookimpl(wrapper=True)
 def pytask_execute(session: Session) -> Generator[None, None, None]:
     if session.config["verbose"] >= 1:
         live_execution = session.config["pm"].get_plugin("live_execution")
         if live_execution:
             live_execution.n_tasks = len(session.tasks)
-
-    yield
+    return (yield)
 
 
 @define(eq=False)
 class LiveManager:
     """A class for live displays during a session.
 
     This class allows to display live information during a session and handles the
@@ -124,55 +127,63 @@
         self._live.refresh()
 
     @property
     def is_started(self) -> bool:
         return self._live.is_started
 
 
+@dataclass
+class _TaskEntry:
+    task: PTask
+    status: TaskExecutionStatus
+
+
 class _ReportEntry(NamedTuple):
     name: str
     outcome: TaskOutcome
     task: PTask
 
 
 @define(eq=False, kw_only=True)
 class LiveExecution:
     """A class for managing the table displaying task progress during the execution."""
 
     live_manager: LiveManager
     n_entries_in_table: int
     verbose: int
     editor_url_scheme: str
+    initial_status: TaskExecutionStatus = TaskExecutionStatus.RUNNING
     sort_final_table: bool = False
     n_tasks: int | str = "x"
     _reports: list[_ReportEntry] = field(factory=list)
-    _running_tasks: dict[str, PTask] = field(factory=dict)
+    _running_tasks: dict[str, _TaskEntry] = field(factory=dict)
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_build(self) -> Generator[None, None, None]:
         """Wrap the execution with the live manager and yield a table at the end."""
         self.live_manager.start()
-        yield
+        result = yield
         self.live_manager.stop(transient=True)
         table = self._generate_table(
             reduce_table=False, sort_table=self.sort_final_table, add_caption=False
         )
         if table is not None:
             console.print(table)
+        return result
 
     @hookimpl(tryfirst=True)
     def pytask_execute_task_log_start(self, task: PTask) -> bool:
         """Mark a new task as running."""
-        self.update_running_tasks(task)
+        self.add_task(new_running_task=task, status=self.initial_status)
         return True
 
     @hookimpl
     def pytask_execute_task_log_end(self, report: ExecutionReport) -> bool:
         """Mark a task as being finished and update outcome."""
-        self.update_reports(report)
+        self.update_report(report)
         return True
 
     def _generate_table(
         self, reduce_table: bool, sort_table: bool, add_caption: bool
     ) -> Table | None:
         """Generate the table.
 
@@ -226,46 +237,54 @@
         table.add_column("Task", overflow="fold")
         table.add_column("Outcome")
         for report in relevant_reports:
             table.add_row(
                 format_task_name(report.task, editor_url_scheme=self.editor_url_scheme),
                 Text(report.outcome.symbol, style=report.outcome.style),
             )
-        for task in self._running_tasks.values():
+        for task_entry in self._running_tasks.values():
             table.add_row(
-                format_task_name(task, editor_url_scheme=self.editor_url_scheme),
-                "running",
+                format_task_name(
+                    task_entry.task, editor_url_scheme=self.editor_url_scheme
+                ),
+                task_entry.status.value,
             )
 
         # If the table is empty, do not display anything.
         if table.rows == []:
-            table = None
-
+            return None
         return table
 
     def _update_table(
         self,
         reduce_table: bool = True,
         sort_table: bool = False,
         add_caption: bool = True,
     ) -> None:
         """Regenerate the table."""
         table = self._generate_table(
             reduce_table=reduce_table, sort_table=sort_table, add_caption=add_caption
         )
         self.live_manager.update(table)
 
-    def update_running_tasks(self, new_running_task: PTask) -> None:
+    def add_task(self, new_running_task: PTask, status: TaskExecutionStatus) -> None:
         """Add a new running task."""
-        self._running_tasks[new_running_task.name] = new_running_task
+        self._running_tasks[new_running_task.signature] = _TaskEntry(
+            task=new_running_task, status=status
+        )
+        self._update_table()
+
+    def update_task(self, signature: str, status: TaskExecutionStatus) -> None:
+        """Update the status of a running task."""
+        self._running_tasks[signature].status = status
         self._update_table()
 
-    def update_reports(self, new_report: ExecutionReport) -> None:
+    def update_report(self, new_report: ExecutionReport) -> None:
         """Update the status of a running task by adding its report."""
-        self._running_tasks.pop(new_report.task.name)
+        self._running_tasks.pop(new_report.task.signature)
         self._reports.append(
             _ReportEntry(
                 name=new_report.task.name,
                 outcome=new_report.outcome,
                 task=new_report.task,
             )
         )
@@ -276,31 +295,31 @@
 class LiveCollection:
     """A class for managing the live status during the collection."""
 
     live_manager: LiveManager
     _n_collected_tasks: int = 0
     _n_errors: int = 0
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_collect(self) -> Generator[None, None, None]:
         """Start the status of the collection."""
         self.live_manager.start()
-        yield
+        return (yield)
 
     @hookimpl
     def pytask_collect_file_log(self, reports: list[CollectionReport]) -> None:
         """Update the status after a file is collected."""
         self._update_statistics(reports)
         self._update_status()
 
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_collect_log(self) -> Generator[None, None, None]:
         """Stop the live display when all tasks have been collected."""
         self.live_manager.stop(transient=True)
-        yield
+        return (yield)
 
     def _update_statistics(self, reports: list[CollectionReport]) -> None:
         """Update the statistics on collected tasks and errors."""
         if reports is None:
             reports = []
         for report in reports:
             if report.outcome == CollectionOutcome.SUCCESS:
```

### Comparing `pytask-0.4.7/src/_pytask/logging.py` & `pytask-0.5.0/src/_pytask/logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """Add general logging capabilities."""
+
 from __future__ import annotations
 
 import contextlib
 import platform
 import sys
 import warnings
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import NamedTuple
-from typing import TYPE_CHECKING
 
-import _pytask
 import click
 import pluggy
-from _pytask.console import console
+from rich.text import Text
+
+import _pytask
+from _pytask.capture_utils import ShowCapture
 from _pytask.console import IS_WINDOWS_TERMINAL
+from _pytask.console import console
 from _pytask.pluginmanager import hookimpl
 from _pytask.reports import ExecutionReport
 from _pytask.traceback import Traceback
-from rich.text import Text
 
 if TYPE_CHECKING:
     from pluggy._manager import DistFacade
+
+    from _pytask.outcomes import CollectionOutcome
     from _pytask.outcomes import TaskOutcome
     from _pytask.session import Session
-    from _pytask.outcomes import CollectionOutcome
 
 
 with contextlib.suppress(ImportError):
     pass
 
 
 class _TimeUnit(NamedTuple):
@@ -60,15 +64,15 @@
             stacklevel=1,
         )
 
 
 @hookimpl
 def pytask_post_parse(config: dict[str, Any]) -> None:
     # Set class variables on traceback object.
-    Traceback.show_locals = config["show_locals"]
+    Traceback._show_locals = config["show_locals"]
     # Set class variables on Executionreport.
     ExecutionReport.editor_url_scheme = config["editor_url_scheme"]
     ExecutionReport.show_capture = config["show_capture"]
     ExecutionReport.show_locals = config["show_locals"]
 
 
 @hookimpl
@@ -117,14 +121,23 @@
     formatted_duration = _format_duration(duration)
     message = Text(
         f"{outcome.description} in {formatted_duration}", style=outcome.style
     )
     console.rule(message, style=outcome.style)
 
 
+@hookimpl
+def pytask_unconfigure() -> None:
+    """Reset class variables."""
+    Traceback._show_locals = False
+    ExecutionReport.editor_url_scheme = "file"
+    ExecutionReport.show_capture = ShowCapture.ALL
+    ExecutionReport.show_locals = False
+
+
 _TIME_UNITS: list[_TimeUnit] = [
     _TimeUnit(singular="day", plural="days", short="d", in_seconds=86400),
     _TimeUnit(singular="hour", plural="hours", short="h", in_seconds=3600),
     _TimeUnit(singular="minute", plural="minutes", short="m", in_seconds=60),
     _TimeUnit(singular="second", plural="seconds", short="s", in_seconds=1),
 ]
```

### Comparing `pytask-0.4.7/src/_pytask/mark/__init__.py` & `pytask-0.5.0/src/_pytask/mark/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 """Contains the main code for the markers plugin."""
+
 from __future__ import annotations
 
 import sys
+from typing import TYPE_CHECKING
 from typing import AbstractSet
 from typing import Any
-from typing import TYPE_CHECKING
 
 import click
+from attrs import define
+from rich.table import Table
+
 from _pytask.click import ColoredCommand
 from _pytask.console import console
 from _pytask.dag_utils import task_and_preceding_tasks
 from _pytask.exceptions import ConfigurationError
 from _pytask.mark.expression import Expression
 from _pytask.mark.expression import ParseError
-from _pytask.mark.structures import Mark
 from _pytask.mark.structures import MARK_GEN
+from _pytask.mark.structures import Mark
 from _pytask.mark.structures import MarkDecorator
 from _pytask.mark.structures import MarkGenerator
 from _pytask.outcomes import ExitCode
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.shared import parse_markers
-from attrs import define
-from rich.table import Table
-
 
 if TYPE_CHECKING:
-    from _pytask.node_protocols import PTask
-    import networkx as nx
     from typing import NoReturn
 
+    import networkx as nx
+
+    from _pytask.node_protocols import PTask
+
 
 __all__ = [
     "Expression",
     "MARK_GEN",
     "Mark",
     "MarkDecorator",
     "MarkGenerator",
     "ParseError",
     "select_by_after_keyword",
     "select_by_keyword",
     "select_by_mark",
+    "select_tasks_by_marks_and_expressions",
 ]
 
 
 @click.command(cls=ColoredCommand)
 def markers(**raw_config: Any) -> NoReturn:
     """Show all registered markers."""
     raw_config["command"] = "markers"
@@ -129,31 +133,29 @@
     _names: AbstractSet[str]
 
     @classmethod
     def from_task(cls, task: PTask) -> KeywordMatcher:
         mapped_names = {task.name}
 
         # Add the names attached to the current function through direct assignment.
-        function_obj = task.function
-        if function_obj:
-            mapped_names.update(function_obj.__dict__)
+        mapped_names.update(task.function.__dict__)
 
         # Add the markers to the keywords as we no longer handle them correctly.
         mapped_names.update(mark.name for mark in task.markers)
 
         return cls(mapped_names)
 
     def __call__(self, subname: str) -> bool:
         subname = subname.lower()
         names = (name.lower() for name in self._names)
 
         return any(subname in name for name in names)
 
 
-def select_by_keyword(session: Session, dag: nx.DiGraph) -> set[str]:
+def select_by_keyword(session: Session, dag: nx.DiGraph) -> set[str] | None:
     """Deselect tests by keywords."""
     keywordexpr = session.config["expression"]
     if not keywordexpr:
         return None
 
     try:
         expression = Expression.compile_(keywordexpr)
@@ -200,15 +202,15 @@
         mark_names = {mark.name for mark in task.markers}
         return cls(mark_names)
 
     def __call__(self, name: str) -> bool:
         return name in self.own_mark_names
 
 
-def select_by_mark(session: Session, dag: nx.DiGraph) -> set[str]:
+def select_by_mark(session: Session, dag: nx.DiGraph) -> set[str] | None:
     """Deselect tests by marks."""
     matchexpr = session.config["marker_expression"]
     if not matchexpr:
         return None
 
     try:
         expression = Expression.compile_(matchexpr)
@@ -229,16 +231,15 @@
 ) -> None:
     """Deselect tasks."""
     for task in session.tasks:
         if task.signature not in remaining:
             task.markers.append(mark)
 
 
-@hookimpl
-def pytask_dag_modify_dag(session: Session, dag: nx.DiGraph) -> None:
+def select_tasks_by_marks_and_expressions(session: Session, dag: nx.DiGraph) -> None:
     """Modify the tasks which are executed with expressions and markers."""
     remaining = select_by_keyword(session, dag)
     if remaining is not None:
         _deselect_others_with_mark(
             session, remaining, Mark("skip", (), {"reason": "Deselected by keyword."})
         )
     remaining = select_by_mark(session, dag)
```

### Comparing `pytask-0.4.7/src/_pytask/mark/expression.py` & `pytask-0.5.0/src/_pytask/mark/expression.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 The semantics are:
 
 - Empty expression evaluates to False.
 - ident evaluates to True of False according to a provided matcher function.
 - or/and/not evaluate according to the usual boolean semantics.
 
 """
+
 from __future__ import annotations
 
 import ast
 import enum
 import re
+from typing import TYPE_CHECKING
 from typing import Callable
 from typing import Iterator
 from typing import Mapping
 from typing import Sequence
-from typing import TYPE_CHECKING
 
 from attrs import define
 
-
 if TYPE_CHECKING:
     import types
     from typing import NoReturn
 
 
 __all__ = ["Expression", "ParseError"]
```

### Comparing `pytask-0.4.7/src/_pytask/mark/structures.py` & `pytask-0.5.0/src/_pytask/mark/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 import warnings
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Mapping
 
-from _pytask.mark_utils import get_all_marks
-from _pytask.models import CollectionMetadata
-from _pytask.typing import is_task_function
 from attrs import define
 from attrs import field
 from attrs import validators
 
+from _pytask.mark_utils import get_all_marks
+from _pytask.models import CollectionMetadata
+from _pytask.typing import is_task_function
+
 
 @define(frozen=True)
 class Mark:
     """A class for a mark containing the name, positional and keyword arguments."""
 
     name: str
     """str: Name of the mark."""
@@ -158,17 +159,17 @@
         obj.pytask_meta.markers = [*get_unpacked_marks(obj), mark]
     else:
         obj.pytask_meta = CollectionMetadata(  # type: ignore[attr-defined]
             markers=[mark]
         )
 
 
-_DEPRECATION_DECORATOR = """'@pytask.mark.{}' is deprecated starting pytask \
-v0.4.0 and will be removed in v0.5.0. To upgrade your project to the new syntax, read \
-the tutorial on product and dependencies: https://tinyurl.com/pytask-deps-prods.
+_DEPRECATION_DECORATOR = """'@pytask.mark.{}' was removed in pytask v0.5.0. To upgrade \
+your project to the new syntax, read the tutorial on product and dependencies: \
+https://tinyurl.com/pytask-deps-prods.
 """
 
 
 class MarkGenerator:
     """Factory for :class:`MarkDecorator` objects.
 
     Exposed as a :class:`pytask.mark` singleton instance.
@@ -190,19 +191,22 @@
 
     def __getattr__(self, name: str) -> MarkDecorator | Any:
         if name[0] == "_":
             msg = "Marker name must NOT start with underscore"
             raise AttributeError(msg)
 
         if name in ("depends_on", "produces"):
-            warnings.warn(
-                _DEPRECATION_DECORATOR.format(name),
-                category=FutureWarning,
-                stacklevel=1,
+            raise RuntimeError(_DEPRECATION_DECORATOR.format(name))
+
+        if name == "task":
+            msg = (
+                "'@pytask.mark.task' is removed. Use '@task' with 'from pytask import "
+                "task' instead."
             )
+            raise RuntimeError(msg)
 
         # If the name is not in the set of known marks after updating,
         # then it really is time to issue a warning or an error.
         if self.config is not None and name not in self.config["markers"]:
             if name in ("parametrize", "parameterize", "parametrise", "parameterise"):
                 msg = (
                     "@pytask.mark.parametrize has been removed since pytask v0.4. "
@@ -217,24 +221,11 @@
 
             warnings.warn(
                 f"Unknown pytask.mark.{name} - is this a typo? You can register "
                 "custom marks to avoid this warning.",
                 stacklevel=2,
             )
 
-        if name == "task":
-            from _pytask.task_utils import task
-
-            warnings.warn(
-                "'@pytask.mark.task' is deprecated starting pytask v0.4.0 and will be "
-                "removed in v0.5.0. Use '@task' with 'from pytask import task' "
-                "instead.",
-                category=FutureWarning,
-                stacklevel=1,
-            )
-
-            return task
-
         return MarkDecorator(Mark(name, (), {}))
 
 
 MARK_GEN = MarkGenerator()
```

### Comparing `pytask-0.4.7/src/_pytask/mark_utils.py` & `pytask-0.5.0/src/_pytask/mark_utils.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Contains utility functions related to marker.
 
 The utility functions are stored here to be separate from the plugin.
 
 """
+
 from __future__ import annotations
 
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 from _pytask.models import CollectionMetadata
 from _pytask.node_protocols import PTask
 
-
 if TYPE_CHECKING:
     from _pytask.mark import Mark
 
 
 def get_all_marks(obj_or_task: Any | PTask) -> list[Mark]:
     """Get all marks from a callable or task."""
     if isinstance(obj_or_task, PTask):
```

### Comparing `pytask-0.4.7/src/_pytask/nodes.py` & `pytask-0.5.0/src/_pytask/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 """Contains implementations of tasks and nodes following the node protocols."""
+
 from __future__ import annotations
 
 import hashlib
 import inspect
 import pickle
+from contextlib import suppress
 from os import stat_result
 from pathlib import Path  # noqa: TCH003
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
-from typing import TYPE_CHECKING
+
+from attrs import define
+from attrs import field
+from upath import UPath
+from upath._stat import UPathStatResult
 
 from _pytask._hashlib import hash_value
 from _pytask.node_protocols import PNode
 from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
 from _pytask.node_protocols import PTaskWithPath
 from _pytask.path import hash_path
-from _pytask.typing import no_default
 from _pytask.typing import NoDefault
-from attrs import define
-from attrs import field
-
+from _pytask.typing import no_default
 
 if TYPE_CHECKING:
+    from _pytask.mark import Mark
     from _pytask.models import NodeInfo
     from _pytask.tree_util import PyTree
-    from _pytask.mark import Mark
 
 
-__all__ = ["PathNode", "PickleNode", "PythonNode", "Task", "TaskWithoutPath"]
+__all__ = [
+    "DirectoryNode",
+    "PathNode",
+    "PickleNode",
+    "PythonNode",
+    "Task",
+    "TaskWithoutPath",
+]
 
 
 @define(kw_only=True)
 class TaskWithoutPath(PTask):
     """The class for tasks without a source file.
 
     Tasks may have no source file because
@@ -56,35 +68,33 @@
     attributes: dict[Any, Any]
         A dictionary to store additional information of the task.
 
     """
 
     name: str
     function: Callable[..., Any]
-    depends_on: dict[str, PyTree[PNode]] = field(factory=dict)
-    produces: dict[str, PyTree[PNode]] = field(factory=dict)
+    depends_on: dict[str, PyTree[PNode | PProvisionalNode]] = field(factory=dict)
+    produces: dict[str, PyTree[PNode | PProvisionalNode]] = field(factory=dict)
     markers: list[Mark] = field(factory=list)
     report_sections: list[tuple[str, str, str]] = field(factory=list)
     attributes: dict[Any, Any] = field(factory=dict)
 
     @property
     def signature(self) -> str:
         raw_key = str(hash_value(self.name))
         return hashlib.sha256(raw_key.encode()).hexdigest()
 
     def state(self) -> str | None:
         """Return the state of the node."""
-        try:
+        with suppress(OSError):
             source = inspect.getsource(self.function)
-        except OSError:
-            return None
-        else:
             return hashlib.sha256(source.encode()).hexdigest()
+        return None
 
-    def execute(self, **kwargs: Any) -> None:
+    def execute(self, **kwargs: Any) -> Any:
         """Execute the task."""
         return self.function(**kwargs)
 
 
 @define(kw_only=True)
 class Task(PTaskWithPath):
     """The class for tasks which are Python functions.
@@ -112,16 +122,16 @@
 
     """
 
     base_name: str
     path: Path
     function: Callable[..., Any]
     name: str = field(default="", init=False)
-    depends_on: dict[str, PyTree[PNode]] = field(factory=dict)
-    produces: dict[str, PyTree[PNode]] = field(factory=dict)
+    depends_on: dict[str, PyTree[PNode | PProvisionalNode]] = field(factory=dict)
+    produces: dict[str, PyTree[PNode | PProvisionalNode]] = field(factory=dict)
     markers: list[Mark] = field(factory=list)
     report_sections: list[tuple[str, str, str]] = field(factory=list)
     attributes: dict[Any, Any] = field(factory=dict)
 
     def __attrs_post_init__(self: Task) -> None:
         """Change class after initialization."""
         if not self.name:
@@ -131,20 +141,17 @@
     def signature(self) -> str:
         """The unique signature of the node."""
         raw_key = "".join(str(hash_value(arg)) for arg in (self.base_name, self.path))
         return hashlib.sha256(raw_key.encode()).hexdigest()
 
     def state(self) -> str | None:
         """Return the state of the node."""
-        if self.path.exists():
-            modification_time = self.path.stat().st_mtime
-            return hash_path(self.path, modification_time)
-        return None
+        return _get_state(self.path)
 
-    def execute(self, **kwargs: Any) -> None:
+    def execute(self, **kwargs: Any) -> Any:
         """Execute the task."""
         return self.function(**kwargs)
 
 
 @define(kw_only=True)
 class PathNode(PPathNode):
     """The class for a node which is a path.
@@ -174,24 +181,15 @@
 
     def state(self) -> str | None:
         """Calculate the state of the node.
 
         The state is given by the modification timestamp.
 
         """
-        if self.path.exists():
-            stat = self.path.stat()
-            if isinstance(stat, stat_result):
-                modification_time = self.path.stat().st_mtime
-                return hash_path(self.path, modification_time)
-            if isinstance(stat, dict):
-                return stat.get("ETag", "0")
-            msg = "Unknown stat object."
-            raise NotImplementedError(msg)
-        return None
+        return _get_state(self.path)
 
     def load(self, is_product: bool = False) -> Path:  # noqa: ARG002
         """Load the value."""
         return self.path
 
     def save(self, value: bytes | str) -> None:
         """Save strings or bytes to file."""
@@ -224,23 +222,24 @@
 
     Examples
     --------
     To allow a :class:`PythonNode` to hash a dictionary, you need to pass your
     own hashing function. For example, from the :mod:`deepdiff` library.
 
     >>> from deepdiff import DeepHash
+    >>> from pytask import PythonNode
     >>> node = PythonNode(name="node", value={"a": 1}, hash=lambda x: DeepHash(x)[x])
 
     .. warning:: Hashing big objects can require some time.
 
     """
 
     name: str = ""
     value: Any | NoDefault = no_default
-    hash: bool | Callable[[Any], bool] = False  # noqa: A003
+    hash: bool | Callable[[Any], bool] = False
     node_info: NodeInfo | None = None
 
     @property
     def signature(self) -> str:
         """The unique signature of the node."""
         raw_key = (
             "".join(
@@ -278,14 +277,16 @@
 
         The hash for strings and bytes is calculated using hashlib because
         ``hash("asd")`` returns a different value every invocation since the hash of
         strings is salted with a random integer and it would confuse users. See
         {meth}`object.__hash__` for more information.
 
         """
+        if self.value is no_default:
+            return None
         if self.hash:
             value = self.load()
             if callable(self.hash):
                 return str(self.hash(value))
             return str(hash_value(value))
         return "0"
 
@@ -317,27 +318,83 @@
         """Instantiate class from path to file."""
         if not path.is_absolute():
             msg = "Node must be instantiated from absolute path."
             raise ValueError(msg)
         return cls(name=path.as_posix(), path=path)
 
     def state(self) -> str | None:
-        if self.path.exists():
-            stat = self.path.stat()
-            if isinstance(stat, stat_result):
-                modification_time = self.path.stat().st_mtime
-                return hash_path(self.path, modification_time)
-            if isinstance(stat, dict):
-                return stat.get("ETag", "0")
-            msg = "Unknown stat object."
-            raise NotImplementedError(msg)
-        return None
+        return _get_state(self.path)
 
     def load(self, is_product: bool = False) -> Any:
         if is_product:
             return self
         with self.path.open("rb") as f:
             return pickle.load(f)  # noqa: S301
 
     def save(self, value: Any) -> None:
         with self.path.open("wb") as f:
             pickle.dump(value, f)
+
+
+@define(kw_only=True)
+class DirectoryNode(PProvisionalNode):
+    """The class for a provisional node that works with directories.
+
+    Attributes
+    ----------
+    name
+        The name of the node.
+    pattern
+        Patterns are the same as for :mod:`fnmatch`, with the addition of ``**`` which
+        means "this directory and all subdirectories, recursively".
+    root_dir
+        The pattern is interpreted relative to the path given by ``root_dir``. If
+        ``root_dir = None``, it is the directory where the path is defined.
+
+    """
+
+    name: str = ""
+    pattern: str = "*"
+    root_dir: Path | None = None
+
+    @property
+    def signature(self) -> str:
+        """The unique signature of the node."""
+        raw_key = "".join(str(hash_value(arg)) for arg in (self.root_dir, self.pattern))
+        return hashlib.sha256(raw_key.encode()).hexdigest()
+
+    def load(self, is_product: bool = False) -> Path:
+        """Inject a path into the task when loaded as a product."""
+        if is_product:
+            return self.root_dir  # type: ignore[return-value]
+        msg = "'DirectoryNode' cannot be loaded as a dependency"  # pragma: no cover
+        raise NotImplementedError(msg)  # pragma: no cover
+
+    def collect(self) -> list[Path]:
+        """Collect paths defined by the pattern."""
+        return list(self.root_dir.glob(self.pattern))  # type: ignore[union-attr]
+
+
+def _get_state(path: Path) -> str | None:
+    """Get state of a path.
+
+    A simple function to handle local and remote files.
+
+    """
+    # Invalidate the cache of the path if it is a UPath because it might have changed in
+    # a different process with pytask-parallel and the main process does not know about
+    # it and relies on the cache.
+    if isinstance(path, UPath):
+        path.fs.invalidate_cache()
+
+    try:
+        stat = path.stat()
+    except FileNotFoundError:
+        return None
+
+    if isinstance(stat, stat_result):
+        modification_time = stat.st_mtime
+        return hash_path(path, modification_time)
+    if isinstance(stat, UPathStatResult):
+        return stat.as_info().get("ETag", "0")
+    msg = "Unknown stat object."
+    raise NotImplementedError(msg)
```

### Comparing `pytask-0.4.7/src/_pytask/outcomes.py` & `pytask-0.5.0/src/_pytask/outcomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Contains code related to outcomes."""
+
 from __future__ import annotations
 
-from enum import auto
 from enum import Enum
 from enum import IntEnum
-from typing import Sequence
+from enum import auto
 from typing import TYPE_CHECKING
-
+from typing import Sequence
 
 if TYPE_CHECKING:
     from _pytask.reports import CollectionReport
     from _pytask.reports import ExecutionReport
 
 
 __all__ = [
@@ -170,15 +170,15 @@
     reports: Sequence[CollectionReport | ExecutionReport],
     outcome_enum: type[CollectionOutcome | TaskOutcome],
 ) -> dict[Enum, int]:
     """Count how often an outcome occurred.
 
     Examples
     --------
-    >>> from _pytask.outcomes import CollectionOutcome, TaskOutcome
+    >>> from _pytask.outcomes import CollectionOutcome, TaskOutcome, count_outcomes
     >>> count_outcomes([], CollectionOutcome)
     {<CollectionOutcome.SUCCESS: 1>: 0, <CollectionOutcome.FAIL: 2>: 0}
 
     """
     return {
         outcome: len([r for r in reports if r.outcome == outcome])
         for outcome in outcome_enum
```

### Comparing `pytask-0.4.7/src/_pytask/parameters.py` & `pytask-0.5.0/src/_pytask/parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Contains common parameters for the commands of the command line interface."""
+
 from __future__ import annotations
 
 import importlib.util
 from pathlib import Path
-from typing import Iterable
 from typing import TYPE_CHECKING
+from typing import Iterable
 
 import click
+from click import Context
+from sqlalchemy.engine import URL
+from sqlalchemy.engine import make_url
+from sqlalchemy.exc import ArgumentError
+
 from _pytask.config_utils import set_defaults_from_config
 from _pytask.path import import_path
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import register_hook_impls_from_modules
 from _pytask.pluginmanager import storage
-from click import Context
-from sqlalchemy.engine import make_url
-from sqlalchemy.engine import URL
-from sqlalchemy.exc import ArgumentError
 
 if TYPE_CHECKING:
     from pluggy import PluginManager
 
 
 _CONFIG_OPTION = click.Option(
     ["-c", "--config"],
@@ -52,15 +54,15 @@
 )
 """click.Option: An option for the --ignore flag."""
 
 
 _PATH_ARGUMENT = click.Argument(
     ["paths"],
     nargs=-1,
-    type=click.Path(exists=True, resolve_path=True),
+    type=click.Path(exists=True, resolve_path=True, path_type=Path),
     is_eager=True,
 )
 """click.Argument: An argument for paths."""
 
 
 _VERBOSE_OPTION = click.Option(
     ["-v", "--verbose"],
@@ -176,14 +178,16 @@
 )
 
 
 @hookimpl(trylast=True)
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Register general markers."""
     for command in ("build", "clean", "collect", "dag", "profile"):
-        cli.commands[command].params.extend((_PATH_ARGUMENT, _DATABASE_URL_OPTION))
+        cli.commands[command].params.extend((_DATABASE_URL_OPTION,))
     for command in ("build", "clean", "collect", "dag", "markers", "profile"):
-        cli.commands[command].params.extend((_CONFIG_OPTION, _HOOK_MODULE_OPTION))
+        cli.commands[command].params.extend(
+            (_CONFIG_OPTION, _HOOK_MODULE_OPTION, _PATH_ARGUMENT)
+        )
     for command in ("build", "clean", "collect", "profile"):
         cli.commands[command].params.extend([_IGNORE_OPTION, _EDITOR_URL_SCHEME_OPTION])
     for command in ("build",):
         cli.commands[command].params.append(_VERBOSE_OPTION)
```

### Comparing `pytask-0.4.7/src/_pytask/persist.py` & `pytask-0.5.0/src/_pytask/persist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Implement the ability for tasks to persist."""
+
 from __future__ import annotations
 
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 from _pytask.dag_utils import node_and_neighbors
 from _pytask.database_utils import has_node_changed
 from _pytask.database_utils import update_states_in_database
 from _pytask.mark_utils import has_mark
 from _pytask.outcomes import Persisted
 from _pytask.outcomes import TaskOutcome
 from _pytask.pluginmanager import hookimpl
-
+from _pytask.provisional_utils import collect_provisional_products
 
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
-    from _pytask.session import Session
     from _pytask.reports import ExecutionReport
+    from _pytask.session import Session
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Add the marker to the configuration."""
     config["markers"]["persist"] = (
         "Prevent execution of a task if all products exist and even if something has "
@@ -35,31 +36,36 @@
 def pytask_execute_task_setup(session: Session, task: PTask) -> None:
     """Exit persisting tasks early.
 
     The decorator needs to be set and all nodes need to exist.
 
     """
     if has_mark(task, "persist"):
-        all_nodes_exist = all(
+        all_states = [
             (
                 session.dag.nodes[name].get("task") or session.dag.nodes[name]["node"]
             ).state()
             for name in node_and_neighbors(session.dag, task.signature)
-        )
+        ]
+        all_nodes_exist = all(all_states)
 
         if all_nodes_exist:
             any_node_changed = any(
                 has_node_changed(
                     task=task,
                     node=session.dag.nodes[name].get("task")
                     or session.dag.nodes[name]["node"],
+                    state=state,
+                )
+                for name, state in zip(
+                    node_and_neighbors(session.dag, task.signature), all_states
                 )
-                for name in node_and_neighbors(session.dag, task.signature)
             )
             if any_node_changed:
+                collect_provisional_products(session, task)
                 raise Persisted
 
 
 @hookimpl
 def pytask_execute_task_process_report(
     session: Session, report: ExecutionReport
 ) -> bool | None:
```

### Comparing `pytask-0.4.7/src/_pytask/pluginmanager.py` & `pytask-0.5.0/src/_pytask/pluginmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Contains the plugin manager."""
+
 from __future__ import annotations
 
 import importlib
 import sys
 from typing import Iterable
 
-from _pytask import hookspecs
 from attrs import define
 from pluggy import HookimplMarker
 from pluggy import PluginManager
 
+from _pytask import hookspecs
 
 __all__ = [
     "get_plugin_manager",
     "hookimpl",
     "register_hook_impls_from_modules",
     "storage",
 ]
@@ -41,14 +42,15 @@
         "_pytask.collect",
         "_pytask.collect_command",
         "_pytask.config",
         "_pytask.dag",
         "_pytask.dag_command",
         "_pytask.database",
         "_pytask.debugging",
+        "_pytask.provisional",
         "_pytask.execute",
         "_pytask.live",
         "_pytask.logging",
         "_pytask.mark",
         "_pytask.nodes",
         "_pytask.parameters",
         "_pytask.persist",
```

### Comparing `pytask-0.4.7/src/_pytask/profile.py` & `pytask-0.5.0/src/_pytask/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 """Contains the code to profile the execution."""
+
 from __future__ import annotations
 
 import csv
 import enum
 import json
 import sys
 import time
 from contextlib import suppress
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
-from typing import TYPE_CHECKING
 
 import click
+from rich.table import Table
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+
 from _pytask.click import ColoredCommand
 from _pytask.click import EnumChoice
 from _pytask.console import console
 from _pytask.console import format_task_name
+from _pytask.dag import create_dag
 from _pytask.database_utils import BaseTable
 from _pytask.database_utils import DatabaseSession
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.node_protocols import PPathNode
 from _pytask.node_protocols import PTask
 from _pytask.outcomes import ExitCode
 from _pytask.outcomes import TaskOutcome
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.session import Session
 from _pytask.traceback import Traceback
-from rich.table import Table
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
 
 if TYPE_CHECKING:
-    from _pytask.reports import ExecutionReport
     from pathlib import Path
     from typing import NoReturn
 
+    from _pytask.reports import ExecutionReport
+
 
 class _ExportFormats(enum.Enum):
     NO = "no"
     JSON = "json"
     CSV = "csv"
 
 
@@ -64,21 +68,22 @@
 def pytask_post_parse(config: dict[str, Any]) -> None:
     """Register the export option."""
     config["pm"].register(ExportNameSpace)
     config["pm"].register(DurationNameSpace)
     config["pm"].register(FileSizeNameSpace)
 
 
-@hookimpl(hookwrapper=True)
+@hookimpl(wrapper=True)
 def pytask_execute_task(task: PTask) -> Generator[None, None, None]:
     """Attach the duration of the execution to the task."""
     start = time.time()
-    yield
+    result = yield
     end = time.time()
     task.attributes["duration"] = (start, end)
+    return result
 
 
 @hookimpl
 def pytask_execute_task_process_report(report: ExecutionReport) -> None:
     """Store runtime of successfully finishing tasks in database."""
     task = report.task
     duration = task.attributes.get("duration")
@@ -120,15 +125,15 @@
         session = Session(exit_code=ExitCode.CONFIGURATION_FAILED)
         console.print(Traceback(sys.exc_info()))
 
     else:
         try:
             session.hook.pytask_log_session_header(session=session)
             session.hook.pytask_collect(session=session)
-            session.hook.pytask_dag(session=session)
+            session.dag = create_dag(session=session)
 
             profile: dict[str, dict[str, Any]] = {
                 task.name: {} for task in session.tasks
             }
             session.hook.pytask_profile_add_info_on_task(
                 session=session, tasks=session.tasks, profile=profile
             )
```

### Comparing `pytask-0.4.7/src/_pytask/reports.py` & `pytask-0.5.0/src/_pytask/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """Contains everything related to reports."""
+
 from __future__ import annotations
 
-from typing import ClassVar
 from typing import TYPE_CHECKING
+from typing import ClassVar
+
+from attrs import define
+from attrs import field
+from rich.rule import Rule
+from rich.text import Text
 
 from _pytask.capture_utils import ShowCapture
 from _pytask.console import format_task_name
 from _pytask.outcomes import CollectionOutcome
 from _pytask.outcomes import TaskOutcome
 from _pytask.traceback import OptionalExceptionInfo
 from _pytask.traceback import Traceback
-from attrs import define
-from attrs import field
-from rich.rule import Rule
-from rich.text import Text
-
 
 if TYPE_CHECKING:
-    from _pytask.node_protocols import PNode
-    from _pytask.node_protocols import PTask
     from rich.console import Console
-    from rich.console import RenderResult
     from rich.console import ConsoleOptions
+    from rich.console import RenderResult
+
+    from _pytask.node_protocols import PNode
+    from _pytask.node_protocols import PProvisionalNode
+    from _pytask.node_protocols import PTask
 
 
 @define
 class CollectionReport:
     """A collection report for a task."""
 
     outcome: CollectionOutcome
-    node: PTask | PNode | None = None
+    node: PTask | PNode | PProvisionalNode | None = None
     exc_info: OptionalExceptionInfo | None = None
 
     @classmethod
     def from_exception(
         cls: type[CollectionReport],
         outcome: CollectionOutcome,
         exc_info: OptionalExceptionInfo,
-        node: PTask | PNode | None = None,
+        node: PTask | PNode | PProvisionalNode | None = None,
     ) -> CollectionReport:
         return cls(outcome=outcome, node=node, exc_info=exc_info)
 
     def __rich_console__(
         self, console: Console, console_options: ConsoleOptions
     ) -> RenderResult:
         header = "Error" if self.node is None else f"Could not collect {self.node.name}"
```

### Comparing `pytask-0.4.7/src/_pytask/session.py` & `pytask-0.5.0/src/_pytask/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Contains code related to the session object."""
+
 from __future__ import annotations
 
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 import networkx as nx
-from _pytask.outcomes import ExitCode
 from attrs import define
 from attrs import field
+from pluggy import HookRelay
 
-# HookRelay was published in v1.3.
-try:
-    from pluggy import HookRelay
-except ImportError:
-    from pluggy._hooks import _HookRelay as HookRelay
+from _pytask.outcomes import ExitCode
 
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
-    from _pytask.warnings_utils import WarningReport
     from _pytask.reports import CollectionReport
-    from _pytask.reports import ExecutionReport
     from _pytask.reports import DagReport
+    from _pytask.reports import ExecutionReport
+    from _pytask.warnings_utils import WarningReport
 
 
 @define(kw_only=True)
 class Session:
     """The session of pytask.
 
     Parameters
```

### Comparing `pytask-0.4.7/src/_pytask/shared.py` & `pytask-0.5.0/src/_pytask/shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 """Functions which are used across various modules."""
+
 from __future__ import annotations
 
 import glob
-import warnings
+import inspect
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
+from typing import Callable
 from typing import Iterable
 from typing import Sequence
-from typing import TYPE_CHECKING
 
 import click
+
+from _pytask.coiled_utils import Function
 from _pytask.console import format_node_name
 from _pytask.console import format_task_name
 from _pytask.node_protocols import PNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
 
 if TYPE_CHECKING:
     from enum import Enum
+
     import networkx as nx
 
 
 __all__ = [
     "convert_to_enum",
     "find_duplicates",
     "parse_markers",
     "parse_paths",
     "reduce_names_of_multiple_nodes",
     "to_list",
+    "unwrap_task_function",
 ]
 
 
 def to_list(scalar_or_iter: Any) -> list[Any]:
     """Convert scalars and iterables to list.
 
     Parameters
@@ -52,28 +59,16 @@
     return (
         [scalar_or_iter]
         if isinstance(scalar_or_iter, str) or not isinstance(scalar_or_iter, Sequence)
         else list(scalar_or_iter)
     )
 
 
-def parse_paths(x: Any | None) -> list[Path] | None:
+def parse_paths(x: Path | list[Path]) -> list[Path]:
     """Parse paths."""
-    if x is None:
-        return None
-
-    if isinstance(x, str):
-        msg = (
-            "Specifying paths as a string in 'pyproject.toml' is deprecated and will "
-            "result in an error in v0.5. Please use a list of strings instead: "
-            f'["{x}"].'
-        )
-        warnings.warn(msg, category=FutureWarning, stacklevel=1)
-        x = [x]
-
     paths = [Path(p) for p in to_list(x)]
     for p in paths:
         if not p.exists():
             msg = f"The path '{p}' does not exist."
             raise FileNotFoundError(msg)
 
     return [
@@ -89,18 +84,21 @@
     """Reduce the names of multiple nodes in the DAG."""
     short_names = []
     for name in names:
         node = dag.nodes[name].get("node") or dag.nodes[name].get("task")
 
         if isinstance(node, PTask):
             short_name = format_task_name(node, editor_url_scheme="no_link").plain
-        elif isinstance(node, PNode):
+        elif isinstance(node, (PNode, PProvisionalNode)):
             short_name = format_node_name(node, paths).plain
         else:
-            msg = f"Requires a 'PTask' or a 'PNode' and not {type(node)!r}."
+            msg = (
+                "Requires a 'PTask', 'PNode', or 'PProvisionalNode' and not "
+                f"{type(node)!r}."
+            )
             raise TypeError(msg)
 
         short_names.append(short_name)
 
     return short_names
 
 
@@ -148,7 +146,17 @@
     """Convert value to enum."""
     try:
         return enum(value)
     except ValueError:
         values = [e.value for e in enum]
         msg = f"Value {value!r} is not a valid {enum!r}. Valid values are {values}."
         raise ValueError(msg) from None
+
+
+def unwrap_task_function(obj: Any) -> Callable[..., Any]:
+    """Unwrap a task function.
+
+    Get the underlying function to avoid having different states of the function, e.g.
+    due to pytask_meta, in different layers of the wrapping.
+
+    """
+    return inspect.unwrap(obj, stop=lambda x: isinstance(x, Function))
```

### Comparing `pytask-0.4.7/src/_pytask/skipping.py` & `pytask-0.5.0/src/_pytask/skipping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Contains everything related to skipping tasks."""
+
 from __future__ import annotations
 
-from typing import Any
 from typing import TYPE_CHECKING
+from typing import Any
 
 from _pytask.dag_utils import descending_tasks
 from _pytask.mark import Mark
 from _pytask.mark_utils import get_marks
 from _pytask.mark_utils import has_mark
 from _pytask.outcomes import Skipped
 from _pytask.outcomes import SkippedAncestorFailed
 from _pytask.outcomes import SkippedUnchanged
 from _pytask.outcomes import TaskOutcome
 from _pytask.pluginmanager import hookimpl
-
+from _pytask.provisional_utils import collect_provisional_products
 
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
-    from _pytask.session import Session
     from _pytask.reports import ExecutionReport
+    from _pytask.session import Session
 
 
 def skip_ancestor_failed(reason: str = "No reason provided.") -> str:
     """Parse information in ``@pytask.mark.skip_ancestor_failed``."""
     return reason
 
 
@@ -48,14 +49,15 @@
 @hookimpl
 def pytask_execute_task_setup(session: Session, task: PTask) -> None:
     """Take a short-cut for skipped tasks during setup with an exception."""
     is_unchanged = has_mark(task, "skip_unchanged") and not has_mark(
         task, "would_be_executed"
     )
     if is_unchanged and not session.config["force"]:
+        collect_provisional_products(session, task)
         raise SkippedUnchanged
 
     is_skipped = has_mark(task, "skip")
     if is_skipped:
         raise Skipped
 
     skipif_marks = get_marks(task, "skipif")
@@ -85,29 +87,28 @@
 
     """
     task = report.task
 
     if report.exc_info:
         if isinstance(report.exc_info[1], SkippedUnchanged):
             report.outcome = TaskOutcome.SKIP_UNCHANGED
+            return True
 
-        elif isinstance(report.exc_info[1], Skipped):
+        if isinstance(report.exc_info[1], Skipped):
             report.outcome = TaskOutcome.SKIP
 
             for descending_task_name in descending_tasks(task.signature, session.dag):
                 descending_task = session.dag.nodes[descending_task_name]["task"]
                 descending_task.markers.append(
                     Mark(
                         "skip",
                         (),
                         {"reason": f"Previous task {task.name!r} was skipped."},
                     )
                 )
+            return True
 
-        elif isinstance(report.exc_info[1], SkippedAncestorFailed):
+        if isinstance(report.exc_info[1], SkippedAncestorFailed):
             report.outcome = TaskOutcome.SKIP_PREVIOUS_FAILED
+            return True
 
-    if report.exc_info and isinstance(
-        report.exc_info[1], (Skipped, SkippedUnchanged, SkippedAncestorFailed)
-    ):
-        return True
     return None
```

### Comparing `pytask-0.4.7/src/_pytask/task.py` & `pytask-0.5.0/src/_pytask/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-"""Contain hooks related to the ``@pytask.mark.task`` decorator."""
+"""Contain hooks related to the :func:`@task <pytask.task>`."""
+
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
-from typing import TYPE_CHECKING
 
 from _pytask.console import format_strings_as_flat_tree
 from _pytask.pluginmanager import hookimpl
 from _pytask.shared import find_duplicates
 from _pytask.task_utils import COLLECTED_TASKS
 from _pytask.task_utils import parse_collected_tasks_with_task_marker
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from _pytask.reports import CollectionReport
     from _pytask.session import Session
-    from pathlib import Path
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Parse the configuration."""
     config["markers"]["task"] = (
         "Mark a function as a task regardless of its name. Or mark tasks which are "
@@ -76,7 +78,12 @@
     msg = (
         "There are some duplicates among the repeated tasks. It happens when you define"
         "the task function outside the loop body and merely wrap in the loop body with "
         "the 'task(...)(func)' decorator. As a workaround, wrap the task function in "
         f"a lambda expression like 'task(...)(lambda **x: func(**x))'.\n\n{flat_tree}"
     )
     raise ValueError(msg)
+
+
+@hookimpl
+def pytask_unconfigure() -> None:
+    COLLECTED_TASKS.clear()
```

### Comparing `pytask-0.4.7/src/_pytask/task_utils.py` & `pytask-0.5.0/src/_pytask/task_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-"""Contains utilities related to the ``@pytask.mark.task`` decorator."""
+"""Contains utilities related to the :func:`@task <pytask.task>`."""
+
 from __future__ import annotations
 
 import functools
 import inspect
 from collections import defaultdict
 from types import BuiltinFunctionType
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
-from typing import TYPE_CHECKING
 
 import attrs
+
+from _pytask.coiled_utils import Function
+from _pytask.coiled_utils import extract_coiled_function_kwargs
 from _pytask.console import get_file
 from _pytask.mark import Mark
 from _pytask.models import CollectionMetadata
 from _pytask.shared import find_duplicates
+from _pytask.shared import unwrap_task_function
 from _pytask.typing import is_task_function
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 __all__ = [
@@ -27,25 +32,26 @@
     "task",
 ]
 
 
 COLLECTED_TASKS: dict[Path | None, list[Callable[..., Any]]] = defaultdict(list)
 """A container for collecting tasks.
 
-Tasks marked by the ``@pytask.mark.task`` decorator can be generated in a loop where one
-iteration overwrites the previous task. To retrieve the tasks later, use this dictionary
-mapping from paths of modules to a list of tasks per module.
+Tasks marked by the :func:`@task <pytask.task>` decorator can be generated in a loop
+where one iteration overwrites the previous task. To retrieve the tasks later, use this
+dictionary mapping from paths of modules to a list of tasks per module.
 
 """
 
 
-def task(
+def task(  # noqa: PLR0913
     name: str | None = None,
     *,
     after: str | Callable[..., Any] | list[Callable[..., Any]] | None = None,
+    is_generator: bool = False,
     id: str | None = None,  # noqa: A002
     kwargs: dict[Any, Any] | None = None,
     produces: Any | None = None,
 ) -> Callable[..., Callable[..., Any]]:
     """Decorate a task function.
 
     This decorator declares every callable as a pytask task.
@@ -58,14 +64,27 @@
     name
         Use it to override the name of the task that is, by default, the name of the
         task function. Read :ref:`customize-task-names` for more information.
     after
         An expression or a task function or a list of task functions that need to be
         executed before this task can be executed. See :ref:`after` for more
         information.
+    is_generator
+        An indicator whether this task is a task generator.
+    id
+        An id for the task if it is part of a parametrization. Otherwise, an automatic
+        id will be generated. See
+        :doc:`this tutorial <../tutorials/repeating_tasks_with_different_inputs>` for
+        more information.
+    kwargs
+        A dictionary containing keyword arguments which are passed to the task when it
+        is executed.
+    produces
+        Definition of products to parse the function returns and store them. See
+        :doc:`this how-to guide <../how_to_guides/using_task_returns>` for more
     id
         An id for the task if it is part of a repetition. Otherwise, an automatic id
         will be generated. See :ref:`how-to-repeat-a-task-with-different-inputs-the-id`
         for more information.
     kwargs
         Use a dictionary to pass any keyword arguments to the task function which can be
         dependencies or products of the task. Read :ref:`task-kwargs` for more
@@ -80,32 +99,37 @@
     --------
     To mark a function without the ``task_`` prefix as a task, attach the decorator.
 
     .. code-block:: python
 
         from typing import Annotated from pytask import task
 
-        @task def create_text_file() -> Annotated[str, Path("file.txt")]:
+        @task()
+        def create_text_file() -> Annotated[str, Path("file.txt")]:
             return "Hello, World!"
 
     """
 
     def wrapper(func: Callable[..., Any]) -> Callable[..., Any]:
         # Omits frame when a builtin function is wrapped.
         _rich_traceback_omit = True
 
         for arg, arg_name in ((name, "name"), (id, "id")):
             if not (isinstance(arg, str) or arg is None):
                 msg = (
-                    f"Argument {arg_name!r} of @pytask.mark.task must be a str, but it "
-                    f"is {arg!r}."
+                    f"Argument {arg_name!r} of @task must be a str, but it is {arg!r}."
                 )
                 raise ValueError(msg)
 
-        unwrapped = inspect.unwrap(func)
+        unwrapped = unwrap_task_function(func)
+        if isinstance(unwrapped, Function):
+            coiled_kwargs = extract_coiled_function_kwargs(unwrapped)
+            unwrapped = unwrap_task_function(unwrapped.function)
+        else:
+            coiled_kwargs = None
 
         # We do not allow builtins as functions because we would need to use
         # ``inspect.stack`` to infer their caller location and they are unable to carry
         # the pytask metadata.
         if isinstance(unwrapped, BuiltinFunctionType):
             msg = (
                 "Builtin functions cannot be wrapped with '@task'. If necessary, wrap "
@@ -116,30 +140,36 @@
         path = get_file(unwrapped)
 
         parsed_kwargs = {} if kwargs is None else kwargs
         parsed_name = _parse_name(unwrapped, name)
         parsed_after = _parse_after(after)
 
         if hasattr(unwrapped, "pytask_meta"):
-            unwrapped.pytask_meta.name = parsed_name
+            unwrapped.pytask_meta.after = parsed_after
+            unwrapped.pytask_meta.is_generator = is_generator
+            unwrapped.pytask_meta.id_ = id
             unwrapped.pytask_meta.kwargs = parsed_kwargs
             unwrapped.pytask_meta.markers.append(Mark("task", (), {}))
-            unwrapped.pytask_meta.id_ = id
+            unwrapped.pytask_meta.name = parsed_name
             unwrapped.pytask_meta.produces = produces
             unwrapped.pytask_meta.after = parsed_after
         else:
-            unwrapped.pytask_meta = CollectionMetadata(
-                name=parsed_name,
+            unwrapped.pytask_meta = CollectionMetadata(  # type: ignore[attr-defined]
+                after=parsed_after,
+                is_generator=is_generator,
+                id_=id,
                 kwargs=parsed_kwargs,
                 markers=[Mark("task", (), {})],
-                id_=id,
+                name=parsed_name,
                 produces=produces,
-                after=parsed_after,
             )
 
+        if coiled_kwargs and hasattr(unwrapped, "pytask_meta"):
+            unwrapped.pytask_meta.attributes["coiled_kwargs"] = coiled_kwargs
+
         # Store it in the global variable ``COLLECTED_TASKS`` to avoid garbage
         # collection when the function definition is overwritten in a loop.
         COLLECTED_TASKS[path].append(unwrapped)
 
         return unwrapped
 
     # In case the decorator is used without parentheses, wrap the function which is
@@ -168,25 +198,24 @@
     after: str | Callable[..., Any] | list[Callable[..., Any]] | None,
 ) -> str | list[Callable[..., Any]]:
     if not after:
         return []
     if isinstance(after, str):
         return after
     if callable(after):
-        if not hasattr(after, "pytask_meta"):
-            after.pytask_meta = CollectionMetadata()  # type: ignore[attr-defined]
-        return [after.pytask_meta._id]  # type: ignore[attr-defined]
+        after = [after]
     if isinstance(after, list):
         new_after = []
         for func in after:
             if not hasattr(func, "pytask_meta"):
-                func.pytask_meta = CollectionMetadata()  # type: ignore[attr-defined]
-            new_after.append(func.pytask_meta._id)  # type: ignore[attr-defined]
+                func = task()(func)  # noqa: PLW2901
+            new_after.append(func.pytask_meta._id)
+        return new_after
     msg = (
-        "'after' should be an expression string, a task, or a list of class. Got "
+        "'after' should be an expression string, a task, or a list of tasks. Got "
         f"{after}, instead."
     )
     raise TypeError(msg)
 
 
 def parse_collected_tasks_with_task_marker(
     tasks: list[Callable[..., Any]],
@@ -227,15 +256,15 @@
 
 def _parse_task(task: Callable[..., Any]) -> tuple[str, Callable[..., Any]]:
     """Parse a single task."""
     meta = task.pytask_meta  # type: ignore[attr-defined]
 
     if meta.name is None and task.__name__ == "_":
         msg = (
-            "A task function either needs 'name' passed by the ``@pytask.mark.task`` "
+            "A task function either needs 'name' passed by the ``@task`` "
             "decorator or the function name of the task function must not be '_'."
         )
         raise ValueError(msg)
 
     parsed_name = task.__name__ if meta.name is None else meta.name
     parsed_kwargs = _parse_task_kwargs(meta.kwargs)
 
@@ -251,15 +280,15 @@
         return kwargs
     # Handle namedtuples.
     if callable(getattr(kwargs, "_asdict", None)):
         return kwargs._asdict()
     if attrs.has(type(kwargs)):
         return attrs.asdict(kwargs)
     msg = (
-        "'@pytask.mark.task(kwargs=...) needs to be a dictionary, namedtuple or an "
+        "'@task(kwargs=...) needs to be a dictionary, namedtuple or an "
         "instance of an attrs class."
     )
     raise ValueError(msg)
 
 
 def parse_keyword_arguments_from_signature_defaults(
     task: Callable[..., Any],
```

### Comparing `pytask-0.4.7/src/_pytask/traceback.py` & `pytask-0.5.0/src/_pytask/traceback.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """Process tracebacks."""
+
 from __future__ import annotations
 
 from pathlib import Path
 from types import TracebackType
+from typing import TYPE_CHECKING
 from typing import ClassVar
 from typing import Generator
 from typing import Tuple
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import Union
 
-import _pytask
 import pluggy
-from _pytask.outcomes import Exit
-from _pytask.tree_util import TREE_UTIL_LIB_DIRECTORY
 from attrs import define
+from attrs import field
 from rich.traceback import Traceback as RichTraceback
 
+import _pytask
+from _pytask.outcomes import Exit
+from _pytask.tree_util import TREE_UTIL_LIB_DIRECTORY
+
 if TYPE_CHECKING:
-    from rich.console import ConsoleOptions
     from rich.console import Console
+    from rich.console import ConsoleOptions
     from rich.console import RenderResult
     from typing_extensions import TypeAlias
 
 
 __all__ = [
     "Traceback",
-    "remove_internal_traceback_frames_from_exc_info",
     "remove_traceback_from_exc_info",
 ]
 
 
 _PLUGGY_DIRECTORY = Path(pluggy.__file__).parent
 _PYTASK_DIRECTORY = Path(_pytask.__file__).parent
 
@@ -40,29 +42,34 @@
 ]
 OptionalExceptionInfo: TypeAlias = Union[ExceptionInfo, Tuple[None, None, None]]
 
 
 @define
 class Traceback:
     exc_info: OptionalExceptionInfo
+    show_locals: bool = field()
 
-    show_locals: ClassVar[bool] = False
+    _show_locals: ClassVar[bool] = False
     suppress: ClassVar[tuple[Path, ...]] = (
         _PLUGGY_DIRECTORY,
-        TREE_UTIL_LIB_DIRECTORY,
         _PYTASK_DIRECTORY,
+        TREE_UTIL_LIB_DIRECTORY,
     )
 
+    @show_locals.default
+    def _show_locals_default(self) -> bool:
+        return self._show_locals
+
     def __rich_console__(
         self, console: Console, console_options: ConsoleOptions
     ) -> RenderResult:
         if self.exc_info and isinstance(self.exc_info[1], Exit):
             self.exc_info = remove_traceback_from_exc_info(self.exc_info)
 
-        filtered_exc_info = remove_internal_traceback_frames_from_exc_info(
+        filtered_exc_info = _remove_internal_traceback_frames_from_exc_info(
             self.exc_info, suppress=self.suppress
         )
 
         # The tracebacks returned by pytask-parallel are strings.
         if isinstance(filtered_exc_info[2], str):
             yield filtered_exc_info[2]
         else:
@@ -74,15 +81,15 @@
 def remove_traceback_from_exc_info(
     exc_info: OptionalExceptionInfo,
 ) -> OptionalExceptionInfo:
     """Remove traceback from exception."""
     return (exc_info[0], exc_info[1], None)  # type: ignore[return-value]
 
 
-def remove_internal_traceback_frames_from_exc_info(
+def _remove_internal_traceback_frames_from_exc_info(
     exc_info: OptionalExceptionInfo,
     suppress: tuple[Path, ...] = (
         _PLUGGY_DIRECTORY,
         TREE_UTIL_LIB_DIRECTORY,
         _PYTASK_DIRECTORY,
     ),
 ) -> OptionalExceptionInfo:
@@ -111,15 +118,15 @@
     The conversion between exceptions and ``sys.exc_info`` is explained here:
     https://stackoverflow.com/a/59041463/7523785.
 
     """
     if exc is None:
         return exc
 
-    _, _, tb = remove_internal_traceback_frames_from_exc_info(
+    _, _, tb = _remove_internal_traceback_frames_from_exc_info(
         (type(exc), exc, exc.__traceback__)
     )
     exc.__traceback__ = tb
     return exc
 
 
 def _is_internal_or_hidden_traceback_frame(
```

### Comparing `pytask-0.4.7/src/_pytask/tree_util.py` & `pytask-0.5.0/src/_pytask/tree_util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Contains code for tree utilities."""
+
 from __future__ import annotations
 
 import functools
 from pathlib import Path
 
 import optree
 from optree import PyTree
 from optree import tree_flatten_with_path as _optree_tree_flatten_with_path
 from optree import tree_leaves as _optree_tree_leaves
 from optree import tree_map as _optree_tree_map
 from optree import tree_map_with_path as _optree_tree_map_with_path
 from optree import tree_structure as _optree_tree_structure
 
-
 __all__ = [
     "PyTree",
     "TREE_UTIL_LIB_DIRECTORY",
     "tree_flatten_with_path",
     "tree_leaves",
     "tree_map",
     "tree_map_with_path",
```

### Comparing `pytask-0.4.7/src/_pytask/typing.py` & `pytask-0.5.0/src/_pytask/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import functools
 from enum import Enum
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Final
 from typing import Literal
-from typing import TYPE_CHECKING
 
 from attrs import define
 
 if TYPE_CHECKING:
+    from pytask import PTask
     from typing_extensions import TypeAlias
 
 
 __all__ = [
     "NoDefault",
     "Product",
     "ProductType",
@@ -34,14 +35,19 @@
 def is_task_function(obj: Any) -> bool:
     """Check if an object is a task function."""
     return (callable(obj) and hasattr(obj, "__name__")) or (
         isinstance(obj, functools.partial) and hasattr(obj.func, "__name__")
     )
 
 
+def is_task_generator(task: PTask) -> bool:
+    """Check if a task is a generator."""
+    return task.attributes.get("is_generator", False)
+
+
 class _NoDefault(Enum):
     """A singleton for no defaults.
 
     We make this an Enum
     1) because it round-trips through pickle correctly (see GH#40397)
     2) because mypy does not understand singletons
```

### Comparing `pytask-0.4.7/src/_pytask/warnings.py` & `pytask-0.5.0/src/_pytask/warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """Contains code for capturing warnings."""
+
 from __future__ import annotations
 
 from collections import defaultdict
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
-from typing import TYPE_CHECKING
 
 import click
+from attrs import define
+from rich.padding import Padding
+from rich.panel import Panel
+
 from _pytask.console import console
 from _pytask.pluginmanager import hookimpl
+from _pytask.warnings_utils import WarningReport
 from _pytask.warnings_utils import catch_warnings_for_item
 from _pytask.warnings_utils import parse_filterwarnings
-from _pytask.warnings_utils import WarningReport
-from attrs import define
-from rich.padding import Padding
-from rich.panel import Panel
 
 if TYPE_CHECKING:
     from rich.console import Console
-    from _pytask.node_protocols import PTask
     from rich.console import ConsoleOptions
-    from _pytask.session import Session
     from rich.console import RenderResult
 
+    from _pytask.node_protocols import PTask
+    from _pytask.session import Session
+
 
 @hookimpl
 def pytask_extend_command_line_interface(cli: click.Group) -> None:
     """Extend the cli."""
     cli.commands["build"].params.extend(
         [
             click.Option(
@@ -53,28 +56,28 @@
         config["pm"].register(WarningsNameSpace)
 
 
 class WarningsNameSpace:
     """A namespace for the warnings plugin."""
 
     @staticmethod
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_collect(session: Session) -> Generator[None, None, None]:
         """Catch warnings while executing a task."""
         with catch_warnings_for_item(session=session):
-            yield
+            return (yield)
 
     @staticmethod
-    @hookimpl(hookwrapper=True)
+    @hookimpl(wrapper=True)
     def pytask_execute_task(
         session: Session, task: PTask
     ) -> Generator[None, None, None]:
         """Catch warnings while executing a task."""
         with catch_warnings_for_item(session=session, task=task):
-            yield
+            return (yield)
 
     @staticmethod
     @hookimpl(trylast=True)
     def pytask_log_session_footer(session: Session) -> None:
         """Log warnings at the end of a session."""
         if session.warnings:
             renderable = _WarningsRenderable(session.warnings)
```

### Comparing `pytask-0.4.7/src/_pytask/warnings_utils.py` & `pytask-0.5.0/src/_pytask/warnings_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Contains utility functions for warnings."""
+
 from __future__ import annotations
 
 import functools
 import re
 import textwrap
 import warnings
 from contextlib import contextmanager
-from typing import cast
+from typing import TYPE_CHECKING
 from typing import Generator
 from typing import NamedTuple
-from typing import TYPE_CHECKING
+from typing import cast
 
 from _pytask.mark_utils import get_marks
 from _pytask.outcomes import Exit
 
-
 if TYPE_CHECKING:
     from _pytask.node_protocols import PTask
     from _pytask.session import Session
 
 
 __all__ = [
     "WarningReport",
@@ -91,15 +91,15 @@
     if module and escape:
         module = re.escape(module) + r"\Z"
     if lineno_:
         try:
             lineno = int(lineno_)
             if lineno < 0:
                 msg = "number is negative"
-                raise ValueError(msg)
+                raise ValueError(msg)  # noqa: TRY301
         except ValueError as e:
             raise Exit(  # noqa: B904
                 error_template.format(error=f"invalid lineno {lineno_!r}: {e}")
             )
     else:
         lineno = 0
     return action, message, category, module, lineno
```

### Comparing `pytask-0.4.7/src/pytask/__init__.py` & `pytask-0.5.0/src/pytask/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,115 +1,122 @@
 """Contains the main namespace for pytask."""
-from __future__ import annotations
+
+from __future__ import annotations  # noqa: I001
 
 from _pytask import __version__
 from _pytask._hashlib import hash_value
 from _pytask.build import build
 from _pytask.capture_utils import CaptureMethod
 from _pytask.capture_utils import ShowCapture
+from _pytask.logging_utils import TaskExecutionStatus
+
+
 from _pytask.click import ColoredCommand
 from _pytask.click import ColoredGroup
 from _pytask.click import EnumChoice
-from _pytask.collect_utils import depends_on
 from _pytask.collect_utils import parse_dependencies_from_task_function
 from _pytask.collect_utils import parse_products_from_task_function
-from _pytask.collect_utils import produces
 from _pytask.compat import check_for_optional_program
 from _pytask.compat import import_optional_dependency
 from _pytask.console import console
 from _pytask.dag_command import build_dag
 from _pytask.data_catalog import DataCatalog
 from _pytask.database_utils import BaseTable
-from _pytask.database_utils import create_database
 from _pytask.database_utils import DatabaseSession
 from _pytask.database_utils import State
+from _pytask.database_utils import create_database
 from _pytask.exceptions import CollectionError
 from _pytask.exceptions import ConfigurationError
 from _pytask.exceptions import ExecutionError
 from _pytask.exceptions import NodeNotCollectedError
+from _pytask.exceptions import NodeLoadError
 from _pytask.exceptions import NodeNotFoundError
 from _pytask.exceptions import PytaskError
 from _pytask.exceptions import ResolvingDependenciesError
-from _pytask.mark import Mark
 from _pytask.mark import MARK_GEN as mark  # noqa: N811
+from _pytask.mark import Mark
 from _pytask.mark import MarkDecorator
 from _pytask.mark import MarkGenerator
 from _pytask.mark_utils import get_all_marks
 from _pytask.mark_utils import get_marks
 from _pytask.mark_utils import has_mark
 from _pytask.mark_utils import remove_marks
 from _pytask.mark_utils import set_marks
 from _pytask.models import CollectionMetadata
 from _pytask.models import NodeInfo
 from _pytask.node_protocols import PNode
 from _pytask.node_protocols import PPathNode
+from _pytask.node_protocols import PProvisionalNode
 from _pytask.node_protocols import PTask
 from _pytask.node_protocols import PTaskWithPath
+from _pytask.nodes import DirectoryNode
 from _pytask.nodes import PathNode
 from _pytask.nodes import PickleNode
 from _pytask.nodes import PythonNode
 from _pytask.nodes import Task
 from _pytask.nodes import TaskWithoutPath
 from _pytask.outcomes import CollectionOutcome
-from _pytask.outcomes import count_outcomes
 from _pytask.outcomes import Exit
 from _pytask.outcomes import ExitCode
 from _pytask.outcomes import Persisted
 from _pytask.outcomes import Skipped
 from _pytask.outcomes import SkippedAncestorFailed
 from _pytask.outcomes import SkippedUnchanged
 from _pytask.outcomes import TaskOutcome
+from _pytask.outcomes import count_outcomes
 from _pytask.pluginmanager import get_plugin_manager
 from _pytask.pluginmanager import hookimpl
 from _pytask.pluginmanager import storage
 from _pytask.profile import Runtime
 from _pytask.reports import CollectionReport
 from _pytask.reports import DagReport
 from _pytask.reports import ExecutionReport
 from _pytask.session import Session
 from _pytask.task_utils import task
-from _pytask.traceback import remove_internal_traceback_frames_from_exc_info
 from _pytask.traceback import Traceback
-from _pytask.typing import is_task_function
 from _pytask.typing import Product
+from _pytask.typing import is_task_function
+from _pytask.warnings_utils import WarningReport
 from _pytask.warnings_utils import parse_warning_filter
 from _pytask.warnings_utils import warning_record_to_str
-from _pytask.warnings_utils import WarningReport
 
 # _pytask.cli needs to be imported last because it triggers extending the cli and
 # therefore loading plugins which will attempt to import modules that might only be
 # partially initialized. Maybe not here, but definitely for plugins.
-from _pytask.cli import cli  # noreorder
+from _pytask.cli import cli
 
 __all__ = [
     "BaseTable",
     "CaptureMethod",
     "CollectionError",
     "CollectionMetadata",
     "CollectionOutcome",
     "CollectionReport",
     "ColoredCommand",
     "ColoredGroup",
     "ConfigurationError",
     "DagReport",
     "DataCatalog",
     "DatabaseSession",
+    "DirectoryNode",
     "EnumChoice",
     "ExecutionError",
     "ExecutionReport",
     "Exit",
     "ExitCode",
     "Mark",
     "MarkDecorator",
     "MarkGenerator",
     "NodeInfo",
+    "NodeLoadError",
     "NodeNotCollectedError",
     "NodeNotFoundError",
     "PNode",
     "PPathNode",
+    "PProvisionalNode",
     "PTask",
     "PTaskWithPath",
     "PathNode",
     "Persisted",
     "PickleNode",
     "Product",
     "PytaskError",
@@ -119,40 +126,38 @@
     "Session",
     "ShowCapture",
     "Skipped",
     "SkippedAncestorFailed",
     "SkippedUnchanged",
     "State",
     "Task",
+    "TaskExecutionStatus",
     "TaskOutcome",
     "TaskWithoutPath",
     "Traceback",
     "WarningReport",
     "__version__",
     "build",
     "build_dag",
     "check_for_optional_program",
     "cli",
     "console",
     "count_outcomes",
     "create_database",
-    "depends_on",
     "get_all_marks",
     "get_marks",
     "get_plugin_manager",
     "has_mark",
     "hash_value",
     "hookimpl",
     "import_optional_dependency",
     "is_task_function",
     "mark",
     "parse_dependencies_from_task_function",
     "parse_products_from_task_function",
     "parse_warning_filter",
-    "produces",
-    "remove_internal_traceback_frames_from_exc_info",
     "remove_marks",
     "set_marks",
     "storage",
     "task",
     "warning_record_to_str",
 ]
```

