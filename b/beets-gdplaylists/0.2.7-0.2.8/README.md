# Comparing `tmp/beets_gdplaylists-0.2.7.tar.gz` & `tmp/beets_gdplaylists-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beets_gdplaylists-0.2.7.tar", last modified: Sat May 25 12:05:05 2024, max compression
+gzip compressed data, was "beets_gdplaylists-0.2.8.tar", last modified: Sun May 26 13:15:29 2024, max compression
```

## Comparing `beets_gdplaylists-0.2.7.tar` & `beets_gdplaylists-0.2.8.tar`

### file list

```diff
@@ -1,87 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.121042 beets_gdplaylists-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.105042 beets_gdplaylists-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.109042 beets_gdplaylists-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/.github/workflows/createrelease.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/.github/workflows/testpythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-25 12:05:05.121042 beets_gdplaylists-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.117042 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-25 12:05:05.000000 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-25 12:05:05.000000 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:05:05.000000 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-25 12:05:05.000000 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 12:05:05.000000 beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.109042 beets_gdplaylists-0.2.7/beetsplug/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.109042 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.109042 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/gdplex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.117042 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1969-11-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1969-12-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1970-01-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1970-01-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-10-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-11-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-12-10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-03-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-24.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-09-07.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-09-08.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-10-30.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-02-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-02-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-17.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-21.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-06-22.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-01.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-02.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-29.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-04-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-12-31.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-03.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-04.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-09.yml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-15.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-25.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1984-04-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1984-04-20.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1985-04-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1985-04-28.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1987-03-26.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1987-03-27.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-06-23.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-07-18.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-07-19.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/justfile
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:05:05.117042 beets_gdplaylists-0.2.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/scripts/mbdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/scripts/releases.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:05:05.121042 beets_gdplaylists-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 12:04:55.000000 beets_gdplaylists-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.158819 beets_gdplaylists-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.162819 beets_gdplaylists-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/.github/workflows/createrelease.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/.github/workflows/testpythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-26 13:15:29.000000 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-26 13:15:29.000000 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:15:29.000000 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 13:15:29.000000 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 13:15:29.000000 beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.162819 beets_gdplaylists-0.2.8/beetsplug/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.162819 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.162819 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/gdplex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1969-11-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1969-12-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1970-01-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1970-01-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-10-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-11-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-12-10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-03-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-03-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-04-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-05-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-03-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-09-07.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-09-08.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-10-30.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-02-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-02-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-21.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-06-22.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-01.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-02.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-29.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-04-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-12-31.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-03.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-04.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-09.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-25.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1984-04-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1984-04-20.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1985-04-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1985-04-28.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1987-03-26.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1987-03-27.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-06-23.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-07-18.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-07-19.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/scripts/mbdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/scripts/releases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:15:29.174819 beets_gdplaylists-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 13:15:16.000000 beets_gdplaylists-0.2.8/setup.py
```

### Comparing `beets_gdplaylists-0.2.7/.github/workflows/createrelease.yml` & `beets_gdplaylists-0.2.8/.github/workflows/createrelease.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/.github/workflows/pythonpublish.yml` & `beets_gdplaylists-0.2.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/.github/workflows/testpythonpublish.yml` & `beets_gdplaylists-0.2.8/.github/workflows/testpythonpublish.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/LICENSE` & `beets_gdplaylists-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/PKG-INFO` & `beets_gdplaylists-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.7
+Version: 0.2.8
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.7/README.md` & `beets_gdplaylists-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/PKG-INFO` & `beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-gdplaylists
-Version: 0.2.7
+Version: 0.2.8
 Summary: beets plugin to create Grateful Dead playlists
 Author-email: Ross Hendry <rhendry@gmail.com>
 Project-URL: Repository, https://github.com/chooban/beets-gogd
 Keywords: beets,grateful dead,plex,playlists
 Platform: ALL
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beets_gdplaylists-0.2.7/beets_gdplaylists.egg-info/SOURCES.txt` & `beets_gdplaylists-0.2.8/beets_gdplaylists.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 beetsplug/gdplaylists/playlists/1969-12-26.yml
 beetsplug/gdplaylists/playlists/1970-01-02.yml
 beetsplug/gdplaylists/playlists/1970-01-03.yml
 beetsplug/gdplaylists/playlists/1971-10-24.yml
 beetsplug/gdplaylists/playlists/1971-11-20.yml
 beetsplug/gdplaylists/playlists/1971-12-09.yml
 beetsplug/gdplaylists/playlists/1971-12-10.yml
+beetsplug/gdplaylists/playlists/1972-03-22.yml
+beetsplug/gdplaylists/playlists/1972-03-23.yml
+beetsplug/gdplaylists/playlists/1972-04-24.yml
+beetsplug/gdplaylists/playlists/1972-05-24.yml
 beetsplug/gdplaylists/playlists/1972-09-03.yml
 beetsplug/gdplaylists/playlists/1972-09-09.yml
 beetsplug/gdplaylists/playlists/1972-09-19.yml
 beetsplug/gdplaylists/playlists/1972-10-17.yml
 beetsplug/gdplaylists/playlists/1972-10-18.yml
 beetsplug/gdplaylists/playlists/1972-10-19.yml
 beetsplug/gdplaylists/playlists/1973-03-24.yml
```

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/__pycache__/gdplex.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/gdplex.py` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/gdplex.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1969-11-02.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1969-11-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1969-12-26.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1969-12-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1970-01-02.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1970-01-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1970-01-03.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1970-01-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-10-24.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-10-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-11-20.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-11-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-12-09.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1971-12-10.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1971-12-10.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-03.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-09.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-09-19.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-09-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-17.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-18.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1972-10-19.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1972-10-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-03-24.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-03-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-22.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-24.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-24.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-06-26.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-06-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-09-07.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-09-07.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-09-08.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-09-08.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-10-29.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1973-10-30.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1973-10-30.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-02-22.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-02-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-02-23.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-02-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-17.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-17.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-19.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-05-21.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-05-21.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-06-22.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-06-22.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1974-06-23.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1974-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-03.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-03.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,146 +1,146 @@
 title: GOGD - 1977-05-03 - The Palladium, New York, NY
 tracks:
 - title: Promised Land
   date: '1977-05-03'
   mbid: 8cd95a4d-6c06-4ba8-9b3c-b0d9391d76f5
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-1
 - title: Bertha
   date: '1977-05-03'
   mbid: 49f51500-725b-4bf6-ad0c-a537adbff698
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-2
 - title: Me and My Uncle
   date: '1977-05-03'
   mbid: cb095f4f-345f-4b58-ba15-b11c4decb570
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-3
 - title: "Peggy\u2010O"
   date: '1977-05-03'
   mbid: ec38ac8f-19c2-4bb5-862a-24aaca95ee6f
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-4
 - title: Jack Straw
   date: '1977-05-03'
   mbid: f772db12-c33f-4d10-bd5e-b2b0e92e8192
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-5
 - title: Row Jimmy
   date: '1977-05-03'
   mbid: 60f6d882-f4fd-4603-a091-fa2784158c21
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-6
 - title: Lazy Lightning
   date: '1977-05-03'
   mbid: d968f34e-03a7-4fd0-b0f3-7e514149d6d4
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-7
 - title: Supplication
   date: '1977-05-03'
   mbid: 02cd79ca-21ed-43ec-abf4-4c97092c2c30
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-8
 - title: Deal
   date: '1977-05-03'
   mbid: 3ad050d2-a754-431c-b163-3028a667c8b8
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-9
 - title: "Good Lovin\u2019"
   date: '1977-05-03'
   mbid: 3de5f26c-3d49-4666-894e-77fcdcf09fca
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-10
 - title: Ship of Fools
   date: '1977-05-03'
   mbid: 2d6aa9c7-23d5-493f-ae0e-56896de97b6f
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-11
 - title: The Music Never Stopped
   date: '1977-05-03'
   mbid: 0f299144-d494-492e-9672-aae9a163b7f0
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 1-12
 - title: Might as Well
   date: '1977-05-03'
   mbid: f6dcf8a0-f4bd-4e0d-b11e-593845c43429
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-1
 - title: Estimated Prophet
   date: '1977-05-03'
   mbid: 7ab5c4c6-63b3-4616-b0f7-c38bf3bbf5f7
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-2
 - title: Sugaree
   date: '1977-05-03'
   mbid: e1bb334b-2ea8-4497-ae4d-e5ad0640448c
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-3
 - title: Samson and Delilah
   date: '1977-05-03'
   mbid: 1d33bad2-dbd5-49fa-bbee-02c2ea743013
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-4
 - title: Friend of the Devil
   date: '1977-05-03'
   mbid: bcb2888f-a271-49bb-9fa5-9a712bf0a51e
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-5
 - title: Eyes of the World
   date: '1977-05-03'
   mbid: 9617397d-c204-4535-97bf-209a3e4e7935
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-1
 - title: Space
   date: '1977-05-03'
   mbid: 3b23ea5f-94f6-45b9-986a-285263f3d80d
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-2
 - title: Wharf Rat
   date: '1977-05-03'
   mbid: 37519319-c964-4b15-94cd-afc64de73e7d
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-3
 - title: Drums
   date: '1977-05-03'
   mbid: ec192d4e-d82c-47e8-8fcd-cd38975d077c
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-4
 - title: Not Fade Away
   date: '1977-05-03'
   mbid: e714042e-ddaf-4caf-a837-90490e623834
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-5
 - title: Around and Around
   date: '1977-05-03'
   mbid: 9c5c1861-32d1-459d-91ec-8eb9ffb7e93a
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-6
 - title: "Uncle John\u2019s Band"
   date: '1977-05-03'
   mbid: 5f1aa0b2-8e2d-4a88-ab04-6bb4750126b9
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-7
```

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-04.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-04.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 title: GOGD - 1977-05-04 - The Palladium, New York, NY
 tracks:
 - title: "Mississippi Half\u2010Step Uptown Toodeloo"
   date: '1977-05-04'
   mbid: a63d0600-529e-4430-a8fb-ec25d977bc70
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-6
 - title: Big River
   date: '1977-05-04'
   mbid: c13c8f90-2f58-4e35-b6f6-28e54d19b906
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-7
 - title: They Love Each Other
   date: '1977-05-04'
   mbid: 1aba6673-2fd9-4ce8-a42e-ff81951c6ab7
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-8
 - title: It Must Have Been the Roses
   date: '1977-05-04'
   mbid: 5a4f7635-3ae8-4c0d-b5f9-6f18c580f61f
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 2-9
 - title: Dancing in the Street
   date: '1977-05-04'
   mbid: be35e43f-4eb4-4dd1-9740-c6b037607da7
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 3-8
 - title: Estimated Prophet
   date: '1977-05-04'
   mbid: cf2b1ae1-9f49-405d-b891-0b821ed0c30e
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-1
 - title: Scarlet Begonias
   date: '1977-05-04'
   mbid: 9320ffb6-3762-4a27-a603-a36b27bd55d8
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-2
 - title: Fire on the Mountain
   date: '1977-05-04'
   mbid: 3635c065-904a-4275-a718-49b6738e8518
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-3
 - title: Terrapin Station
   date: '1977-05-04'
   mbid: 23b18f40-a9e7-4264-a7c5-ba7387f2a1c8
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-4
 - title: Playing in the Band
   date: '1977-05-04'
   mbid: 84074bc1-7c9d-421e-9c39-79874f5b9c89
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-5
 - title: Comes a Time
   date: '1977-05-04'
   mbid: 850df0ff-0a22-4145-bada-65aeee3e1433
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-6
 - title: Playing in the Band
   date: '1977-05-04'
   mbid: d029b122-4264-49c5-817d-3b2618f9271e
-  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77)"
+  release_title: "Dave\u2019s Picks Volume 50: The Palladium, New York, NY \xB7 5/3/77"
   release_mbid: f8a96a7a-1413-491f-9cde-9ac30bf348e9
   release_position: 4-7
```

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-05-26.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-05-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-01.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-01.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-02.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-02.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1977-10-29.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1977-10-29.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-04-15.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-04-18.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-04-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1978-12-31.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1978-12-31.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-03.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-03.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-04.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-04.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1979-12-09.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1979-12-09.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-15.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-15.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-25.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-25.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1983-04-26.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1983-04-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1984-04-19.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1984-04-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1984-04-20.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1984-04-20.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1985-04-27.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1985-04-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1985-04-28.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1985-04-28.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1987-03-26.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1987-03-26.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1987-03-27.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1987-03-27.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-06-23.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-06-23.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-07-18.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-07-18.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/beetsplug/gdplaylists/playlists/1990-07-19.yml` & `beets_gdplaylists-0.2.8/beetsplug/gdplaylists/playlists/1990-07-19.yml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/pyproject.toml` & `beets_gdplaylists-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/scripts/mbdl.py` & `beets_gdplaylists-0.2.8/scripts/mbdl.py`

 * *Files identical despite different names*

### Comparing `beets_gdplaylists-0.2.7/scripts/releases.yml` & `beets_gdplaylists-0.2.8/scripts/releases.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 releases:
-# - title: Rockin' The Rhein
-#   mbid: f8278162-30b5-4d2f-8ade-18c0b5bf241e
+- title: Rockin' The Rhein
+  mbid: f8278162-30b5-4d2f-8ade-18c0b5bf241e
 - title: Closing of Winterland
   mbid: fe59ec56-28f2-4722-afa9-d37d1f92903b
 - title: Listen to the River
   mbid: d50b6763-15b8-44c9-9c86-6fbc73367493
 - title: Pacific Northwest '73-'74
   mbid: ebb7953a-9c8f-4c6d-98a0-96418e98f5ed
 - title: Dave's Picks 50
```

