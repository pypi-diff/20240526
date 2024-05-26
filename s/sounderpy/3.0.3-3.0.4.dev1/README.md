# Comparing `tmp/sounderpy-3.0.3.tar.gz` & `tmp/sounderpy-3.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-3.0.3.tar", last modified: Sun Mar 24 14:16:26 2024, max compression
+gzip compressed data, was "sounderpy-3.0.4.dev1.tar", last modified: Sun May 26 11:06:33 2024, max compression
```

## Comparing `sounderpy-3.0.3.tar` & `sounderpy-3.0.4.dev1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.546359 sounderpy-3.0.3/
--rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.3/LICENSE
--rw-rw-rw-   0        0        0    11209 2024-03-24 14:16:26.533350 sounderpy-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9762 2024-03-24 13:28:59.000000 sounderpy-3.0.3/README.md
--rw-rw-rw-   0        0        0     1395 2024-03-24 14:15:55.000000 sounderpy-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-24 14:16:26.546359 sounderpy-3.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:25.950707 sounderpy-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:25.997576 sounderpy-3.0.3/src/sounderpy/
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.028821 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/
--rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.032339 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/ci/
--rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
--rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/ci/screen.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.044866 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/
--rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
--rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/available.py
--rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:25.966330 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.060501 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/io/
--rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.060501 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/plot/
--rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
--rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.185885 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
--rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
--rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
--rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
--rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
--rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
--rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
--rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
--rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
--rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
--rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
--rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
--rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
--rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
--rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
--rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
--rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
--rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
--rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
--rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
--rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.279512 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/
--rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
--rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
--rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
--rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
--rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
--rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
--rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
--rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
--rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
--rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
--rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
--rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.467816 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/
--rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
--rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
--rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
--rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
--rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
--rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
--rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
--rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
--rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
--rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
--rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
--rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
--rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
--rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
--rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
--rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
--rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
--rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
--rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
--rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
--rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
--rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
--rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
--rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
--rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.514696 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/
--rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
--rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/async.py
--rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
--rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/config.py
--rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
--rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/progress.py
--rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/utils.py
--rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
--rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.3/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0    41978 2024-03-24 13:55:06.000000 sounderpy-3.0.3/src/sounderpy/calc.py
--rw-rw-rw-   0        0        0   177673 2024-03-24 13:55:04.000000 sounderpy-3.0.3/src/sounderpy/plot.py
--rw-rw-rw-   0        0        0    97801 2024-03-24 13:26:56.000000 sounderpy-3.0.3/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2024-03-24 14:16:26.533350 sounderpy-3.0.3/src/sounderpy.egg-info/
--rw-rw-rw-   0        0        0    11209 2024-03-24 14:16:25.000000 sounderpy-3.0.3/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4156 2024-03-24 14:16:25.000000 sounderpy-3.0.3/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 14:16:25.000000 sounderpy-3.0.3/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      177 2024-03-24 14:16:25.000000 sounderpy-3.0.3/src/sounderpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-24 14:16:25.000000 sounderpy-3.0.3/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.166935 sounderpy-3.0.4.dev1/
+-rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.4.dev1/LICENSE
+-rw-rw-rw-   0        0        0    11192 2024-05-26 11:06:33.160955 sounderpy-3.0.4.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     9759 2024-05-26 00:48:06.000000 sounderpy-3.0.4.dev1/README.md
+-rw-rw-rw-   0        0        0     1379 2024-05-26 10:51:07.000000 sounderpy-3.0.4.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 11:06:33.167936 sounderpy-3.0.4.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.362280 sounderpy-3.0.4.dev1/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.418120 sounderpy-3.0.4.dev1/src/sounderpy/
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.451235 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/
+-rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.462223 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/
+-rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
+-rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/screen.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.487212 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/
+-rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
+-rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/available.py
+-rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.371672 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.496533 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/io/
+-rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.508751 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/
+-rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
+-rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.708731 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
+-rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
+-rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
+-rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
+-rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
+-rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
+-rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
+-rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
+-rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
+-rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
+-rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
+-rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
+-rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
+-rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
+-rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
+-rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
+-rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
+-rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
+-rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
+-rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
+-rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.843838 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/
+-rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
+-rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
+-rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
+-rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
+-rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
+-rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
+-rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
+-rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
+-rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
+-rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.073306 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/
+-rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
+-rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
+-rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
+-rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
+-rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
+-rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
+-rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
+-rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
+-rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
+-rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
+-rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
+-rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
+-rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
+-rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
+-rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
+-rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
+-rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
+-rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
+-rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
+-rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
+-rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
+-rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
+-rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
+-rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
+-rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.142500 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/
+-rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
+-rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async.py
+-rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
+-rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/config.py
+-rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
+-rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/progress.py
+-rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/utils.py
+-rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
+-rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0    44655 2024-05-26 10:51:15.000000 sounderpy-3.0.4.dev1/src/sounderpy/calc.py
+-rw-rw-rw-   0        0        0   193583 2024-05-26 11:04:56.000000 sounderpy-3.0.4.dev1/src/sounderpy/plot.py
+-rw-rw-rw-   0        0        0    97993 2024-05-26 01:49:30.000000 sounderpy-3.0.4.dev1/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.149478 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/
+-rw-rw-rw-   0        0        0    11192 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4156 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-3.0.3/LICENSE` & `sounderpy-3.0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/PKG-INFO` & `sounderpy-3.0.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.3
+Version: 3.0.4.dev1
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
-Author-email: "Kyle J Gillett, Central Michigan University" <kjgillett10@gmail.com>
+Author-email: "Kyle J Gillett, University of North Dakota" <kjgillett10@gmail.com>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
-Project-URL: My Website, https://kylegillettwx.wordpress.com/
+Project-URL: My Website, https://kylegillettphoto.com
 Keywords: meteorology,science,data-analysis,weather,forecasting
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cartopy>=0.21.0
 Requires-Dist: cdsapi>=0.6.1
 Requires-Dist: ecape-parcel>=1.2.0.2
-Requires-Dist: matplotlib<=3.7.1,>=3.3.0
+Requires-Dist: matplotlib>=3.3.0
 Requires-Dist: metpy>=1.5.1
 Requires-Dist: netcdf4>=1.6.4
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.2.0
-Requires-Dist: arm_pyart>=1.16.1
 Requires-Dist: siphon>=0.9
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: xarray>=0.18.0
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 </div>
 
 # SounderPy, the vertical profile data retrieval and analysis tool for Python
-LATEST VERSION: v3.0.3 |  RELEASED: March, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
+LATEST VERSION: v3.0.4 |  RELEASED: May, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
 
 A Python package that helps you to access and plot vertical profile data for meteorological analysis 
 
 [![PyPI Package](https://img.shields.io/pypi/v/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://github.com/kylejgillett/sounderpy/blob/main/LICENSE.txt)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
@@ -173,29 +173,29 @@
    <img src="https://kylejgillett.github.io/sounderpy/_images/example-hodograph_dark.png" width="600">
    </div>
 
 ### To learn more about what you can do with SounderPy, [check out the documentation](https://kylejgillett.github.io/sounderpy/)
 ------
 
 ## AUTHORS AND CONTRIBUTORS
-### **AUTHOR: Kyle J Gillett, Central Michigan University** 
+### **AUTHOR: Kyle J Gillett, University of North Dakota** 
 ##### *CONTRIBUTOR: Scott Thomas, NWS Grand Rapids | VWP Hodograph, Buoy-sites listing*
 ##### *CONTRIBUTOR: Amelia R H Urquhart, University of Oklahoma | ecape-parcels library*
 ##### *CONTRIBUTOR: Daryl Herzmann, Iowa State University | SounderPy Feedstock for conda-forge*
 
 ------
 
 
 ## CITING SOUNDERPY
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10443609.svg)](https://doi.org/10.5281/zenodo.10443609)
 
 
 in AMS format:
 
-- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.3). Py-Pi, https://pypi.org/project/sounderpy/
+- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.4). Py-Pi, https://pypi.org/project/sounderpy/
 
 ------
 
 
 
 ## REFERENCES
 - Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 10.1038/s41586-020-2649-2.
```

### Comparing `sounderpy-3.0.3/README.md` & `sounderpy-3.0.4.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 </div>
 
 # SounderPy, the vertical profile data retrieval and analysis tool for Python
-LATEST VERSION: v3.0.3 |  RELEASED: March, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
+LATEST VERSION: v3.0.4 |  RELEASED: May, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
 
 A Python package that helps you to access and plot vertical profile data for meteorological analysis 
 
 [![PyPI Package](https://img.shields.io/pypi/v/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://github.com/kylejgillett/sounderpy/blob/main/LICENSE.txt)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
@@ -139,29 +139,29 @@
    <img src="https://kylejgillett.github.io/sounderpy/_images/example-hodograph_dark.png" width="600">
    </div>
 
 ### To learn more about what you can do with SounderPy, [check out the documentation](https://kylejgillett.github.io/sounderpy/)
 ------
 
 ## AUTHORS AND CONTRIBUTORS
-### **AUTHOR: Kyle J Gillett, Central Michigan University** 
+### **AUTHOR: Kyle J Gillett, University of North Dakota** 
 ##### *CONTRIBUTOR: Scott Thomas, NWS Grand Rapids | VWP Hodograph, Buoy-sites listing*
 ##### *CONTRIBUTOR: Amelia R H Urquhart, University of Oklahoma | ecape-parcels library*
 ##### *CONTRIBUTOR: Daryl Herzmann, Iowa State University | SounderPy Feedstock for conda-forge*
 
 ------
 
 
 ## CITING SOUNDERPY
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10443609.svg)](https://doi.org/10.5281/zenodo.10443609)
 
 
 in AMS format:
 
-- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.3). Py-Pi, https://pypi.org/project/sounderpy/
+- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.4). Py-Pi, https://pypi.org/project/sounderpy/
 
 ------
 
 
 
 ## REFERENCES
 - Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 10.1038/s41586-020-2649-2.
```

### Comparing `sounderpy-3.0.3/pyproject.toml` & `sounderpy-3.0.4.dev1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "3.0.3"
+version = "3.0.4dev1"
 authors = [
-  { name="Kyle J Gillett, Central Michigan University", email="kjgillett10@gmail.com" },
+  { name="Kyle J Gillett, University of North Dakota", email="kjgillett10@gmail.com" },
 ]
 description = "Vertical Profile Data Retrieval and Analysis Tool For Python"
 readme = "README.md"
 keywords = ["meteorology", "science", "data-analysis", "weather", "forecasting"]
 requires-python = ">=3.1"
 classifiers = [
     "Programming Language :: Python",
@@ -19,26 +19,26 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
+	"cartopy>=0.21.0",
 	"cdsapi>=0.6.1",
 	"ecape-parcel>=1.2.0.2",
-	"matplotlib>=3.3.0, <=3.7.1",
+	"matplotlib>=3.3.0",
 	"metpy>=1.5.1",
 	"netcdf4>=1.6.4",
 	"numpy>=1.20.0",
 	"pandas>=1.2.0",
-	"arm_pyart>=1.16.1",
 	"siphon>=0.9",
 	"scipy>= 1.10.1",
 	"xarray>=0.18.0",
 ]
 
 [project.urls]
 "Docs" = "https://kylejgillett.github.io/sounderpy/"
 "Code" = "https://github.com/kylejgillett/sounderpy"
 "Operational Site" = "https://sounderpysoundings.anvil.app/"
 "PyPi" = "https://pypi.org/project/sounderpy/"
-"My Website" = "https://kylegillettwx.wordpress.com/"
+"My Website" = "https://kylegillettphoto.com"
```

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/available.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/available.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/datasources/data_source.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/data_source.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/async.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/config.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/config.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/progress.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/progress.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py` & `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/__init__.py` & `sounderpy-3.0.4.dev1/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.3/src/sounderpy/calc.py` & `sounderpy-3.0.4.dev1/src/sounderpy/calc.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 from .SHARPPYMAIN.sharppy.sharptab.params import *
 
 from ecape_parcel.ecape_calc import calc_ecape
 
 import numpy as np
 import numpy.ma as ma
 import warnings
+import copy
 import metpy.calc as mpcalc
 from metpy.units import units
 
 
 
-#########################################################
-#            SOUNDERPY SPYCALC FUNCTIONS                #
-# (C) KYLE J GILLETT, CENTRAL MICHIGAN UNIVERSTIY, 2024 #
-#########################################################
+########################################################
+#            SOUNDERPY SPYCALC FUNCTIONS               #
+# (C) KYLE J GILLETT, UNIVERSITY OF NORTH DAKOTA, 2024 #
+########################################################
 
 
 
 class sounding_params:
 
 
-    def __init__(self, clean_data, storm_motion='right_moving'):
+    def __init__(self, clean_data, storm_motion='right_moving', modify_sfc=None):
             self.clean_data = clean_data 
             self.storm_motion = storm_motion
+            self.modify_sfc = modify_sfc
 
             
     ######################################################################################################
     ### CALC FUNCTION -- COMPUTE VALUES ###
     ######################################################################################################        
     def calc(self):
         
@@ -58,29 +60,39 @@
         # declare easy variable names for reuse from `clean_data`
         # first, check for correct units: 
         if self.clean_data['T'].units != 'degree_Celsius':
             self.clean_data['T'] =  self.clean_data['T'].to(units.degC)
         if self.clean_data['Td'].units != 'degree_Celsius':
             self.clean_data['Td'] = self.clean_data['Td'].to(units.degC)
         
-        T   = self.clean_data['T']
-        Td  = self.clean_data['Td']
-        p   = self.clean_data['p']
-        z   = self.clean_data['z']
-        u   = self.clean_data['u']
-        v   = self.clean_data['v']
+        # SFC CORRECTION
+        # create a deepcopy of clean_data
+        sounding_data = copy.deepcopy(self.clean_data)
+    
+        # if `modify_sfc` is a list, correct the sfc values
+        if str(type(self.modify_sfc)) == "<class 'list'>":
+            sounding_data['T'][0] = self.modify_sfc[0]*units.degC
+            sounding_data['Td'][0] = self.modify_sfc[1]*units.degC
+        
+        
+        T   = sounding_data['T']
+        Td  = sounding_data['Td']
+        p   = sounding_data['p']
+        z   = sounding_data['z']
+        u   = sounding_data['u']
+        v   = sounding_data['v']
         wd  = mpcalc.wind_direction(u, v)
         ws  = mpcalc.wind_speed(u, v)
 
         # compute useful variables and add them to a new dict of 
         # data that this function will return 
-        if self.clean_data['site_info']['site-elv'] == 9999:
+        if sounding_data['site_info']['site-elv'] == 9999:
             general['elevation'] = z[0].m
         else:
-            general['elevation'] = int(self.clean_data['site_info']['site-elv'])
+            general['elevation'] = int(sounding_data['site_info']['site-elv'])
 
 
         general['sfc_pressure']  = (p[0].m*(1-(0.0065*(general['elevation']))/(T[0].m+(0.0065*(general['elevation']))+273.15))**-5.257)*units.hPa
         general['wet_bulb']      = mpcalc.wet_bulb_temperature(p, T, Td)
         general['rel_humidity']  = mpcalc.relative_humidity_from_dewpoint(T, Td)*100
         general['spec_humidity'] = (mpcalc.specific_humidity_from_dewpoint(p, Td)*1000)*units.g/units.kg
         general['mix_ratio']     = mpcalc.mixing_ratio_from_specific_humidity(general['spec_humidity'])
@@ -107,30 +119,32 @@
                 except IndexError:
                     # Handle the case where the index is out of bounds
                     varinterp[i] = np.nan 
             return varinterp 
 
         resolution=100
 
-        rhINTRP = general['rel_humidity'].m[np.isnan(z)==False]
-        mrINTRP = general['mix_ratio'].m[np.isnan(z)==False]
+        rhINTRP     = general['rel_humidity'].m[np.isnan(z)==False]
+        mrINTRP     = general['mix_ratio'].m[np.isnan(z)==False]
         thetaINTRP  = general['theta'].m[np.isnan(z)==False]
         thetaeINTRP = general['theta_e'].m[np.isnan(z)==False]
+        wbINTRP     = general['wet_bulb'].m[np.isnan(z)==False]
         pINTRP  = p.m[np.isnan(z)==False]
         tINTRP  = T.m[np.isnan(z)==False]
         uINTRP  = u.m[np.isnan(z)==False]
         vINTRP  = v.m[np.isnan(z)==False]
         zINTRP  = z.m[np.isnan(z)==False]
         zINTRP  = zINTRP-zINTRP[0]
         # Interpolation, add to intrp dict
         intrp['rhINTRP'] = interpolate(rhINTRP,zINTRP,resolution)
         intrp['tINTRP']  = interpolate(tINTRP,zINTRP,resolution)
         intrp['mrINTRP'] = interpolate(mrINTRP,zINTRP,resolution)
         intrp['thetaINTRP']  = interpolate(thetaINTRP,zINTRP,resolution)
         intrp['thetaeINTRP'] = interpolate(thetaeINTRP,zINTRP,resolution)
+        intrp['wbINTRP'] = interpolate(wbINTRP,zINTRP,resolution)
         intrp['pINTRP'] = interpolate(pINTRP,zINTRP,resolution)
         intrp['uINTRP'] = interpolate(uINTRP,zINTRP,resolution)
         intrp['vINTRP'] = interpolate(vINTRP,zINTRP,resolution)
         intrp['zINTRP'] = interpolate(zINTRP,zINTRP,resolution)
 
         hgt_lvls = {}
         hgt_var_list = ['h0', 'h05', 'h1', 'h15', 'h2', 'h25', 
@@ -157,14 +171,23 @@
             general['frz_pt_z'] = intrp['zINTRP'][frz_pt_index]*units.m
         except IndexError:
             general['frz_pt_p'] = ma.masked
             general['frz_pt_z'] = ma.masked
             warnings.warn("This sounding does not have a freezing point (not enough data)", Warning)
             pass
 
+        try: 
+            wb_frz_pt_index = intrp['wbINTRP'].tolist().index(list(filter(lambda i: i <= 0, intrp['wbINTRP'].tolist()))[0])
+            general['wb_frz_pt_p'] = intrp['pINTRP'][wb_frz_pt_index]*units.hPa
+            general['wb_frz_pt_z'] = intrp['zINTRP'][wb_frz_pt_index]*units.m
+        except IndexError:
+            general['wb_frz_pt_p'] = ma.masked
+            general['wb_frz_pt_z'] = ma.masked
+            warnings.warn("This sounding does not have a wet bulb freezing point (not enough data)", Warning)
+            pass
 
 
         ###################################################################
         ### SHARPPY VARIABLES CALC ###
         ###################################################################
         # create sharppy profile object
         prof = create_profile(profile='default',pres=p.m, hght=z.m, tmpc=T.m, dwpc=Td.m, wspd=ws, wdir=wd, 
@@ -183,14 +206,15 @@
         thermo['sb_lcl_p'] = sbpcl.lclpres
         thermo['sb_lcl_z'] = sbpcl.lclhght 
         thermo['sb_lfc_p'] = sbpcl.lfcpres
         thermo['sb_lfc_z'] = sbpcl.lfchght
         thermo['sb_el_p']  = sbpcl.elpres  
         thermo['sb_el_z']  = sbpcl.elhght
         thermo['sb_el_T']  = temp(prof, pres(prof, thermo['sb_el_z']))
+        thermo['sb_mpl_p'] = sbpcl.mplpres
         thermo['sbcape']   = sbpcl.bplus
         thermo['sbcin']    = sbpcl.bminus
         thermo['sb3cape']  = sbpcl.b3km
         thermo['sb6cape']  = sbpcl.b6km
 
         #--- MOST UNSTABLE PARCEL PROPERTIES ---#
         # ---------------------------------------------------------------
@@ -203,14 +227,15 @@
         thermo['mu_lcl_p'] = mupcl.lclpres 
         thermo['mu_lcl_z'] = mupcl.lclhght 
         thermo['mu_lfc_p'] = mupcl.lfcpres 
         thermo['mu_lfc_z'] = mupcl.lfchght
         thermo['mu_el_p']  = mupcl.elpres
         thermo['mu_el_z']  = mupcl.elhght
         thermo['mu_el_T']  = temp(prof, pres(prof, thermo['mu_el_z']))
+        thermo['mu_mpl_p'] = mupcl.mplpres
         thermo['mucape']   = mupcl.bplus
         thermo['mucin']    = mupcl.bminus
         thermo['mu3cape']  = mupcl.b3km
         thermo['mu6cape']  = mupcl.b6km
 
         #--- MIXED LAYER PARCEL PROPERTIES ---#
         # ---------------------------------------------------------------
@@ -222,14 +247,15 @@
         thermo['ml_lcl_p'] = mlpcl.lclpres
         thermo['ml_lcl_z'] = mlpcl.lclhght
         thermo['ml_lfc_p'] = mlpcl.lfcpres
         thermo['ml_lfc_z'] = mlpcl.lfchght
         thermo['ml_el_p']  = mlpcl.elpres
         thermo['ml_el_z']  = mlpcl.elhght
         thermo['ml_el_T']  = temp(prof, pres(prof, thermo['ml_el_z']))
+        thermo['ml_mpl_p'] = mlpcl.mplpres
         thermo['mlcape']   = mlpcl.bplus
         thermo['mlcin']    = mlpcl.bminus
         thermo['ml3cape']  = mlpcl.b3km
         thermo['ml6cape']  = mlpcl.b6km
 
         #--- NORMALIZED CAPE ---#
         # ---------------------------------------------------------------
@@ -268,28 +294,30 @@
         thermo['lr_03km'] = lapse_rate(prof, 0, 3000, pres=False) 
         thermo['lr_max']  = max_lapse_rate(prof, lower=0, upper=6000, 
                                          interval=250, depth=2000)
         
         #--- TEMPERATURE ADVECTION ---#
         # ---------------------------------------------------------------
         #returns temp_adv (C/hr) array and 2D array of top and bottom bounds of temp advection layer (mb)
-        thermo['temp_adv'] = inferred_temp_adv(prof, lat=self.clean_data['site_info']['site-latlon'][0])
+        thermo['temp_adv'] = inferred_temp_adv(prof, lat=sounding_data['site_info']['site-latlon'][0])
         ####################################################################
         
         
 
 
 
         ####################################################################
         ### KINEMATIC VALUES ###
         ####################################################################
         #--- LAPSE RATES ---#
         # ---------------------------------------------------------------   
-        kinem['eil'] = effective_inflow_layer(prof, ecape=100, ecinh=- 250)
+        kinem['eil'] = effective_inflow_layer(prof, ecape=100, ecinh=-50)
         kinem['eil_z'] = [to_agl(prof, hght(prof, kinem['eil'][0])), to_agl(prof, hght(prof, kinem['eil'][1]))]
+        
+        eil_idx = [find_nearest(intrp['zINTRP'], kinem['eil_z'][0]), find_nearest(intrp['zINTRP'], kinem['eil_z'][1])]
 
         #--- STORM MOTION ---#
         # ---------------------------------------------------------------   
         sm_rm = bunkers_storm_motion(prof)[0:2] 
         sm_lm = bunkers_storm_motion(prof)[2:4] 
         sm_mw = mean_wind(prof, pbot=850, ptop=250)
 
@@ -360,65 +388,74 @@
         p9km = pres(prof, to_msl(prof, 9000.))
 
         shear_0_to_500  = wind_shear(prof, pbot=sfc, ptop=p500m)
         shear_0_to_1000 = wind_shear(prof, pbot=sfc, ptop=p1km)
         shear_1_to_3000 = wind_shear(prof, pbot=p1km, ptop=p3km)
         shear_3_to_6000 = wind_shear(prof, pbot=p3km, ptop=p6km)
         shear_6_to_9000 = wind_shear(prof, pbot=p6km, ptop=p9km)
+        shear_eil       = wind_shear(prof, pbot=kinem['eil'][0], ptop=kinem['eil'][1])
 
         kinem['shear_0_to_500']  = comp2vec(shear_0_to_500[0], shear_0_to_500[1])[1]
         kinem['shear_0_to_1000'] = comp2vec(shear_0_to_1000[0], shear_0_to_1000[1])[1]
         kinem['shear_1_to_3000'] = comp2vec(shear_1_to_3000[0], shear_1_to_3000[1])[1]
         kinem['shear_3_to_6000'] = comp2vec(shear_3_to_6000[0], shear_3_to_6000[1])[1]
         kinem['shear_6_to_9000'] = comp2vec(shear_6_to_9000[0], shear_6_to_9000[1])[1]
+        kinem['shear_eil'] = comp2vec(shear_eil[0], shear_eil[1])[1]
             
         #--- SRH ---#
         # ---------------------------------------------------------------
         if ma.is_masked(kinem['sm_u']) == False:
-            kinem['srh_0_to_500']  = helicity(prof, 0, 500.,     stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
-            kinem['srh_0_to_1000'] = helicity(prof, 0, 1000.,    stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
-            kinem['srh_1_to_3000'] = helicity(prof, 1000, 3000., stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
-            kinem['srh_3_to_6000'] = helicity(prof, 3000, 6000., stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
-            kinem['srh_6_to_9000'] = helicity(prof, 6000, 9000., stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
+            
+            keys = ['srh_0_to_500', 'srh_0_to_1000', 'srh_1_to_3000', 'srh_3_to_6000', 'srh_6_to_9000', 'srh_eil']
+            lwrs = [0, 0, 1000, 3000, 6000, kinem['eil_z'][0]]
+            uprs = [500, 1000, 3000, 6000, 9000, kinem['eil_z'][1]]
+            
+            for key, lwr, upr in zip(keys, lwrs, uprs):
+                try:
+                    kinem[key]  = helicity(prof, lwr, upr, stu = kinem['sm_u'], stv = kinem['sm_v'])[0]
+                except:
+                    kinem[key] = ma.masked
+                    pass
         else:
             kinem['srh_0_to_500']  = ma.masked
             kinem['srh_0_to_1000'] = ma.masked
             kinem['srh_1_to_3000'] = ma.masked
             kinem['srh_3_to_6000'] = ma.masked
             kinem['srh_6_to_9000'] = ma.masked
+            kinem['srh_6_to_9000'] = ma.masked
+            kinem['srh_eil'] = ma.masked
             warnings.warn("Storm Relative Helicity could not be computed for this sounding (no valid storm motion)", Warning)
 
 
         #--- SRW LAYERS ---#
         # --------------------------------------------------------------- 
         if ma.is_masked(kinem['sm_u']) == False:
             def calc_srw_layer(prof, level):
                 u, v = components(prof, p=pres(prof, to_msl(prof, level)))
                 sru = u - kinem['sm_u']
                 srv = v - kinem['sm_v']
                 return mpcalc.wind_speed(sru*units.kts, srv*units.kts)
-            try:
-                kinem['srw_0_to_500']  = (calc_srw_layer(prof, 500)  + calc_srw_layer(prof, 0))/2
-                kinem['srw_0_to_1000'] = (calc_srw_layer(prof, 1000) + calc_srw_layer(prof, 0))/2
-                kinem['srw_1_to_3000'] = (calc_srw_layer(prof, 3000) + calc_srw_layer(prof, 1000))/2
-                kinem['srw_3_to_6000'] = (calc_srw_layer(prof, 6000) + calc_srw_layer(prof, 3000))/2
-                kinem['srw_6_to_9000'] = (calc_srw_layer(prof, 9000) + calc_srw_layer(prof, 6000))/2
-            except:
-                kinem['srw_0_to_500']  = ma.masked
-                kinem['srw_0_to_1000'] = ma.masked
-                kinem['srw_1_to_3000'] = ma.masked
-                kinem['srw_3_to_6000'] = ma.masked
-                kinem['srw_6_to_9000'] = ma.masked
-                pass
+            
+            keys = ['srw_0_to_500', 'srw_0_to_1000', 'srw_1_to_3000', 'srw_3_to_6000', 'srw_6_to_9000', 'srw_eil']
+            lwrs = [0, 0, 1000, 3000, 6000, kinem['eil_z'][0]]
+            uprs = [500, 1000, 3000, 6000, 9000, kinem['eil_z'][1]]
+            
+            for key, lwr, upr in zip(keys, lwrs, uprs):
+                try:
+                    kinem[key] = (calc_srw_layer(prof, upr)  + calc_srw_layer(prof, lwr))/2
+                except:
+                    kinem[key] = ma.masked
+                    pass
         else:
             kinem['srw_0_to_500']  = ma.masked
             kinem['srw_0_to_1000'] = ma.masked
             kinem['srw_1_to_3000'] = ma.masked
             kinem['srw_3_to_6000'] = ma.masked
             kinem['srw_6_to_9000'] = ma.masked
+            kinem['srw_eil'] = ma.masked
             warnings.warn("Storm Relative Wind could not be computed for this sounding (no valid storm motion)", Warning)
             
         #--- SRV ---#
         # ---------------------------------------------------------------
         # adopted from Sam Brandt (2022)    
         if ma.is_masked(kinem['sm_u']) == False: 
             # CONVERT TO m/s (uses `sm_u, sm_v` calculated above)
@@ -453,34 +490,38 @@
 
             # layer average streamwiseness and total streamwise vorticity
             kinem['swv_perc_0_to_500']  = np.mean(kinem['swv_perc'][0:5])
             kinem['swv_perc_0_to_1000'] = np.mean(kinem['swv_perc'][0:10])
             kinem['swv_perc_1_to_3000'] = np.mean(kinem['swv_perc'][10:30])
             kinem['swv_perc_3_to_6000'] = np.mean(kinem['swv_perc'][30:60])
             kinem['swv_perc_6_to_9000'] = np.mean(kinem['swv_perc'][60:90])
+            kinem['swv_perc_eil']       = np.mean(kinem['swv_perc'][eil_idx[0]:eil_idx[1]])
             kinem['swv_0_to_500']       = np.mean(kinem['swv'][0:5])
             kinem['swv_0_to_1000']      = np.mean(kinem['swv'][0:10])
             kinem['swv_1_to_3000']      = np.mean(kinem['swv'][10:30])
             kinem['swv_3_to_6000']      = np.mean(kinem['swv'][30:60])
             kinem['swv_6_to_9000']      = np.mean(kinem['swv'][60:90])
+            kinem['swv_eil']            = np.mean(kinem['swv'][eil_idx[0]:eil_idx[1]])
         else:
             kinem['srw']                = ma.masked
             kinem['swv']                = ma.masked
             kinem['swv_perc']           = ma.masked
             kinem['vort']               = ma.masked
             kinem['swv_perc_0_to_500']  = ma.masked
             kinem['swv_perc_0_to_1000'] = ma.masked
             kinem['swv_perc_1_to_3000'] = ma.masked
             kinem['swv_perc_3_to_6000'] = ma.masked
             kinem['swv_perc_6_to_9000'] = ma.masked
+            kinem['swv_perc_eil']       = ma.masked
             kinem['swv_0_to_500']       = ma.masked
             kinem['swv_0_to_1000']      = ma.masked
             kinem['swv_1_to_3000']      = ma.masked
             kinem['swv_3_to_6000']      = ma.masked
             kinem['swv_6_to_9000']      = ma.masked
+            kinem['swv_eil']            = ma.masked
             warnings.warn("Streamwise Vorticity could not be computed for this sounding (no valid storm motion)", Warning)
         
         
         #--- SIMPLE ENTRAINING CAPE ---#
         # ---------------------------------------------------------------
         try: 
             thermo['mu_ecape'] = calc_ecape(z, p, T, general['spec_humidity'], u, v, 'most_unstable', storm_motion='user_defined', u_sm=kinem['sm_u']*units.kts, v_sm=kinem['sm_v']*units.kts).m
@@ -544,24 +585,27 @@
 
 
 
 
 
 
 
+        
+        
 
 
 
 # VAD Profile Calc functions 
 
 class vad_params:
     
-    def __init__(self, vad_data, storm_motion='right_moving'):
+    def __init__(self, vad_data, storm_motion='right_moving', modify_sfc=None):
             self.vad_data = vad_data 
             self.storm_motion = storm_motion
+            self.modify_sfc = modify_sfc
             
     
     ######################################################################################################
     ### CALC FUNCTION -- COMPUTE VALUES ###
     ######################################################################################################        
     def calc(self):
     
@@ -651,24 +695,24 @@
               shrmag = np.hypot(u_shr, v_shr)
               return shrmag
 
         
         # CALC MEAN_WIND COMPONENTS 
         def calc_meanwind(u_layer, v_layer, z, top):
               layer_top = np.where(z == (top))[0][0]
-              mean_u = np.mean(u_layer[:layer_top])
-              mean_v = np.mean(v_layer[:layer_top])
+              mean_u = np.nanmean(u_layer[:layer_top])
+              mean_v = np.nanmean(v_layer[:layer_top])
               return mean_u, mean_v
 
         
         # CALC BUNKERS STORM MOTION
         def calc_bunkers(u_layer, v_layer, z):
               layer_top = np.where(z == (6000))[0][0]
-              mean_u = np.mean(u_layer[:layer_top])
-              mean_v = np.mean(v_layer[:layer_top])
+              mean_u = np.nanmean(u_layer[:layer_top])
+              mean_v = np.nanmean(v_layer[:layer_top])
 
               layer_top = np.where(z == (6000))[0][0]
               u_shr = u_layer[layer_top] - u_layer[0]
               v_shr = v_layer[layer_top] - v_layer[0]
 
               dev = 7.5 * 1.94
 
@@ -710,15 +754,15 @@
         def calc_srh(u_comp, v_comp, z, depth, bottom, storm_u, storm_v):
             srh = mpcalc.storm_relative_helicity(height=z, u=u_comp, v=v_comp, depth=depth,
                                            bottom=bottom, storm_u=storm_u, storm_v=storm_v)[0]
             return srh.m
                 
             
         # CALC STORM RELATIVE WIND 
-        def calc_srw_layer(u, v, bottom, top):
+        def calc_srw_layer(u, v, bottom, top, z):
             layer_top = np.where(z == (top))[0][0]
             layer_bot = np.where(z == (bottom))[0][0]
             
             top_sru = u[layer_top] - kinem['sm_u']
             top_srv = v[layer_top] - kinem['sm_v']
             
             bot_sru = u[layer_bot] - kinem['sm_u']
@@ -729,17 +773,17 @@
             return mean_srw.m
         
                 
         
             
         #--- BUNKERS STORM MOTION ---#
         # --------------------------------------------------------------- 
-        kinem['sm_rm'] = calc_bunkers(u, v, z)[0:2]
-        kinem['sm_lm'] = calc_bunkers(u, v, z)[2:4]
-        kinem['sm_mw'] = calc_meanwind(u, v, z, 6000)
+        kinem['sm_rm'] = calc_bunkers(intrp['uINTRP'], intrp['vINTRP'], intrp['zINTRP'])[0:2]
+        kinem['sm_lm'] = calc_bunkers(intrp['uINTRP'], intrp['vINTRP'], intrp['zINTRP'])[2:4]
+        kinem['sm_mw'] = calc_meanwind(intrp['uINTRP'], intrp['vINTRP'], intrp['zINTRP'], 6000)
        
         
         #--- USER DEFINED SM PT ---#
         # ---------------------------------------------------------------  
         if str(type(self.storm_motion)) == "<class 'list'>":
             kinem['sm_u'], kinem['sm_v'] = mpcalc.wind_components(self.storm_motion[1]*units.kts, self.storm_motion[0]*units.deg)
             kinem['sm_u'], kinem['sm_v'] = kinem['sm_u'].m, kinem['sm_v'].m
@@ -764,55 +808,55 @@
                 kinem['sm_v'] = ma.masked
                 
                 
                 
         #--- DEVIANT TORNADO MOTION ---#
         # --------------------------------------------------------------- 
         if ma.is_masked(kinem['sm_u']) == False:
-            mw_u_300, mw_v_300 = calc_meanwind(u, v, z, 300)
+            mw_u_300, mw_v_300 = calc_meanwind(intrp['uINTRP'],intrp['vINTRP'],intrp['zINTRP'], 300)
             kinem['dtm'] = ((kinem['sm_u']+mw_u_300)/2, (kinem['sm_v']+mw_v_300)/2)
         else:
             kinem['dtm'] = ma.masked
           
         
         
         #--- CORFIDI MSC MOTION ---#
         #----------------------------------------------------------------
-        kinem['mcs'] = calc_corfidi(u, v, z, 
-                                    calc_meanwind(u, v, z, 6000)[0],
-                                    calc_meanwind(u, v, z, 6000)[1])
+        kinem['mcs'] = calc_corfidi(intrp['uINTRP'],intrp['vINTRP'],intrp['zINTRP'],
+                                    calc_meanwind(intrp['uINTRP'],intrp['vINTRP'],intrp['zINTRP'], 6000)[0],
+                                    calc_meanwind(intrp['uINTRP'],intrp['vINTRP'],intrp['zINTRP'], 6000)[1])
 
 
         
         #--- BULK SHEAR ---#
         # ---------------------------------------------------------------  
-        kinem['shear_0_to_500']  = calc_shear(u, v, 0, 500, z)
-        kinem['shear_0_to_1000'] = calc_shear(u, v, 0, 1000, z)
-        kinem['shear_1_to_3000'] = calc_shear(u, v, 1000, 3000, z)
-        kinem['shear_3_to_6000'] = calc_shear(u, v, 3000, 6000, z)
-        kinem['shear_6_to_9000'] = calc_shear(u, v, 6000, 9000, z)
+        kinem['shear_0_to_500']  = calc_shear(intrp['uINTRP'],intrp['vINTRP'], 0, 500, intrp['zINTRP'])
+        kinem['shear_0_to_1000'] = calc_shear(intrp['uINTRP'],intrp['vINTRP'], 0, 1000, intrp['zINTRP'])
+        kinem['shear_1_to_3000'] = calc_shear(intrp['uINTRP'],intrp['vINTRP'], 1000, 3000, intrp['zINTRP'])
+        kinem['shear_3_to_6000'] = calc_shear(intrp['uINTRP'],intrp['vINTRP'], 3000, 6000, intrp['zINTRP'])
+        kinem['shear_6_to_9000'] = calc_shear(intrp['uINTRP'],intrp['vINTRP'], 6000, 9000, intrp['zINTRP'])
             
             
             
         #--- SRH ---#
         # ---------------------------------------------------------------
         if ma.is_masked(kinem['sm_u']) == False:
-            kinem['srh_0_to_500']  = calc_srh(u_comp=u*units.kts, v_comp=v*units.kts, z=z*units.m, 
+            kinem['srh_0_to_500']  = calc_srh(u_comp=intrp['uINTRP']*units.kts, v_comp=intrp['vINTRP']*units.kts, z=intrp['zINTRP']*units.m, 
                                               bottom=None, depth=500*units.m,  
                                               storm_u=kinem['sm_u']*units.kts, storm_v=kinem['sm_v']*units.kts)
-            kinem['srh_0_to_1000'] = calc_srh(u_comp=u*units.kts, v_comp=v*units.kts, z=z*units.m, 
+            kinem['srh_0_to_1000'] = calc_srh(u_comp=intrp['uINTRP']*units.kts, v_comp=intrp['vINTRP']*units.kts, z=intrp['zINTRP']*units.m, 
                                               bottom=None, depth=1000*units.m, 
                                               storm_u=kinem['sm_u']*units.kts, storm_v=kinem['sm_v']*units.kts)
-            kinem['srh_1_to_3000'] = calc_srh(u_comp=u*units.kts, v_comp=v*units.kts, z=z*units.m, 
+            kinem['srh_1_to_3000'] = calc_srh(u_comp=intrp['uINTRP']*units.kts, v_comp=intrp['vINTRP']*units.kts, z=intrp['zINTRP']*units.m, 
                                               bottom=1000*units.m, depth=3000*units.m, 
                                               storm_u=kinem['sm_u']*units.kts, storm_v=kinem['sm_v']*units.kts)
-            kinem['srh_3_to_6000'] = calc_srh(u_comp=u*units.kts, v_comp=v*units.kts, z=z*units.m, 
+            kinem['srh_3_to_6000'] = calc_srh(u_comp=intrp['uINTRP']*units.kts, v_comp=intrp['vINTRP']*units.kts, z=intrp['zINTRP']*units.m, 
                                               bottom=3000*units.m, depth=6000*units.m, 
                                               storm_u=kinem['sm_u']*units.kts, storm_v=kinem['sm_v']*units.kts)
-            kinem['srh_6_to_9000'] = calc_srh(u_comp=u*units.kts, v_comp=v*units.kts, z=z*units.m, 
+            kinem['srh_6_to_9000'] = calc_srh(u_comp=intrp['uINTRP']*units.kts, v_comp=intrp['vINTRP']*units.kts, z=intrp['zINTRP']*units.m, 
                                               bottom=6000*units.m, depth=9000*units.m, 
                                               storm_u=kinem['sm_u']*units.kts, storm_v=kinem['sm_v']*units.kts)
         else:
             kinem['srh_0_to_500']  = ma.masked
             kinem['srh_0_to_1000'] = ma.masked
             kinem['srh_1_to_3000'] = ma.masked
             kinem['srh_3_to_6000'] = ma.masked
@@ -820,19 +864,19 @@
             warnings.warn("Storm Relative Helicity could not be computed for this sounding (no valid storm motion)", Warning)
 
 
             
         #--- SRW LAYERS ---#
         # --------------------------------------------------------------- 
         if ma.is_masked(kinem['sm_u']) == False:
-            kinem['srw_0_to_500']  = calc_srw_layer(u, v, 0, 500)
-            kinem['srw_0_to_1000'] = calc_srw_layer(u, v, 0, 1000)
-            kinem['srw_1_to_3000'] = calc_srw_layer(u, v, 1000, 3000)
-            kinem['srw_3_to_6000'] = calc_srw_layer(u, v, 3000, 6000)
-            kinem['srw_6_to_9000'] = calc_srw_layer(u, v, 6000, 9000)
+            kinem['srw_0_to_500']  = calc_srw_layer(intrp['uINTRP'],intrp['vINTRP'], 0, 500, intrp['zINTRP'])
+            kinem['srw_0_to_1000'] = calc_srw_layer(intrp['uINTRP'],intrp['vINTRP'], 0, 1000, intrp['zINTRP'])
+            kinem['srw_1_to_3000'] = calc_srw_layer(intrp['uINTRP'],intrp['vINTRP'], 1000, 3000, intrp['zINTRP'])
+            kinem['srw_3_to_6000'] = calc_srw_layer(intrp['uINTRP'],intrp['vINTRP'], 3000, 6000, intrp['zINTRP'])
+            kinem['srw_6_to_9000'] = calc_srw_layer(intrp['uINTRP'],intrp['vINTRP'], 6000, 9000, intrp['zINTRP'])
 
         
         
         #--- SRV ---#
         # ---------------------------------------------------------------
         # adopted from Sam Brandt (2022)    
         if ma.is_masked(kinem['sm_u']) == False:
```

### Comparing `sounderpy-3.0.3/src/sounderpy/plot.py` & `sounderpy-3.0.4.dev1/src/sounderpy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,138 +1,289 @@
+# METPY OPERATIONS 
 import metpy.calc as mpcalc
 from metpy.units import units
-from metpy.plots import SkewT, Hodograph
+from metpy.plots import SkewT, Hodograph, USCOUNTIES
 
+#MATPLOTLIB OPERATIONS
 import matplotlib.lines    as mlines
 import matplotlib.pyplot as plt
 import matplotlib.transforms as mtransforms
 import matplotlib.colors as mcolors
 
+# NUMPY OPERATIONS 
 import numpy as np
 import numpy.ma as ma
+import copy
 
-from urllib.request import urlopen
-from PIL import Image
+# STANDARD PYTHON
 import warnings
 import time
+from datetime import datetime
+
+# ECAPE
+from ecape_parcel.calc import calc_ecape_parcel, density_temperature
+
+# FOR MAPPING
+from urllib.request import urlopen
+from PIL import Image
+import cartopy.crs as ccrs
+import cartopy.feature as cfeature
+import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+from cartopy.io.shapereader import Reader
+from cartopy.feature import ShapelyFeature
+
+# DATA RETRIEVAL
+from xarray.backends import NetCDF4DataStore
+from xarray import open_dataset
+from siphon.catalog import TDSCatalog
+from netCDF4 import Dataset
+from matplotlib.colors import LinearSegmentedColormap
 
+# SOUNDERPY MODULES
 from .calc import *
 
-from ecape_parcel.calc import calc_ecape_parcel, density_temperature
 
-#########################################################
-#            SOUNDERPY SPYPLOT FUNCTIONS                #
-# (C) KYLE J GILLETT, CENTRAL MICHIGAN UNIVERSTIY, 2024 #
-#########################################################
+
+
+########################################################
+#            SOUNDERPY SPYPLOT FUNCTIONS               #
+# (C) KYLE J GILLETT, UNIVERSITY OF NORTH DAKOTA, 2024 #
+########################################################
 
 
 
 #########################################################################
 ########################## FULL SOUNDING ################################
 
+def __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels=None, 
+                    show_radar=True, radar_time='sounding', map_zoom=2, modify_sfc=None):
+    
+    
+    # record process time 
+    st = time.time()  
+
+    
+    # make text prettier
+    # magnitude number text 
+    def mag(param):
+        if ma.is_masked(param):
+            fixed = '---'
+        else:
+            try:
+                fixed = int(param.m)
+            except:
+                try: 
+                    fixed = int(param)
+                except: fixed = param
+        return fixed
+    
+    
+    # make text prettier
+    # magnitude and round number text
+    def mag_round(param, dec, mag=False):
+        if ma.is_masked(param):
+            fixed = '---'
+        elif mag == True:
+            fixed = np.round(param.m, dec)
+        else:
+            fixed = np.round(param, dec)
+        return fixed
+
+    
+    # find nearest value in array
+    def find_nearest(array, value):
+        array = np.asarray(array)
+        nearest_idx = (np.abs(array - value)).argmin()
+        return nearest_idx
+    
+    
+    # get radar mosaic data for map inset
+    def get_radar_mosaic(clean_data, map_zoom, radar_time):
+        '''
+        GET RADAR MOSAIC DATA FOR SOUNDING PLOT
+        
+        - gets data from NCEI for 'sounding time' or now
+        - data only goes back 1 month from current time
+        '''
+    
+        # search the NCEI database for the file closest to 
+        # the requested radar date/time
+        def find_file(target_time, file_names):
+            closest_index = None
+            closest_difference = float('inf')
+
+            for idx, file_name in enumerate(file_names):
+                # Extract the final component (ex: "1220") from the file name
+                components = file_name.split('_')
+                if len(components) > 1:
+                    # Remove file extension if present
+                    last_component = components[-1].split('.')[0]
+                    try:
+                        file_time = int(last_component)
+                        # Convert the target_time to an integer for comparison
+                        target_time_int = int(target_time)
+                        difference = abs(file_time - target_time_int)
+                        if difference < closest_difference:
+                            closest_difference = difference
+                            closest_index = idx
+                    except ValueError:
+                        pass  # Skip if the last component is not a valid integer
+
+            return closest_index
+
+
+        # PREFORM DATETIME OPERATIONS------------------------------------------------------------------------
+        # get sounding data from from clean_data
+        data_dt = datetime(int(clean_data['site_info']['valid-time'][0]), int(clean_data['site_info']['valid-time'][1]), 
+             int(clean_data['site_info']['valid-time'][2]), int(clean_data['site_info']['valid-time'][3][0:2]))
+
+        # get current time
+        curr_dt = datetime.utcnow()
+
+        # if data time is after current time, default to now
+        if data_dt > curr_dt:
+            time = curr_dt.strftime('%H%M')
+            datestr = curr_dt.strftime('%Y%m%d')
+        
+        # if radar time is given as now, time is now
+        elif radar_time == 'now':
+            time = curr_dt.strftime('%H%M')
+            datestr = curr_dt.strftime('%Y%m%d')
+
+        # if radar time is given as sounding, use the valid-time info from clean_data
+        elif radar_time == 'sounding':
+            if len(clean_data['site_info']['valid-time'][3]) == 2:
+                time = f"{clean_data['site_info']['valid-time'][3]}00"
+            else:
+                time = clean_data['site_info']['valid-time'][3]
+            datestr = data_dt.strftime('%Y%m%d')
+
 
-def __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels=None):
+        # PULL SOUNDING DATA LAT/LON ----------------------------------------------------------------------
+        data_lat = clean_data['site_info']['site-latlon'][0]
+        data_lon = clean_data['site_info']['site-latlon'][1]
 
 
+        # GET RADAR DATA ----------------------------------------------------------------------------------
+        composite_url = 'https://thredds.ucar.edu/thredds/catalog/nexrad/composite/gini/dhr/1km/'+datestr+'/catalog.xml'
+        try:
+            # try accessing the NCEI TDS database
+            composite_catalog = TDSCatalog(composite_url).datasets
+            data_found = True
+        except:
+            # no data is available, return no data
+            print('- no radar data available -')
+            data_found = False
+            pass
         
+        if data_found == True:
+            # if data is foudn, parse it for plotting.
+            filename = composite_catalog[find_file(time, composite_catalog)].subset()
+            composite_query = filename.query()
+            composite_query.lonlat_box(north = data_lat + (map_zoom + 1),
+                             south = data_lat - (map_zoom + 1),
+                             east  = data_lon + (map_zoom + 1),
+                             west  = data_lon - (map_zoom + 1))
+            composite_query.add_lonlat(value=True)
+            composite_query.accept('netcdf4')
+            composite_query.variables('Reflectivity')
+            radar_data = filename.get_data(composite_query)
+            radar_data = open_dataset(NetCDF4DataStore(radar_data))
+
+            return radar_data
         
+    # define display mode colors and alphas    
     if dark_mode == True:
         gen_txt_clr = 'white'
         bckgrnd_clr = 'black'
         brdr_clr    = 'white'
         barb_clr    = 'white'
         shade_alpha = 0.06
         skw_ln_clr = 'white'
+        marker_clr = 'white'
     else: 
         gen_txt_clr = 'black'
         bckgrnd_clr = 'white'
         brdr_clr    = 'black'
         barb_clr    = 'black'
         shade_alpha = 0.02
         skw_ln_clr = 'black'
-    
-    # record process time 
-    st = time.time()  
+        marker_clr = 'black'
 
-    def find_nearest(array, value):
-        array = np.asarray(array)
-        nearest_idx = (np.abs(array - value)).argmin()
-        return nearest_idx
-    
+
+    # define colorblindness colors
     if color_blind == True:
         td_color = 'cornflowerblue'
     else:
         td_color = 'green'
         
-    hodo_color = ['purple','red','darkorange','gold','#fff09f'] 
-    
-    def mag(param):
-        if ma.is_masked(param):
-            fixed = '---'
-        else:
-            try:
-                fixed = int(param.m)
-            except:
-                try: 
-                    fixed = int(param)
-                except: fixed = param
-        return fixed
     
-    def mag_round(param, dec):
-        if ma.is_masked(param):
-            fixed = '---'
-        else:
-            fixed = np.round(param, dec)
-        return fixed
-
 
     #################################################################
     ### SET UP THE DATA ###
     #################################################################
+    # SFC CORRECTION
+    # create a deepcopy of clean_data
+    sounding_data = copy.deepcopy(clean_data)
+    
+    # if `sfc_correction` is a list, correct the sfc values
+    modify_sfc_txt = False 
+    if str(type(modify_sfc)) == "<class 'list'>":
+        sounding_data['T'][0] = modify_sfc[0]*units.degC
+        sounding_data['Td'][0] = modify_sfc[1]*units.degC
+        # add 'user corrected sfc' txt
+        modify_sfc_txt = True
+    
     # declare easy variable names for reuse from `clean_data` 
-    T  = clean_data['T']
-    Td = clean_data['Td']
-    p  = clean_data['p']
-    z  = clean_data['z']
-    u  = clean_data['u']
-    v  = clean_data['v']
+    T  = sounding_data['T']
+    Td = sounding_data['Td']
+    p  = sounding_data['p']
+    z  = sounding_data['z']
+    u  = sounding_data['u']
+    v  = sounding_data['v']
     wd = mpcalc.wind_direction(u, v)
     ws = mpcalc.wind_speed(u, v) 
     
     # calculate other sounding parameters using SounderPy Calc
-    general, thermo, kinem, intrp = sounding_params(clean_data, storm_motion).calc()
+    general, thermo, kinem, intrp = sounding_params(sounding_data, storm_motion).calc()
     #################################################################
     
     
     
     #################################################################
     ### DETERMINE PLOT TITLE BASED ON THE DATA ###
     #################################################################
     
     if 'ACARS' in clean_data['site_info']['source']:
+        # title specific to ACARS
         top_title = f"ACARS AIRCRAFT OBSERVATION VERTICAL PROFILE"
         left_title = f"VALID: {clean_data['site_info']['valid-time'][1]}-{clean_data['site_info']['valid-time'][2]}-{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z"
-        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
+        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']}, {clean_data['site_info']['site-lctn']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
 
     elif 'BUFKIT' in clean_data['site_info']['source']:
+        # title specific to bufkit
         top_title = f"BUFKIT MODEL FORECAST PROFILE | {clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']}"
         left_title = f" VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z"
-        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
+        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']}, {clean_data['site_info']['site-lctn']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
 
     elif 'RAOB' in clean_data['site_info']['source']:
+        # title specific to RAOB Obs
         top_title = "RAOB OBSERVED VERTICAL PROFILE"
         left_title = f"VALID: {clean_data['site_info']['valid-time'][1]}-{clean_data['site_info']['valid-time'][2]}-{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z"
-        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
+        right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']}, {clean_data['site_info']['site-lctn']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
 
     elif 'REANALYSIS' in clean_data['site_info']['source']:
+        # title spcific to reanalysis data
         top_title = f"{clean_data['site_info']['source']} VERTICAL PROFILE | {clean_data['site_info']['valid-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']}"
         left_title = f"{clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z"
         right_title = f"{clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]} | {clean_data['site_info']['box_area']}    " 
         
     else:
+        # title for other data
         top_title = clean_data['site_info']['source']
         left_title = f"VALID: {clean_data['site_info']['valid-time'][1]}-{clean_data['site_info']['valid-time'][2]}-{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z"
         right_title = f"{clean_data['site_info']['site-id']} - {clean_data['site_info']['site-name']} | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}    " 
         
     ################################################################    
         
     
@@ -142,40 +293,42 @@
     
     
     
     #################################################################
     ### CREATE FIGURE ###
     #################################################################
     #################################################################
-    # Define figure and skew-t
-    fig = plt.figure(figsize=(22,13), linewidth=10, edgecolor=brdr_clr)          # create figure                                   # create figure
+    # create master figure
+    fig = plt.figure(figsize=(22,13), linewidth=10, edgecolor=brdr_clr)         
+    # create skew-t obj and axes params
     skew = SkewT(fig, rotation=47, rect=(0.1124, 0.1005, 0.60, 0.85))  
     skew.ax.set_box_aspect(0.87)
     skew.ax.zorder = 5
-    # Define axis bounds 
+    # Define axis bounds, temp axis based on data
     skew.ax.set_adjustable('datalim')
     skew.ax.set_ylim(1050, 100)    
     if T[0].m <= -10:
         bounds = [-42, 42]
         if T[0].m <= -20:
             bounds = [-52, 32]
     elif T[0].m >= 20:
         bounds = [-22, 62]
     else: 
         bounds = [-32, 52]
     skew.ax.set_xlim(bounds[0], bounds[1])   
-    # Define axis labels 
+    # Define and customize axis labels 
     plt.xlabel("  ", fontsize=12)
     plt.ylabel("  ", fontsize=12) 
-    plt.xticks(fontsize=13)  
-    plt.yticks(fontsize=13, ha='left')
-    plt.tick_params(axis="x",direction="in", pad=-12, colors=gen_txt_clr)
-    plt.tick_params(axis="y",direction="in", pad=-7, colors=gen_txt_clr)
+    plt.xticks(fontsize=13, weight='bold')  
+    plt.yticks(fontsize=13, ha='left', weight='bold')
+    plt.tick_params(axis="x", direction="in", pad=-12, colors=gen_txt_clr)
+    plt.tick_params(axis="y", direction="in", pad=-7, colors=gen_txt_clr)
     skew.ax.set_yticks([1000, 900, 800, 700, 600, 500, 400, 300, 200])
     skew.ax.set_yticklabels([1000, 900, 800, 700, 600, 500, 400, 300, 200], color=gen_txt_clr)
+    # add skew-t axis spines
     skew.ax.spines["top"].set_color(brdr_clr)
     skew.ax.spines["left"].set_color(brdr_clr)
     skew.ax.spines["right"].set_color(brdr_clr)
     skew.ax.spines["bottom"].set_color(brdr_clr)
     skew.ax.spines["bottom"].set_color(brdr_clr)
     # Define background colors
     fig.set_facecolor(bckgrnd_clr)         
@@ -190,30 +343,42 @@
     
     
     
     #################################################################
     ### PLOT SKEW T LINES ###
     #################################################################
     # Plot relevent Skew-T lines
+    # 0C and -20C highlights
     skew.ax.axvline(0 * units.degC, linestyle='--', color='blue', alpha=0.3)
     skew.ax.axvline(-20 * units.degC, linestyle='--', color='blue', alpha=0.3)
-    skew.plot_dry_adiabats(color=skw_ln_clr, linewidth=0.5, alpha=0.7)   
-    skew.plot_moist_adiabats(color=skw_ln_clr, linewidth=0.5, alpha=0.7)
+    # dry adiabats
+    skew.plot_dry_adiabats(color='cornflowerblue', linewidth=0.2, alpha=0.7) 
+    # moist adiabats
+    skew.plot_moist_adiabats(color='cornflowerblue', linewidth=0.2, alpha=0.7)
+    # mixing ratio lines
     skew.plot_mixing_lines(color=skw_ln_clr, linewidth=0.2, alpha=0.7)
-    # add basic temperature lines
-    twline = skew.plot(p, general['wet_bulb'], '#3d8aff', linewidth=1, label='WETBULB TEMP', alpha=0.3)
-    #tvline = skew.plot(p, general['virt_temp'], 'red', linestyle='--', linewidth=3, label='VIRTUAL TEMP', alpha=0.6)  
+    # wet bulb temp (Tw)
+    twline = skew.plot(p, general['wet_bulb'], '#3d8aff', linewidth=2, label='WETBULB TEMP', alpha=0.6)
+    # virtual temp (Tv)
+    tvline = skew.plot(p, general['virt_temp'], 'darkred', linestyle=(0, (1, 1)), linewidth=4, label='VIRTUAL TEMP', alpha=0.7)  
+    # dewpoint temp (Td)
     tdline = skew.plot(p, Td, td_color, linewidth=5, label='DEWPOINT')
+    # temp (T)
     tline1 = skew.plot(p, T, 'red', linewidth=5, label='TEMPERATURE')  
 
     
     
     #################################################################
     ### PARCELS LOGIC ###
     #################################################################
+    '''
+    SounderPy 'Special Parcels Logic' using Amelia Urquhart’s ecape_parcels library: https://github.com/a-urq/ecape-parcel-py
+    
+    Docs: https://kylejgillett.github.io/sounderpy/plottingdata.html#parcel-logic
+    '''
     parcel_details = {
 
             'term1': {'sb': 'surface_based', 
                       'ml': 'mixed_layer', 
                       'mu': 'most_unstable',
                      },
             'term2': {'ps': [True,  'pseudoadiabatic'],
@@ -245,15 +410,15 @@
         parcel_dict = {}
 
         for parcel in all_parcels:
             
             if parcel not in valid_parcel_codes:
                     sys.exit(f"Invalid parcel code provided in 'special_parcels' kwarg. Please make sure parcel codes are one of these:\n{valid_parcel_codes}\n" +
                             "Valid parcel codes include the parcel type ('mu', 'sb', 'ml'), adiabatic scheme ('ps', 'ia'), and cape type ('cape', 'ecape').\n" +
-                            "See ####### DOCS LINK ########## for more info.")
+                            "See 'https://kylejgillett.github.io/sounderpy/plottingdata.html#parcel-logic' for more info.")
 
             # set vars to None 
             trace = None 
             trace_Trho = [None]
 
             # build parcel trace obj
             trace = calc_ecape_parcel(p, z, T, Td, u, v, 
@@ -271,25 +436,25 @@
                  trace = trace + (trace_Trho, ) 
 
 
             # add parcel data to the parcel_dict
             parcel_dict[parcel] = trace
 
 
-        # loop through the parcels agin to plot them  
+        # loop through the parcels again to plot them  
         for parcel in parcel_dict.keys():
 
             if len(parcel_dict[parcel]) == 6:
 
                 parcel_name = str.upper(f"{parcel.split('_')[0]} {parcel_details['term2'][parcel.split('_')[1]][1]} {parcel.split('_')[2]}")
-
+                # if parcel exists, plot it
                 if parcel in special_parcels[0]:
                             skew.plot(parcel_dict[parcel][0], parcel_dict[parcel][-1], color='red', linestyle='--',  
                                              linewidth=2, alpha=1, label=parcel_name)
-
+                # if parcel exists, plot it
                 elif parcel in special_parcels[1]:
                             skew.plot(parcel_dict[parcel][0], parcel_dict[parcel][-1], color='#808080', linestyle='--',  
                                              linewidth=2, alpha=0.5, label=parcel_name)
     
     
     
     
@@ -307,15 +472,25 @@
                                   storm_motion_u=kinem['sm_u']*units.kts, storm_motion_v=kinem['sm_v']*units.kts)
 
                 trace_Trho = density_temperature(trace[2], trace[3], trace[4])
 
                 muecapeline = skew.plot(trace[0], trace_Trho, 
                                         linestyle='--', linewidth=3, alpha=1, color='red',
                                         label='MUECAPE PARCEL')
+            
+#                 print(trace_Trho[0:len(T)].m-273.15)
+#                 return trace[0]
+                
+#                 skew.ax.fill_betweenx(p, T, trace_Trho[0:len(T)].m-273.15,
+#                                       color='red', alpha=0.1)
+                
+                #skew.shade_cape(p, T, np.linspace(trace_Trho[0], trace_Trho[-1], len(T)), color='red', alpha=0.4) 
+                #skew.shade_cape(p, T, mu_parcel_path, color='orange') 
         
+        # if CAPE for SB, MU, ML parcels is >0, plotm them
         if thermo['sbcape'] > 0:
             sbparcelline = skew.plot(thermo['sbP_trace'], thermo['sbT_trace'], 
                                      linestyle='--', linewidth=2, alpha=0.5, color='#808080', 
                                      label='SBCAPE PARCEL')    
         if thermo['mlcape'] > 0:
             mlparcelline = skew.plot(thermo['mlP_trace'], thermo['mlT_trace'],
                                      linestyle='--', linewidth=2, alpha=0.5, color='#808080',
@@ -329,99 +504,138 @@
     # ADD DOWNDRAFT PARCEL TRACE
     skew.plot(thermo['dparcel_p'], thermo['dparcel_T'], linestyle='--',linewidth=0.7, color='purple', 
               alpha=0.8, label='DWNDRFT PARCEL')
     
     
     #################################################################
     ### PLOT SKEW T ANNOTATIONS ###
-    #################################################################    
+    #################################################################  
+    #plot left side hgt level markers
     hgt_lvls =[]
     for key in intrp['hgt_lvls'].keys():
         hgt_lvls.append(intrp['hgt_lvls'][key])
     hgt_lvls.pop(0) 
 
     for key in hgt_lvls[1::4]:
+        # for a hgt_lvl key, find the pressure at that level's index, plot the hgt at the pressure
         trans, _, _ = skew.ax.get_yaxis_text1_transform(0)
         skew.ax.text(0.048, intrp['pINTRP'][key], f"{int(intrp['zINTRP'][key]/1000)}km", 
-                     fontsize=13, transform=trans, alpha=0.6, weight='bold', color=gen_txt_clr)   
-    
+                     fontsize=11, transform=trans, alpha=0.6, weight='bold', color=gen_txt_clr) 
+        
+    # add a '-sfc-' marker with an elevation of the sfc in meters
     trans, _, _ = skew.ax.get_yaxis_text1_transform(0)
     sfc = mpcalc.height_to_pressure_std(general['elevation']*units.m)
-    skew.ax.text(0.048, p[0], '-SFC-', fontsize=13, transform=trans, alpha=0.6, weight='bold', color=gen_txt_clr) # plot 'SFC' @ surface pressure
+    skew.ax.text(0.048, p[0], f"-SFC ({mag(general['elevation'])}m) -", 
+                 fontsize=11, transform=trans, alpha=0.6, weight='bold', color=gen_txt_clr)
     
     
     # SFC TEMPERATURE AND DEWPOINT ANNOTATIONS---------------------------------------------
+    # plot sfc T value in degF
     T_degF = np.round(T.to(units.degF), 1)
     T_degF_label = '{}°F'.format(int(T_degF[0].magnitude))                             
     plt.annotate(T_degF_label, (T[0], p[0]), textcoords="offset points", xytext=(16,-15),
-                     fontsize=12, color='red', weight='bold', alpha=0.7, ha='center')   
+                     fontsize=12, color='red', weight='bold', alpha=0.7, ha='center') 
+    
+    # plot sfc Td value in DegF
     Td_degF = np.round(Td.to(units.degF), 1) 
     Td_degF_label = '{}°F'.format(int(Td_degF[0].magnitude))                             
     plt.annotate(Td_degF_label,(Td[0], p[0]),textcoords="offset points",xytext=(-16,-15), 
                      fontsize=12, color=td_color, weight='bold', alpha=0.7, ha='center') 
-
+    
+    # if the sfc was modified by the user, plot a modified sfc flag
+    if modify_sfc_txt == True: 
+        plt.annotate("USER MODIFIED SFC →", (Td[0], p[0]),textcoords="offset points",xytext=(-50,0), 
+                     fontsize=10, color='black', weight='bold', alpha=0.5, ha='right')
+        
+        
     # PARCEL HEIGHT ANNOTATIONS------------------------------------------------------------- 
+    # plot the SBLCL and draw a line between the sfc and the lcl
     plt.text((0.82), (thermo['sb_lcl_p']), "←SBLCL", weight='bold',color='gray',
              alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
-    lcl_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_lcl_p']), color='gray', linestyle=':', alpha=1, transform=skew.ax.get_yaxis_transform())
+    lcl_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_lcl_p']), 
+                          color='gray', linestyle=':', alpha=1, transform=skew.ax.get_yaxis_transform())
     skew.ax.add_artist(lcl_line)
+    
+    # if a mulfc doesn't exist,
+    # plot the sblfc, and sbel and draw a line between the lcl and lfc and the lcl to the el
     if ma.is_masked(thermo['mu_lfc_z']) == True:
         plt.text((0.82), (thermo['sb_lfc_p']), "←SBLFC", weight='bold',color='gray',
                  alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
         plt.text((0.82), (thermo['sb_el_p']), "←SBEL", weight='bold',color='gray', 
                  alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
-        el_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_el_p']), color='gray', linestyle=':', alpha=0.3, transform=skew.ax.get_yaxis_transform())
+        el_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_el_p']), 
+                             color='gray', linestyle=':', alpha=0.3, transform=skew.ax.get_yaxis_transform())
         skew.ax.add_artist(el_line)
-        lfc_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_lfc_p']), color='gray', linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
+        lfc_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_lfc_p']), 
+                              color='gray', linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
         skew.ax.add_artist(lfc_line)
+    
     else: 
+        # if not, plot mulfc and muel and draw a line between the lcl and lfc and the lcl to the el
         plt.text((0.82), (thermo['mu_lfc_p']), "←MULFC", weight='bold',color='gray',
                  alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
         plt.text((0.82), (thermo['mu_el_p']), "←MUEL", weight='bold',color='gray',
                  alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
-        el_line = plt.Line2D([0.86, 0.86], (p[0], thermo['mu_el_p']), color='gray', linestyle=':', alpha=0.3, transform=skew.ax.get_yaxis_transform())
+        el_line = plt.Line2D([0.86, 0.86], (p[0], thermo['mu_el_p']), 
+                             color='gray', linestyle=':', alpha=0.3, transform=skew.ax.get_yaxis_transform())
         skew.ax.add_artist(el_line)
-        lfc_line = plt.Line2D([0.86, 0.86], (p[0], thermo['mu_lfc_p']), color='gray', linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
+        lfc_line = plt.Line2D([0.86, 0.86], (p[0], thermo['mu_lfc_p']), 
+                              color='gray', linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
         skew.ax.add_artist(lfc_line)
         
+        # plot mumpl, but if its above 110 hPa, just plot whatever the value is at 110 hPa
+        if thermo['mu_mpl_p'] < 110:
+            plt.text((0.82), (110), f"↑MUMPL: {mag(thermo['mu_mpl_p'])}hPa", weight='bold',color='gray',
+                     alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
+        else: 
+            plt.text((0.82), (thermo['mu_mpl_p']), "←MUMPL", weight='bold',color='gray',
+                     alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
         
         
         
-    #FRREZING POINT ANNOTATION--------------------------------------------------------------
+        
+    # T & WB FRREZING POINT ANNOTATION--------------------------------------------------------------
     if ma.is_masked(general['frz_pt_z']) == False:
         if general['frz_pt_z'] >= 50*units.m:
-            plt.text((0.78), (general['frz_pt_p']), "←FRZ", weight='bold',color='cornflowerblue',  
-                     alpha=0.6, fontsize=10, transform=skew.ax.get_yaxis_transform(), clip_on=True)
+            plt.text((0.76), (general['frz_pt_p']), "←FRZ", weight='bold',color='cornflowerblue',  
+                     alpha=0.6, fontsize=12, transform=skew.ax.get_yaxis_transform(), clip_on=True)
+    
+    if ma.is_masked(general['wb_frz_pt_z']) == False:
+        if general['wb_frz_pt_z'] >= 50*units.m:
+            plt.text((0.76), (general['wb_frz_pt_p']), "←WB0", weight='bold',color='darkblue',  
+                     alpha=0.6, fontsize=12, transform=skew.ax.get_yaxis_transform(), clip_on=True)
 
-    #PBL TOP POINT ANNOTATION---------------------------------------------------------------                   
+            
+    # PBL TOP POINT ANNOTATION---------------------------------------------------------------                   
     plt.text((0.78), (thermo['pbl_top']), "←PBL", weight='bold',color='gray', 
              alpha=0.9, fontsize=10, transform=skew.ax.get_yaxis_transform(), clip_on=True)
-    pbl_line = plt.Line2D([0.80, 0.80], (p[0], thermo['pbl_top']), color='gray', linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
+    pbl_line = plt.Line2D([0.80, 0.80], (p[0], thermo['pbl_top']), color='gray', 
+                          linestyle=':', alpha=0.7, transform=skew.ax.get_yaxis_transform())
     skew.ax.add_artist(pbl_line)
 
     
     # 0-3km & 0-6km CAPE ANNOTATIONS--------------------------------------------------------
     if thermo['mu3cape'] > 10:
         idx = find_nearest(thermo['muZ_trace'], 3000)
         cape03_label = " ←{}J/kg".format(mag(thermo['mu3cape']))     
         plt.annotate(cape03_label,  ((thermo['muT_trace'][idx]+7), intrp['pINTRP'][intrp['hgt_lvls']['h3']]),  textcoords="offset points",  xytext=(20, 0), 
-                     color='red', alpha=0.4, fontsize=13.5, weight='bold', ha='right')  
+                     color='red', alpha=0.6, fontsize=13.5, ha='right')  
             
             
     if thermo['mu6cape'] > thermo['mu3cape']:
         idx = find_nearest(thermo['muZ_trace'], 6000)
         cape06_label = " ←{}J/kg".format(mag(thermo['mu6cape']))                                            
         plt.annotate(cape06_label, ((thermo['muT_trace'][idx]+7), intrp['pINTRP'][intrp['hgt_lvls']['h6']]), textcoords="offset points",  xytext=(10, 0), 
-                         color='red', alpha=0.4, fontsize=13.5, weight='bold', ha='right') 
+                         color='red', alpha=0.6, fontsize=13.5, ha='right') 
             
             
     if thermo['mucape'] > thermo['mu6cape']:
             cape_label = "←{}J/kg".format(mag(thermo['mucape']))                                            
             plt.annotate(cape_label,((thermo['mu_el_T']), thermo['mu_el_p']), textcoords="offset points",  xytext=(5, 0), 
-                         color='red', alpha=0.4, fontsize=13.5, weight='bold', ha='left') 
+                         color='red', alpha=0.6, fontsize=13.5, ha='left') 
             
             
             
     # MAX LAPSE RATE ANNOTATION---------------------------------
     x_start, x_end = 0.15, 0.17
     x_mid = (x_start + x_end)/2
     Lapse_line = plt.Line2D([x_mid, x_mid], (thermo['lr_max'][1], thermo['lr_max'][2]), color='firebrick', linewidth=3, alpha=0.3, transform=skew.ax.get_yaxis_transform())
@@ -434,24 +648,24 @@
     x_mid = (x_start + x_end)/2
     plt.text((x_start+0.01), (kinem['eil'][1]-8), "EIL", weight='bold',color='lightblue', alpha=0.4, ha='center', fontsize=13, transform=skew.ax.get_yaxis_transform())
     EIL_line = plt.Line2D([x_mid, x_mid], (kinem['eil'][0], kinem['eil'][1]), color='lightblue', linewidth=3, alpha=0.4, transform=skew.ax.get_yaxis_transform())
     skew.ax.add_artist(EIL_line)
 
     # DGZ ANNOTATION-------------------------------
     if T[0].m < 5:
-        if thermo['dgz'][1] < clean_data['p'][0].m:
+        if thermo['dgz'][1] < p[0].m:
             x_start, x_end = 0.12, 0.14
             x_mid = (x_start + x_end)/2
             plt.text((x_start+0.01), (thermo['dgz'][1]-8), "DGZ", weight='bold',color='blue', alpha=0.4, ha='center', fontsize=13, transform=skew.ax.get_yaxis_transform())
             dgz_line = plt.Line2D([x_mid, x_mid], (thermo['dgz'][0], thermo['dgz'][1]), color='blue', linewidth=3, alpha=0.4, transform=skew.ax.get_yaxis_transform())
             skew.ax.add_artist(dgz_line)
       
     # HGZ ANNOTATION-------------------------------
     else:
-        if thermo['hgz'][1] < clean_data['p'][0].m:
+        if thermo['hgz'][1] < p[0].m:
             x_start, x_end = 0.12, 0.14
             x_mid = (x_start + x_end)/2
             plt.text((x_start+0.01), (thermo['hgz'][1]-8), "HGZ", weight='bold',color='green', alpha=0.4, ha='center', fontsize=13, transform=skew.ax.get_yaxis_transform())
             hgz_line = plt.Line2D([x_mid, x_mid], (thermo['hgz'][0], thermo['hgz'][1]), color='green', alpha=0.4, linewidth=3, transform=skew.ax.get_yaxis_transform())
             skew.ax.add_artist(hgz_line)
             
             
@@ -460,34 +674,36 @@
 
     try:
         for hgt_idx in hgts:
             label = "{}% →".format(int(intrp['rhINTRP'][hgt_idx]))
             plt.annotate(label, (mpcalc.dewpoint_from_relative_humidity(intrp['tINTRP'][hgt_idx]*units.degC, 
                                                                     intrp['rhINTRP'][hgt_idx]/100),
                          intrp['pINTRP'][hgt_idx]*units.hPa), textcoords="offset points", xytext=(-40, 0), 
-                         color='green', weight='bold', alpha=0.4, fontsize=13.5, ha='center') 
+                         color='green', alpha=0.4, fontsize=13.5, ha='center', clip_on=True) 
     except:
         pass
     #################################################################
     
     
     
     
     #################################################################
     ### PLOT SKEW T WIND BARBS ###
     #################################################################
-    interval = np.logspace(2.113, 3, 30) *units.hPa # Arrange wind barbs for best fit
-    idx = mpcalc.resample_nn_1d(p, interval) # Resample wind barbs for best fit
+    # Arrange wind barbs for best fit & resample wind barbs for best fit
+    interval = np.logspace(2.113, 3, 30) *units.hPa
+    idx = mpcalc.resample_nn_1d(p, interval) 
 
     # create blank barbs for small dot at the start of each actual barb
     blank_len = len(u[idx])     
     blank = np.zeros(blank_len)  
     skew.plot_barbs(pressure=p[idx], u=blank, v=blank, xloc=0.955, fill_empty=True, color=barb_clr,
                     sizes=dict(emptybarb=0.075, width=0.18, height=0.4))
 
+    # plot actual wind barbs
     skew.plot_barbs(pressure=p[idx], u=u[idx], v=v[idx], xloc=0.955, fill_empty=True, color=barb_clr,
                     sizes=dict(emptybarb=0.075, width=0.18, height=0.4), length=8)
 
     # Draw line underneath wind barbs
     line = mlines.Line2D([0.955, 0.955], [0.01,0.95],color=barb_clr,linewidth=0.5,
                          transform=skew.ax.transAxes,clip_on=False,zorder=1)
     skew.ax.add_line(line)  
@@ -498,17 +714,17 @@
     ############################## HODOGRAPH ################################
     #########################################################################
     
     
     #################################################################
     ### DEFINE HODOGRAPH BOUNDS ###
     #################################################################
+    # restructure u and v, p, ws and z data arrays based on corrected u and v arrays and hodo_layer depth
     if (z.max().m - z[0].m) > 9001: 
         hodo_hgt = 9000*units.m
-        # restructure u and v, p, ws and z data arrays based on corrected u and v arrays and hodo_layer depth
         p_hodo, u_hodo, v_hodo, z_hodo = mpcalc.get_layer(p, u, v, z, depth=hodo_hgt)
     else:
         p_hodo = p
         u_hodo = u
         v_hodo = v
         z_hodo = z
     # determine max height of wind data to plot on hodograph in km (if hodo_layer = 9, 0-9km u and v are plotted)
@@ -517,178 +733,213 @@
     v_clean = v.magnitude[np.logical_not(np.isnan(v.magnitude))]
     # restructure u and v, p, ws and z data arrays based on corrected u and v arrays and hodo_layer depth
     # define x and y min/max values from 'cleaned' and restructured u and v arrays
     x_min = u_hodo.min().m
     y_min = v_hodo.min().m
     x_max = u_hodo.max().m
     y_max = v_hodo.max().m
+    
     # if statements to determine approprate x axis and y axis limits (to change dynamically with the data)
     if y_max >= 0:
-        y_Maxlimit = (y_max + 15)
+        y_Maxlimit = (y_max + 30)
     if y_max < 0:
-        y_Maxlimit = (y_max + 15)
+        y_Maxlimit = (y_max + 30)
 
     if x_max >= 0:
-        x_Maxlimit = (x_max + 15)
+        x_Maxlimit = (x_max + 30)
     if x_max < 0:
-        x_Maxlimit = (x_max + 15)
+        x_Maxlimit = (x_max + 30)
 
     if y_min >= 0:
-        y_Minlimit = (y_min - 40)
+        y_Minlimit = (y_min - 45)
     if y_min < 0:
-        y_Minlimit = (y_min - 40)
+        y_Minlimit = (y_min - 45)
 
     if x_min >= 0:
-        x_Minlimit = (x_min - 40)
+        x_Minlimit = (x_min - 45)
     if x_min < 0:
-        x_Minlimit = (x_min - 40)
+        x_Minlimit = (x_min - 45)
     #################################################################
         
         
+        
     #################################################################
     ### CREATE HODOGRAPH OBJECT ###
     #################################################################
+    # create hodograph object
     hod_ax = plt.axes((0.53, 0.1003, 0.85, 0.85))
     h = Hodograph(hod_ax, component_range=160.)
+    # dynamically set hodograph axis bounds
     try:
         h.ax.set_xlim(x_Minlimit, x_Maxlimit)                                  
         h.ax.set_ylim(y_Minlimit, y_Maxlimit)                             
     except:
         h.ax.set_xlim(-65,65)
         h.ax.set_ylim(-65,65)
-        pass                                                                         
-    h.add_grid(increment=20, color=gen_txt_clr, linestyle='-', linewidth=1.5, alpha=0.4) 
-    h.add_grid(increment=10, color=gen_txt_clr, linewidth=1, linestyle='--', alpha=0.4) 
+        pass
+    # add hodograph grid lines
+    h.add_grid(increment=20, color=gen_txt_clr, linestyle='-', linewidth=1.5, alpha=0.2) 
+    h.add_grid(increment=10, color=gen_txt_clr, linewidth=1, linestyle='--', alpha=0.2) 
+    # add background color
     h.ax.set_facecolor(bckgrnd_clr)
+    # add spines 
     h.ax.spines["top"].set_color(brdr_clr)
     h.ax.spines["left"].set_color(brdr_clr)
     h.ax.spines["right"].set_color(brdr_clr)
     h.ax.spines["bottom"].set_color(brdr_clr)
     h.ax.spines["bottom"].set_color(brdr_clr)
-    h.ax.set_box_aspect(1) 
+    # define box aspect
+    h.ax.set_box_aspect(1)
+    # define tick label params (remove them)
     h.ax.set_yticklabels([])
     h.ax.set_xticklabels([])
     h.ax.set_xticks([])
     h.ax.set_yticks([])
     h.ax.set_xlabel(' ')
     h.ax.set_ylabel(' ')
     #################################################################
     
     
     
     #################################################################
-    ### PLOT HEIGHT MARKERS ###
+    ### PLOT VELOCITY AND HEIGHT MARKERS ###
     #################################################################
+    # add small velocity markers on the rings 
     plt.xticks(np.arange(0,0,1))
     plt.yticks(np.arange(0,0,1))
     for i in range(10,130,20):
-        h.ax.annotate(str(i),(i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
+        h.ax.annotate(str(i),(i,0),xytext=(0,2),textcoords='offset pixels',
+                      clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
-        h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
+        h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',
+                      clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
-        h.ax.annotate(str(i),(-i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
+        h.ax.annotate(str(i),(-i,0),xytext=(0,2),textcoords='offset pixels',
+                      clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
-        h.ax.annotate(str(i),(0,-i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
+        h.ax.annotate(str(i),(0,-i),xytext=(0,2),textcoords='offset pixels',
+                      clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
 
-    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', 
+    
+    # add 0.5km marker
+    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', markeredgecolor='black',
            color='white', alpha=1, markersize=30, clip_on=True, zorder=5)
     h.ax.annotate(str('.5'),(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']]),
-                  weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+                  weight='bold', fontsize=11, color='black',xytext=(0.02,-5),
+                  textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
 
+    # add hgt markers 
     hgt_lvls = [] 
     for key in intrp['hgt_lvls'].keys():
         hgt_lvls.append(intrp['hgt_lvls'][key])
     hgt_lvls.pop(0) 
 
-    for i in hgt_lvls[1::2]:
-        h.plot(intrp['uINTRP'][i],intrp['vINTRP'][i], marker='.', color='white', alpha=1, markersize=30, zorder=5)
-        h.ax.annotate(str(int(round(intrp['zINTRP'][i]/1000,0))),(intrp['uINTRP'][i],intrp['vINTRP'][i]), 
-                      weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+    for lvl in hgt_lvls[1::2]:
+        if lvl < 130:
+            h.plot(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl], marker='.', color='white', 
+                   markeredgecolor='black', alpha=1, markersize=30, zorder=5)
+            h.ax.annotate(str(int(round(intrp['zINTRP'][lvl]/1000,0))),(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl]), 
+                          weight='bold', fontsize=11, color='black',xytext=(0.02,-5),
+                          textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=5.1) 
     #################################################################
     
     
     
     
     
+    
     #################################################################
     ### PLOT HODOGRAPH LINE ###
     #################################################################
     hodo_color = ['purple','red','darkorange','gold','#fff09f']
 
-    h.ax.plot(intrp['uINTRP'][0:10+1],   intrp['vINTRP'][0:10+1],   color=hodo_color[0], linewidth=7, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][10:30+1],  intrp['vINTRP'][10:30+1],  color=hodo_color[1], linewidth=7, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][30:60+1],  intrp['vINTRP'][30:60+1],  color=hodo_color[2], linewidth=7, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][60:90+1],  intrp['vINTRP'][60:90+1],  color=hodo_color[3], linewidth=7, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][90:120+1], intrp['vINTRP'][90:120+1], color=hodo_color[4], linewidth=7, clip_on=True) 
+    h.ax.plot(intrp['uINTRP'][0:10+1],   intrp['vINTRP'][0:10+1],   color=hodo_color[0], linewidth=7, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][10:30+1],  intrp['vINTRP'][10:30+1],  color=hodo_color[1], linewidth=7, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][30:60+1],  intrp['vINTRP'][30:60+1],  color=hodo_color[2], linewidth=7, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][60:90+1],  intrp['vINTRP'][60:90+1],  color=hodo_color[3], linewidth=7, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][90:120+1], intrp['vINTRP'][90:120+1], color=hodo_color[4], linewidth=7, zorder=4, clip_on=True) 
 
     
     
+    
     #################################################################
-    ### ADD HODOGRAPH ANNOTATION ###
+    ### ADD HODOGRAPH ANNOTATIONS ###
     #################################################################
+    # BUNKERS STORM MOTION
     if ma.is_masked(kinem['sm_rm']) == False:
-        # BUNKERS STORM MOTION
-        h.ax.text((kinem['sm_rm'][0]+0.5), (kinem['sm_rm'][1]-0.5), 'RM', weight='bold', ha='left', fontsize=14, alpha=0.9, color=gen_txt_clr)
-        h.ax.text((kinem['sm_lm'][0]+0.5), (kinem['sm_lm'][1]-0.5), 'LM', weight='bold', ha='left', fontsize=14, alpha=0.9, color=gen_txt_clr)
-        h.ax.text((kinem['sm_mw'][0]+0.5), (kinem['sm_mw'][1]-0.5), 'MW', weight='bold', ha='left', fontsize=14, alpha=0.9, color=gen_txt_clr)
+        h.ax.text((kinem['sm_rm'][0]+0.5), (kinem['sm_rm'][1]-0.5), 'RM', 
+                  weight='bold', ha='left', fontsize=14, zorder=7, alpha=0.9, color=gen_txt_clr)
+        h.ax.text((kinem['sm_lm'][0]+0.5), (kinem['sm_lm'][1]-0.5), 'LM', 
+                  weight='bold', ha='left', fontsize=14, zorder=7, alpha=0.9, color=gen_txt_clr)
+        h.ax.text((kinem['sm_mw'][0]+0.5), (kinem['sm_mw'][1]-0.5), 'MW', 
+                  weight='bold', ha='left', fontsize=14, zorder=7, alpha=0.9, color=gen_txt_clr)
     
+    # DEVIANT TORNADO MOTION
     if ma.is_masked(kinem['sm_u']) == False:
-        # DEVIANT TORNADO MOTION
-        h.ax.text(kinem['dtm'][0], (kinem['dtm'][1] + 2), 'DTM', weight='bold', fontsize=10, color='brown', ha='center')
-        h.plot(kinem['dtm'][0], kinem['dtm'][1], marker='v', color='brown', markersize=8, alpha=0.8, ls='', label='DEVIANT TORNADO MOTION')
+        h.ax.text(kinem['dtm'][0], (kinem['dtm'][1] + 2), 'DTM', 
+                  weight='bold', fontsize=10, zorder=7, color='brown', ha='center')
+        h.plot(kinem['dtm'][0], kinem['dtm'][1], marker='v', color='brown', 
+               markersize=8, zorder=7, alpha=0.8, ls='', label='DEVIANT TORNADO MOTION')
     
-        # ADD SM POINT IF ITS A CUSTOM STORM MOTION
+    # ADD SM POINT IF ITS A CUSTOM STORM MOTION
         if str(type(storm_motion)) == "<class 'list'>":
-            h.ax.text((kinem['sm_u']+0.5), (kinem['sm_v']-0.5), 'SM', weight='bold', ha='left', fontsize=14, alpha=0.9, color=gen_txt_clr)
+            h.ax.text((kinem['sm_u']+0.5), (kinem['sm_v']-0.5), 'SM', 
+                      weight='bold', ha='left', fontsize=14, alpha=0.9, zorder=7, color=gen_txt_clr)
         
         h.ax.arrow(0,0,kinem['sm_u']-0.3, kinem['sm_v']-0.3, linewidth=3, color=gen_txt_clr, alpha=0.2, 
-                label='SM Vector', length_includes_head=True, head_width=0.5)
+                label='SM Vector', length_includes_head=True, head_width=0.6)
     
     
     # EFFECTIVE INFLOW LAYER SRH FILL
     if ma.is_masked(kinem['eil_z'][0]) == False:
         
-        ebot = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]), (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]),  
-                 linestyle='--', linewidth=2.3, alpha=0.5, color='lightblue', label='Effective Inflow Layer')
-        etop = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]), (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]),  
-                 linestyle='--', linewidth=2.3, alpha=0.5, color='lightblue')
-        fill_srh = h.ax.fill(np.append(intrp['uINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_u']), 
-                             np.append(intrp['vINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_v']),
-                             'lightblue',alpha=0.1, label='EIL SRH')
+        ebot = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]), 
+                         (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]),  
+                 linestyle='-', linewidth=2.3, alpha=0.5, zorder=3, color='lightblue', label='Effective Inflow Layer')
+        etop = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]), 
+                         (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]),  
+                 linestyle='-', linewidth=2.3, alpha=0.5, zorder=3, color='lightblue')
+        fill_srh = h.ax.fill(np.append(intrp['uINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_u']), np.append(intrp['vINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_v']),'lightblue',alpha=0.3, zorder=2, label='EIL SRH')
     else:
         fill_srh = h.ax.fill(np.append(intrp['uINTRP'][find_nearest(intrp['zINTRP'], 0):find_nearest(intrp['zINTRP'], 3000)], kinem['sm_u']), 
                      np.append(intrp['vINTRP'][find_nearest(intrp['zINTRP'], 0):find_nearest(intrp['zINTRP'], 3000)], kinem['sm_v']),
-                     'lightblue',alpha=0.1, label='0-3 SRH')
+                     'lightblue',alpha=0.1, zorder=2, label='0-3 SRH')
     
     
     # MCS MOTION
-    h.ax.text(kinem['mcs'][0], kinem['mcs'][1], 'UP', weight='bold', fontsize=12, color='orange', ha='center', alpha=0.5, clip_on=True)
-    h.ax.text(kinem['mcs'][2], kinem['mcs'][3], 'DN', weight='bold', fontsize=12, color='orange', ha='center', alpha=0.5, clip_on=True)
+    h.ax.text(kinem['mcs'][0], kinem['mcs'][1], 'UP', 
+              weight='bold', fontsize=12, color='orange', zorder=7, ha='center', alpha=0.5, clip_on=True)
+    h.ax.text(kinem['mcs'][2], kinem['mcs'][3], 'DN', 
+              weight='bold', fontsize=12, color='orange', zorder=7, ha='center', alpha=0.5, clip_on=True)
     
     
     # STORM MOTION PRINTOUT
     if ma.is_masked(kinem['sm_u']) == False:
         try:
             keys = ['sm_rm', 'sm_lm', 'sm_mw', 'dtm'] 
 
             speeds = []
             directions = []
             
             speeds.append(mpcalc.wind_speed(kinem['sm_u']*units.kts,kinem['sm_v']*units.kts).m) 
-            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['sm_u'],kinem['sm_v']))), full=False, level=3)) 
+            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['sm_u'],kinem['sm_v']))), 
+                                                        full=False, level=3)) 
 
             for key in keys:
                 speeds.append(mpcalc.wind_speed(kinem[key][0]*units.kts,kinem[key][1]*units.kts).m) 
-                directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem[key][0],kinem[key][1]))), full=False, level=3))
+                directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem[key][0],kinem[key][1]))), 
+                                                            full=False, level=3))
 
             speeds.append(mpcalc.wind_speed(kinem['mcs'][0]*units.kts,kinem['mcs'][1]*units.kts).m) 
-            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['mcs'][0],kinem['mcs'][1]))), full=False, level=3))   
+            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['mcs'][0],kinem['mcs'][1]))), 
+                                                        full=False, level=3))   
 
             speeds.append(mpcalc.wind_speed(kinem['mcs'][2]*units.kts,kinem['mcs'][3]*units.kts).m) 
-            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['mcs'][2],kinem['mcs'][3]))), full=False, level=3)) 
+            directions.append(mpcalc.angle_to_direction((np.degrees(np.arctan2(kinem['mcs'][2],kinem['mcs'][3]))), 
+                                                        full=False, level=3)) 
                     
                     
             #plot Bunkers Storm Motion & DTM Data in box on Hodograph 
             plt.figtext(0.748, 0.919, 
                         f' RM: {directions[1]} @ {mag(speeds[1])} kts\n LM: {directions[2]} @ {mag(speeds[2])} kts\n' + 
                         f' MW: {directions[3]} @ {mag(speeds[3])} kts\nDTM: {directions[4]} @ {mag(speeds[4])} kts\n US: {directions[5]} @ {mag(speeds[5])} kts\n' + 
                         f' DS: {directions[6]} @ {mag(speeds[6])} kts\n',
@@ -728,15 +979,14 @@
     temp_adv_ax = plt.axes((0.701,0.1003,0.04,0.85))
     temp_adv_ax.spines["top"].set_color(brdr_clr)
     temp_adv_ax.spines["left"].set_color(brdr_clr)
     temp_adv_ax.spines["right"].set_color(brdr_clr)
     temp_adv_ax.spines["bottom"].set_color(brdr_clr)
     temp_adv_ax.spines["bottom"].set_color(brdr_clr)   
     temp_adv_ax.set_facecolor(bckgrnd_clr)    
-    
     plt.yscale('log')
     temp_adv_ax.set_ylim(1050, 100)
     temp_adv_ax.set_xlim(np.nanmin(thermo['temp_adv'][0])-4, np.nanmax(thermo['temp_adv'][0])+4)
     plt.ylabel(' '), plt.xlabel(' ')
     temp_adv_ax.set_yticklabels([]), temp_adv_ax.set_xticklabels([])
     temp_adv_ax.tick_params(axis='y', length = 0), temp_adv_ax.tick_params(axis='x', length = 0)
     # ADD LINES
@@ -745,24 +995,92 @@
         plt.plot((-20,20), (lvl,lvl), color='gray', alpha=0.8, linewidth=1, linestyle='-', clip_on=True)
     # PLOT TEMP ADV BINS 
     for i in range(len(thermo['temp_adv'][0])):
                         if thermo['temp_adv'][0][i] <= 0:
                             temp_adv_bxclr = 'cornflowerblue'
                         elif thermo['temp_adv'][0][i]  > 0:
                             temp_adv_bxclr = 'red'
-                        temp_adv_ax.barh(top_arr[i], thermo['temp_adv'][0][i], align='center', height=bot_arr[i]-top_arr[i], edgecolor='black', alpha=0.3, color=temp_adv_bxclr)
+                        temp_adv_ax.barh(top_arr[i], thermo['temp_adv'][0][i], align='center', 
+                                         height=bot_arr[i]-top_arr[i], edgecolor='black', alpha=0.3, color=temp_adv_bxclr)
                         if thermo['temp_adv'][0][i] > 0:
-                            temp_adv_ax.annotate((np.round(thermo['temp_adv'][0][i],1)), xy=(0.3, top_arr[i]+10), color=gen_txt_clr, textcoords='data', ha='left', weight='bold')
+                            temp_adv_ax.annotate((np.round(thermo['temp_adv'][0][i],1)), 
+                                                 xy=(0.3, top_arr[i]+10), color=gen_txt_clr, textcoords='data', 
+                                                 ha='left', weight='bold')
                         if thermo['temp_adv'][0][i] < 0:
-                            temp_adv_ax.annotate((np.round(thermo['temp_adv'][0][i],1)), xy=(-0.3, top_arr[i]+10), color=gen_txt_clr, textcoords='data', ha='right', weight='bold')
+                            temp_adv_ax.annotate((np.round(thermo['temp_adv'][0][i],1)), 
+                                                 xy=(-0.3, top_arr[i]+10), color=gen_txt_clr, textcoords='data', 
+                                                 ha='right', weight='bold')
     temp_adv_ax.axvline(x=0, color=gen_txt_clr, linewidth=1, linestyle='--', clip_on=True)
     #################################################################
     
     
     
+    
+    
+    
+    #################################################################
+    ### SOUNDING MAP INSET -- TEST ###
+    #################################################################
+    # BUILD SIMPLE MAP -----------------------------------------------------------------------------------------------------
+    if map_zoom > 0:
+        proj = ccrs.PlateCarree()
+        map_ax = plt.axes((0.7005, 0.1, 0.20, 0.20), projection=proj, zorder=12) # 1, 0.1 | 0.542, 0.75, 0.20, 0.20
+        map_ax.spines['geo'].set_color(gen_txt_clr)
+
+        zoom_factor = map_zoom
+        map_ax.set_extent([clean_data['site_info']['site-latlon'][1] + zoom_factor, 
+                           clean_data['site_info']['site-latlon'][1] - zoom_factor, 
+                           clean_data['site_info']['site-latlon'][0] + zoom_factor, 
+                           clean_data['site_info']['site-latlon'][0] - zoom_factor])
+        map_ax.set_box_aspect(1) 
+
+        map_ax.add_feature(cfeature.STATES, color=bckgrnd_clr, zorder=1)
+        map_ax.add_feature(cfeature.STATES, edgecolor=gen_txt_clr, alpha=0.7, 
+                       linestyle='-', linewidth=2, zorder=6)
+        map_ax.add_feature(USCOUNTIES, alpha=0.3, edgecolor=gen_txt_clr, 
+                           linestyle='-', linewidth=0.2, zorder=5)
+
+        if show_radar == True:
+            # BUILD COLOR MAP -----------------------------------------------------------------------------------------------------
+            radar_cmap = LinearSegmentedColormap.from_list('custom_cmap',
+                        ['#B0C4DE', '#4682B4', '#90EE90', '#228B22', '#FFFF4D', '#E6E600',
+                        '#FFC34D', '#E69900', '#FF4D4D', '#E60000', '#FFCCEE', '#FF198C',
+                        '#D400FF', '#550080'], N=256)
+
+
+            # PLOT RADAR DATA -----------------------------------------------------------------------------------------------------
+            try:
+                radar_data = get_radar_mosaic(sounding_data, map_zoom, radar_time)
+
+                reflectivity = np.ma.masked_array(np.array(radar_data['Reflectivity'])[0,:,:],
+                                                  np.array(radar_data['Reflectivity'])[0,:,:]<10)
+
+                map_ax.pcolormesh(radar_data['lon']+0.05, radar_data['lat']+0.05, reflectivity, 
+                                  vmin=10, vmax=80, cmap=radar_cmap, alpha=1, zorder=4)
+
+                radar_timestamp = f"{str(radar_data['time'].values[0])[5:10]} | {str(radar_data['time'].values[0])[11:16]}"
+
+
+                plt.figtext(0.80, 0.11, f'Valid: {radar_timestamp}', 
+                        ha='center', alpha=0.9, weight='bold', fontsize=13, zorder=13, color=gen_txt_clr,
+                        bbox=dict(facecolor=bckgrnd_clr, alpha=0.8, edgecolor=gen_txt_clr, pad=3))
+            except: 
+                pass
+
+        # ADD PROFILE LOCATION ------------------------------------------------------------------------------------------------
+        map_ax.plot(clean_data['site_info']['site-latlon'][1],clean_data['site_info']['site-latlon'][0], 
+                    marker='o', mfc='none', markeredgewidth=1.5, 
+                    color=marker_clr, markersize='11', transform=ccrs.PlateCarree(), zorder=10, clip_on=True)
+        map_ax.plot(clean_data['site_info']['site-latlon'][1],clean_data['site_info']['site-latlon'][0], 
+                    marker='+', color=marker_clr, markeredgewidth=1.5, 
+                    markersize='18', transform=ccrs.PlateCarree(), zorder=10, clip_on=True)
+
+    #################################################################
+    
+    
     #################################################################
     ### STREAMWISENESS AND RH W/HGT ###
     #################################################################
     # PLOT AXIS/LOC
     strmws_ax = plt.axes((0.945, -0.13, 0.065, 0.23))
     plt.figtext(0.978, 0.07, f'SW ζ (%)', color=gen_txt_clr, weight='bold', fontsize=12, ha='center', alpha=0.7)
     strmws_ax.spines["top"].set_color(brdr_clr)
@@ -830,21 +1148,23 @@
         #XTICKS
         vort_ax.set_xlabel(' ')
         vort_max = kinem['vort'][0:30].max()+0.005
         vort_min = kinem['vort'][0:30].min()-0.005
     
         vort_ax.set_xlim(vort_min-0.002, vort_max+0.002)
         vort_ax.set_xticks([(vort_min+0.005),(vort_max-0.005)])
-        vort_ax.set_xticklabels([(np.round(vort_min+0.002,2)),(np.round(vort_max-0.002,2))], weight='bold', alpha=0.5, fontstyle='italic', color=gen_txt_clr)
+        vort_ax.set_xticklabels([(np.round(vort_min+0.002,2)),(np.round(vort_max-0.002,2))], 
+                                weight='bold', alpha=0.5, fontstyle='italic', color=gen_txt_clr)
  
         vort_ax.plot(kinem['swv'][0:30],  intrp['zINTRP'][0:30], color='orange', linewidth=3, alpha=0.8, label='SW ζ')
         vort_ax.plot(kinem['vort'][0:30], intrp['zINTRP'][0:30], color=gen_txt_clr,  linewidth=4, alpha=0.4, label='Total ζ')
         
         if ma.is_masked(kinem['eil_z'][0]) == False:
-            vort_ax.fill_between(x=(vort_min-0.002, vort_max+0.002), y1=kinem['eil_z'][0], y2=kinem['eil_z'][1], color='lightblue', alpha=0.2)
+            vort_ax.fill_between(x=(vort_min-0.002, vort_max+0.002), y1=kinem['eil_z'][0], 
+                                 y2=kinem['eil_z'][1], color='lightblue', alpha=0.2)
     else:
         warnings.warn("Total Vorticity could not be plotted (no valid storm motion/not enough data)", Warning)
     #################################################################
     
     
     
     
@@ -872,22 +1192,26 @@
 
     if ma.is_masked(kinem['sm_u']) == False:
         #XTICKS
         wind_max = kinem['srw'][0:30].max()+1
         wind_min = kinem['srw'][0:30].min()-1
         wind_ax.set_xlim(wind_min-5, wind_max+5)
         wind_ax.set_xticks([(wind_min)+2, (wind_max)-2])
-        wind_ax.set_xticklabels([(int(wind_min)+2), (int(wind_max)-2)], weight='bold', alpha=0.5, fontstyle='italic', color=gen_txt_clr)
+        wind_ax.set_xticklabels([(int(wind_min)+2), (int(wind_max)-2)], weight='bold', 
+                                alpha=0.5, fontstyle='italic', color=gen_txt_clr)
 
         #PLOT SR WIND  
-        wind_ax.plot(kinem['srw'][0:11],  intrp['zINTRP'][0:11],  color=hodo_color[0], clip_on=True, linewidth=3, alpha=0.8, label='0-1 SR Wind')
-        wind_ax.plot(kinem['srw'][10:30], intrp['zINTRP'][10:30], color=hodo_color[1], clip_on=True, linewidth=3, alpha=0.8, label='1-3 SR Wind')
+        wind_ax.plot(kinem['srw'][0:11],  intrp['zINTRP'][0:11],  color=hodo_color[0], clip_on=True, 
+                     linewidth=3, alpha=0.8, label='0-1 SR Wind')
+        wind_ax.plot(kinem['srw'][10:30], intrp['zINTRP'][10:30], color=hodo_color[1], clip_on=True, 
+                     linewidth=3, alpha=0.8, label='1-3 SR Wind')
         
         if ma.is_masked(kinem['eil_z'][0]) == False:
-            wind_ax.fill_between(x=(wind_min-5, wind_max+5), y1=kinem['eil_z'][0], y2=kinem['eil_z'][1], color='lightblue', alpha=0.2)
+            wind_ax.fill_between(x=(wind_min-5, wind_max+5), y1=kinem['eil_z'][0], y2=kinem['eil_z'][1], 
+                                 color='lightblue', alpha=0.2)
     else:
         warnings.warn("Storm Relative Wind could not be plotted (no valid storm motion/not enough data)", Warning)
         
     #################################################################
     
     
     
@@ -925,15 +1249,16 @@
     theta_ax.set_xlabel(' ')
 
     #PLOT THETA VS HGT
     plt.plot(intrp['thetaINTRP'], intrp['zINTRP'], color='purple', linewidth=3.5, alpha=0.5, clip_on=True)
     plt.plot(intrp['thetaeINTRP'], intrp['zINTRP'], color='purple', linewidth=3.5, alpha=0.8, clip_on=True)
 
     if ma.is_masked(kinem['eil_z'][0]) == False:
-        theta_ax.fill_between(x=(mintheta - 5, maxtheta + 5), y1=kinem['eil_z'][0], y2=kinem['eil_z'][1], color='lightblue', alpha=0.2)
+        theta_ax.fill_between(x=(mintheta - 5, maxtheta + 5), y1=kinem['eil_z'][0], 
+                              y2=kinem['eil_z'][1], color='lightblue', alpha=0.2)
     #################################################################
 
 
     
     #########################################################################
     ############################## TEXT PLOTS ###############################
     #########################################################################
@@ -958,15 +1283,16 @@
     #################################################################
     
     
     
     #################################################################
     ### THERMODYNAMICS ###
     #################################################################
-    plt.figtext( 0.17, 0.07, 'SR-ECAPE       CAPE         6CAPE         3CAPE          CIN            LCL', color=gen_txt_clr, weight='bold', fontsize=15)
+    plt.figtext( 0.17, 0.07, 'SR-ECAPE       CAPE         6CAPE         3CAPE          CIN            LCL', 
+                color=gen_txt_clr, weight='bold', fontsize=15)
     #SBCAPE
     plt.figtext( 0.13,  0.04, f"SB:", weight='bold',   fontsize=15, color=gen_txt_clr)
     plt.figtext( 0.17,  0.04, f"{mag(thermo['sb_ecape'])} J/kg",  fontsize=15, color='firebrick', weight='bold')
     plt.figtext( 0.235,  0.04, f"{mag(thermo['sbcape'])} J/kg",  fontsize=15, color='orangered', weight='bold')
     plt.figtext( 0.30,  0.04, f"{mag(thermo['sb6cape'])} J/kg", fontsize=15, color='orangered', weight='bold')
     plt.figtext( 0.364, 0.04, f"{mag(thermo['sb3cape'])} J/kg", fontsize=15, color='orangered', weight='bold')
     plt.figtext( 0.425, 0.04, f"{mag(thermo['sbcin'])} J/kg",   fontsize=15, color='orangered', weight='bold')
@@ -1029,17 +1355,17 @@
 
     plt.figtext( 0.54,  -0.08, f"6-9ₖₘ:", fontsize=15, color=gen_txt_clr, weight='bold',)
     plt.figtext( 0.541, -0.06, f"___", fontsize=15, color='black', alpha=0.64, weight='bold')
     plt.figtext( 0.585, -0.08, f"{mag(general['rh_6_9000'])} %", fontsize=15, color='forestgreen', alpha=0.64, weight='bold')
     plt.figtext( 0.62,  -0.08, f"{mag_round(general['w_6_9000'],1)} g/kg", fontsize=15, color='forestgreen',alpha=0.64, weight='bold')
 
     plt.figtext( 0.54,  -0.115, f"PWAT:", fontsize=15, weight='bold', color=gen_txt_clr)
-    plt.figtext( 0.588, -0.115, f"{mag(general['pwat'])} in", fontsize=15, color='darkgreen', ha='center', weight='bold')
-    plt.figtext( 0.625, -0.115, f"Tw:", fontsize=15, weight='bold', color=gen_txt_clr, ha='center')
-    plt.figtext( 0.65,  -0.115, f"{mag(general['wet_bulb'][0])} °C", fontsize=15, color='darkgreen', ha='center', weight='bold')
+    plt.figtext( 0.595, -0.115, f"{mag_round(general['pwat'], 2, mag=True)}in", fontsize=15, color='darkgreen', ha='center', weight='bold')
+    plt.figtext( 0.627, -0.115, f"WB:", fontsize=15, weight='bold', color=gen_txt_clr, ha='center')
+    plt.figtext( 0.655,  -0.115, f"{mag(general['wet_bulb'][0])} °C", fontsize=15, color='darkgreen', ha='center', weight='bold')
     #################################################################
     
     
     
     #################################################################
     ### KINEMATICS ###
     #################################################################   
@@ -1077,25 +1403,32 @@
     
     plt.figtext( 0.689, -0.08, f"6-9ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
     plt.figtext( 0.732, -0.08, f"{mag(kinem['shear_6_to_9000'])} kt", fontsize=15, color='navy', weight='bold')
     plt.figtext( 0.769, -0.08, f"{mag(kinem['srh_6_to_9000'])* met_per_sec:~P}", fontsize=15, color='navy', weight='bold')
     plt.figtext( 0.828, -0.08, f"{mag(kinem['srw_6_to_9000'])} kt", fontsize=15, color='navy', weight='bold')
     plt.figtext( 0.870, -0.08, f"{mag(kinem['swv_perc_6_to_9000'])}", fontsize=15, color='navy', weight='bold')
     plt.figtext( 0.905, -0.08, f"{mag_round(kinem['swv_6_to_9000'], 3)}", fontsize=15, color='navy', weight='bold')
+    
+    plt.figtext( 0.689, -0.11, f"EIL:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
+    plt.figtext( 0.732, -0.11, f"{mag(kinem['shear_eil'])} kt", fontsize=15, color='magenta', weight='bold')
+    plt.figtext( 0.769, -0.11, f"{mag(kinem['srh_eil'])* met_per_sec:~P}", fontsize=15, color='magenta', weight='bold')
+    plt.figtext( 0.828, -0.11, f"{mag(kinem['srw_eil'])} kt", fontsize=15, color='magenta', weight='bold')
+    plt.figtext( 0.870, -0.11, f"{mag(kinem['swv_perc_eil'])}", fontsize=15, color='magenta', weight='bold')
+    plt.figtext( 0.905, -0.11, f"{mag_round(kinem['swv_eil'], 3)}", fontsize=15, color='magenta', weight='bold')
     #################################################################
     
     
     
     #########################################################################
     ############################# PLOT EXTRAS ############################### 
     #########################################################################   
     plt.figtext( 0.125, 0.985, top_title, weight='bold', ha='left', fontsize=30, color=gen_txt_clr)
     plt.figtext( 0.125, 0.959, left_title, ha='left', fontsize=23, color=gen_txt_clr)
     plt.figtext( 1.22, 0.959, right_title, ha='right', fontsize=23, color=gen_txt_clr)
-    skewleg1 = skew.ax.legend(loc='upper left', framealpha=0.3, labelcolor=gen_txt_clr)
+    skewleg1 = skew.ax.legend(loc='upper left', framealpha=0.5, labelcolor=gen_txt_clr, facecolor=bckgrnd_clr)
     
     # plot author credit information 
     plt.figtext( 0.34, -0.105, 'SOUNDERPY VERTICAL PROFILE ANALYSIS TOOL', 
                 fontsize=20, ha='center', color='cornflowerblue', weight='bold', alpha=0.6)
     plt.figtext( 0.34, -0.125, '(C) KYLE J GILLETT | sounderpysoundings.anvil.app', 
                 fontsize=15, ha='center', color='cornflowerblue', weight='bold', alpha=0.6)
 
@@ -1118,20 +1451,21 @@
 
 
 
 
 
 
 
-
 #########################################################################
 ########################## SIMPLE SOUNDING ##############################
 
 def __simple_sounding(clean_data, color_blind, dark_mode, storm_motion='right_moving'):
     
+    warnings.warn("SounderPy's 'Simple Sounding' will be deprecated upon the next release (v3.0.5)", DeprecationWarning)
+    
     if dark_mode == True:
         gen_txt_clr = 'white'
         bckgrnd_clr = 'black'
         brdr_clr    = 'white'
         barb_clr    = 'white'
         shade_alpha = 0.06
         skw_ln_clr  = 'white'
@@ -1166,17 +1500,19 @@
                 fixed = int(param.m)
             except:
                 try: 
                     fixed = int(param)
                 except: fixed = param
         return fixed
     
-    def mag_round(param, dec):
+    def mag_round(param, dec, mag=False):
         if ma.is_masked(param):
             fixed = '---'
+        elif mag == True:
+            fixed = np.round(param.m, dec)
         else:
             fixed = np.round(param, dec)
         return fixed
 
 
     #################################################################
     ### SET UP THE DATA ###
@@ -1422,32 +1758,32 @@
     # define x and y min/max values from 'cleaned' and restructured u and v arrays
     x_min = u_hodo.min().m
     y_min = v_hodo.min().m
     x_max = u_hodo.max().m
     y_max = v_hodo.max().m
     # if statements to determine approprate x axis and y axis limits (to change dynamically with the data)
     if y_max >= 0:
-        y_Maxlimit = (y_max + 15)
+        y_Maxlimit = (y_max + 20)
     if y_max < 0:
-        y_Maxlimit = (y_max + 15)
+        y_Maxlimit = (y_max + 20)
 
     if x_max >= 0:
-        x_Maxlimit = (x_max + 15)
+        x_Maxlimit = (x_max + 20)
     if x_max < 0:
-        x_Maxlimit = (x_max + 15)
+        x_Maxlimit = (x_max + 20)
 
     if y_min >= 0:
-        y_Minlimit = (y_min - 40)
+        y_Minlimit = (y_min - 45)
     if y_min < 0:
-        y_Minlimit = (y_min - 40)
+        y_Minlimit = (y_min - 45)
 
     if x_min >= 0:
-        x_Minlimit = (x_min - 40)
+        x_Minlimit = (x_min - 45)
     if x_min < 0:
-        x_Minlimit = (x_min - 40)
+        x_Minlimit = (x_min - 45)
     #################################################################
         
         
     #################################################################
     ### CREATE HODOGRAPH OBJECT ###
     #################################################################
     hodo_ax = plt.axes((0.52, 0.45, 0.5, 0.5))
@@ -1492,14 +1828,19 @@
     for i in range(10,130,20):
         h.ax.annotate(str(i),(0,-i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=9,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
 
     h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', 
            color='white', alpha=1, markersize=30, clip_on=True, zorder=5)
     h.ax.annotate(str('.5'),(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']]),
                   weight='bold', fontsize=9, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+    
+    h.plot(intrp['uINTRP'][0],intrp['vINTRP'][0],marker='.', 
+           color='white', alpha=1, markersize=30, clip_on=True, zorder=5)
+    h.ax.annotate(str('sfc'),(intrp['uINTRP'][0],intrp['vINTRP'][0]),
+                  weight='bold', fontsize=5, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
 
     hgt_lvls = [] 
     for key in intrp['hgt_lvls'].keys():
         hgt_lvls.append(intrp['hgt_lvls'][key])
     hgt_lvls.pop(0) 
 
     for i in hgt_lvls[1::2]:
@@ -1510,64 +1851,64 @@
     
     
     #################################################################
     ### PLOT HODOGRAPH LINE ###
     #################################################################
     hodo_color = ['purple','red','darkorange','gold','#fff09f']
 
-    h.ax.plot(intrp['uINTRP'][0:10+1],   intrp['vINTRP'][0:10+1],   color=hodo_color[0], linewidth=5, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][10:30+1],  intrp['vINTRP'][10:30+1],  color=hodo_color[1], linewidth=5, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][30:60+1],  intrp['vINTRP'][30:60+1],  color=hodo_color[2], linewidth=5, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][60:90+1],  intrp['vINTRP'][60:90+1],  color=hodo_color[3], linewidth=5, clip_on=True)
-    h.ax.plot(intrp['uINTRP'][90:120+1], intrp['vINTRP'][90:120+1], color=hodo_color[4], linewidth=5, clip_on=True) 
+    h.ax.plot(intrp['uINTRP'][0:10+1],   intrp['vINTRP'][0:10+1],   color=hodo_color[0], linewidth=5, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][10:30+1],  intrp['vINTRP'][10:30+1],  color=hodo_color[1], linewidth=5, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][30:60+1],  intrp['vINTRP'][30:60+1],  color=hodo_color[2], linewidth=5, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][60:90+1],  intrp['vINTRP'][60:90+1],  color=hodo_color[3], linewidth=5, zorder=4, clip_on=True)
+    h.ax.plot(intrp['uINTRP'][90:120+1], intrp['vINTRP'][90:120+1], color=hodo_color[4], linewidth=5, zorder=4, clip_on=True) 
     #################################################################
     
     
     
     #################################################################
     ### ADD HODOGRAPH ANNOTATION ###
     #################################################################
     if ma.is_masked(kinem['sm_rm']) == False:
         # BUNKERS STORM MOTION
-        h.ax.text((kinem['sm_rm'][0]+0.5), (kinem['sm_rm'][1]-0.5), 'RM', weight='bold', ha='left', fontsize=10, alpha=0.9, color=gen_txt_clr)
-        h.ax.text((kinem['sm_lm'][0]+0.5), (kinem['sm_lm'][1]-0.5), 'LM', weight='bold', ha='left', fontsize=10, alpha=0.9, color=gen_txt_clr)
-        h.ax.text((kinem['sm_mw'][0]+0.5), (kinem['sm_mw'][1]-0.5), 'MW', weight='bold', ha='left', fontsize=10, alpha=0.9, color=gen_txt_clr)
+        h.ax.text((kinem['sm_rm'][0]+0.5), (kinem['sm_rm'][1]-0.5), 'RM', weight='bold', ha='left', fontsize=10, alpha=0.9, zorder=7, color=gen_txt_clr)
+        h.ax.text((kinem['sm_lm'][0]+0.5), (kinem['sm_lm'][1]-0.5), 'LM', weight='bold', ha='left', fontsize=10, alpha=0.9, zorder=7, color=gen_txt_clr)
+        h.ax.text((kinem['sm_mw'][0]+0.5), (kinem['sm_mw'][1]-0.5), 'MW', weight='bold', ha='left', fontsize=10, alpha=0.9, zorder=7, color=gen_txt_clr)
     
     if ma.is_masked(kinem['sm_u']) == False:
         # DEVIANT TORNADO MOTION
-        h.ax.text(kinem['dtm'][0], (kinem['dtm'][1] + 2), 'DTM', weight='bold', fontsize=8, color='brown', ha='center')
-        h.plot(kinem['dtm'][0], kinem['dtm'][1], marker='v', color='brown', markersize=5, alpha=0.8, ls='', label='DEVIANT TORNADO MOTION')
+        h.ax.text(kinem['dtm'][0], (kinem['dtm'][1] + 2), 'DTM', weight='bold', fontsize=8, color='brown', zorder=7, ha='center')
+        h.plot(kinem['dtm'][0], kinem['dtm'][1], marker='v', color='brown', markersize=5, alpha=0.8, ls='', zorder=7, label='DEVIANT TORNADO MOTION')
     
         # ADD SM POINT IF ITS A CUSTOM STORM MOTION
         if str(type(storm_motion)) == "<class 'list'>":
-            h.ax.text((kinem['sm_u']+0.5), (kinem['sm_v']-0.5), 'SM', weight='bold', ha='left', fontsize=10, alpha=0.9, color=gen_txt_clr)
+            h.ax.text((kinem['sm_u']+0.5), (kinem['sm_v']-0.5), 'SM', weight='bold', ha='left', fontsize=10, alpha=0.9, zorder=7, color=gen_txt_clr)
         
         h.ax.arrow(0,0,kinem['sm_u']-0.3, kinem['sm_v']-0.3, linewidth=2, color=gen_txt_clr, alpha=0.2, 
-               label='SM Vector', length_includes_head=True, head_width=0.5)
+               label='SM Vector', length_includes_head=True, zorder=6.5, head_width=0.5)
 
     
     # EFFECTIVE INFLOW LAYER SRH FILL
     if ma.is_masked(kinem['eil_z'][0]) == False:
         
         ebot = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]), (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][0])]),  
-                 linestyle='--', linewidth=2.3, alpha=0.5, color='lightblue', label='Effective Inflow Layer')
+                 linestyle='-', linewidth=1.5, alpha=0.8, zorder=2, color='lightblue', label='Effective Inflow Layer')
         etop = h.ax.plot((kinem['sm_u'], intrp['uINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]), (kinem['sm_v'], intrp['vINTRP'][find_nearest(intrp['zINTRP'],kinem['eil_z'][1])]),  
-                 linestyle='--', linewidth=2.3, alpha=0.5, color='lightblue')
+                 linestyle='-', linewidth=1.5, alpha=0.8, zorder=2, color='lightblue')
         fill_srh = h.ax.fill(np.append(intrp['uINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_u']), 
                              np.append(intrp['vINTRP'][find_nearest(intrp['zINTRP'], kinem['eil_z'][0]):find_nearest(intrp['zINTRP'], kinem['eil_z'][1])+1], kinem['sm_v']),
-                             'lightblue',alpha=0.1, label='EIL SRH')
+                             'lightblue', zorder=2, alpha=0.03, label='EIL SRH')
     else:
         fill_srh = h.ax.fill(np.append(intrp['uINTRP'][find_nearest(intrp['zINTRP'], 0):find_nearest(intrp['zINTRP'], 3000)], kinem['sm_u']), 
                      np.append(intrp['vINTRP'][find_nearest(intrp['zINTRP'], 0):find_nearest(intrp['zINTRP'], 3000)], kinem['sm_v']),
-                     'lightblue',alpha=0.1, label='0-3 SRH')
+                     'lightblue',alpha=0.03, zorder=2, label='0-3 SRH')
     
     
     # MCS MOTION
-    h.ax.text(kinem['mcs'][0], kinem['mcs'][1], 'UP', weight='bold', fontsize=10, color='orange', ha='center', alpha=0.5, clip_on=True)
-    h.ax.text(kinem['mcs'][2], kinem['mcs'][3], 'DN', weight='bold', fontsize=10, color='orange', ha='center', alpha=0.5, clip_on=True)
+    h.ax.text(kinem['mcs'][0], kinem['mcs'][1], 'UP', weight='bold', fontsize=10, color='orange', ha='center', zorder=7, alpha=0.5, clip_on=True)
+    h.ax.text(kinem['mcs'][2], kinem['mcs'][3], 'DN', weight='bold', fontsize=10, color='orange', ha='center', zorder=7, alpha=0.5, clip_on=True)
     
     
     # STORM MOTION PRINTOUT
     if ma.is_masked(kinem['sm_u']) == False:
         speeds = []
         directions = []
             
@@ -1887,28 +2228,31 @@
     for i in range(10,130,20):
         h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
         h.ax.annotate(str(i),(-i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
         h.ax.annotate(str(i),(0,-i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
 
-    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', 
+        
+        
+    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', markeredgecolor='black',
            color='white', alpha=1, markersize=30, clip_on=True, zorder=5)
     h.ax.annotate(str('.5'),(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']]),
-                  weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+                  weight='bold', fontsize=11, color='black',xytext=(0.02,-5),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
 
     hgt_lvls = [] 
     for key in intrp['hgt_lvls'].keys():
         hgt_lvls.append(intrp['hgt_lvls'][key])
     hgt_lvls.pop(0) 
 
-    for i in hgt_lvls[1::2]:
-        h.plot(intrp['uINTRP'][i],intrp['vINTRP'][i], marker='.', color='white', alpha=1, markersize=30, zorder=5)
-        h.ax.annotate(str(int(round(intrp['zINTRP'][i]/1000,0))),(intrp['uINTRP'][i],intrp['vINTRP'][i]), 
-                      weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+    for lvl in hgt_lvls[1::2]:
+        if lvl < 130:
+            h.plot(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl], marker='.', color='white', markeredgecolor='black', alpha=1, markersize=30, zorder=5)
+            h.ax.annotate(str(int(round(intrp['zINTRP'][lvl]/1000,0))),(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl]), 
+                          weight='bold', fontsize=11, color='black',xytext=(0.02,-5),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=5.1) 
     #################################################################
     
     
     
     
     
     #################################################################
@@ -2640,15 +2984,15 @@
 
         if profile['site_info']['source'] == 'RAOB OBSERVED PROFILE':
             types.append(f"RAOB")
             locs.append(f"{profile['site_info']['site-id']}, {profile['site_info']['site-name']}")
             val_times.append(f"{profile['site_info']['valid-time'][3]}Z | {profile['site_info']['valid-time'][1]}-{profile['site_info']['valid-time'][2]}-{profile['site_info']['valid-time'][0]}")
             int_times.append(f"{profile['site_info']['valid-time'][3]}Z | {profile['site_info']['valid-time'][1]}-{profile['site_info']['valid-time'][2]}-{profile['site_info']['valid-time'][0]}")
 
-        if profile['site_info']['source'] == 'MODEL REANALYSIS PROFILE':
+        if profile['site_info']['source'] == 'MODEL REANALYSIS':
             types.append(f"{profile['site_info']['fcst-hour']} {profile['site_info']['model']}")
             locs.append(f"{profile['site_info']['site-latlon']}")
             val_times.append(f"{profile['site_info']['valid-time'][3]}Z | {profile['site_info']['valid-time'][1]}-{profile['site_info']['valid-time'][2]}-{profile['site_info']['valid-time'][0]}")
             int_times.append(f"{profile['site_info']['run-time'][3]}Z | {profile['site_info']['run-time'][1]}-{profile['site_info']['run-time'][2]}-{profile['site_info']['run-time'][0]}")
 
         if profile['site_info']['source'] == 'BUFKIT FORECAST PROFILE':
             types.append(f"{profile['site_info']['fcst-hour']} {profile['site_info']['model']}")
@@ -2903,28 +3247,29 @@
     for i in range(10,130,20):
         h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
         h.ax.annotate(str(i),(-i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
     for i in range(10,130,20):
         h.ax.annotate(str(i),(0,-i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=12,weight='bold',alpha=0.2,zorder=0, color=gen_txt_clr)
 
-    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', 
+    h.plot(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']],marker='.', markeredgecolor='black',
            color='white', alpha=1, markersize=30, clip_on=True, zorder=5)
     h.ax.annotate(str('.5'),(intrp['uINTRP'][intrp['hgt_lvls']['h05']],intrp['vINTRP'][intrp['hgt_lvls']['h05']]),
-                  weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+                  weight='bold', fontsize=11, color='black',xytext=(0.02,-5),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
 
     hgt_lvls = [] 
     for key in intrp['hgt_lvls'].keys():
         hgt_lvls.append(intrp['hgt_lvls'][key])
     hgt_lvls.pop(0) 
 
-    for i in hgt_lvls[1::2]:
-        h.plot(intrp['uINTRP'][i],intrp['vINTRP'][i], marker='.', color='white', alpha=1, markersize=30, zorder=5)
-        h.ax.annotate(str(int(round(intrp['zINTRP'][i]/1000,0))),(intrp['uINTRP'][i],intrp['vINTRP'][i]), 
-                      weight='bold', fontsize=12, color='black',xytext=(0,-3.2),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=6) 
+    for lvl in hgt_lvls[1::2]:
+        if lvl < 130:
+            h.plot(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl], marker='.', color='white', markeredgecolor='black', alpha=1, markersize=30, zorder=5)
+            h.ax.annotate(str(int(round(intrp['zINTRP'][lvl]/1000,0))),(intrp['uINTRP'][lvl],intrp['vINTRP'][lvl]), 
+                          weight='bold', fontsize=11, color='black',xytext=(0.02,-5),textcoords='offset pixels',horizontalalignment='center',clip_on=True, zorder=5.1) 
     #################################################################
     
     
     
     
     
     #################################################################
```

### Comparing `sounderpy-3.0.3/src/sounderpy/sounderpy.py` & `sounderpy-3.0.4.dev1/src/sounderpy/sounderpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 '''
     SOUNDERPY | Vertical Profile Data Retrieval and Analysis Tool For Python
     -------------------------------------------------------------------------
     An atmospheric science Python package that retrieves & visualizes vertical profile data for meteorological analysis. 
 
     THIS RELEASE
     -------
-    Version: 3.0.3 | March 2024
+    Version: 3.0.4 | May 2024
 
     DOCUMENTATION
     -------
     Docs: https://kylejgillett.github.io/sounderpy/
     Code: https://github.com/kylejgillett/sounderpy
     PyPi: https://pypi.org/project/sounderpy/
     Operational Site: https://sounderpysoundings.anvil.app/
@@ -62,15 +62,15 @@
     Created by Kyle J Gillett (@wxkylegillett) 2023, 2024
     
 '''
 
 citation_text = f"""
 ## ---------------------------------- SOUNDERPY ----------------------------------- ##
 ##          Vertical Profile Data Retrieval and Analysis Tool For Python            ##
-##                     v3.0.3 | Mar. 2024 | (C) Kyle J Gillett                      ##
+##                      v3.0.4 | May 2024 | (C) Kyle J Gillett                      ##
 ##                 Docs: https://kylejgillett.github.io/sounderpy/                  ##
 ## --------------------- THANK YOU FOR USING THIS PACKAGE! ------------------------ ##
 """
 print(citation_text)
 
 #########################################################################################################
 
@@ -816,15 +816,15 @@
             pflag=np.array(df['pflag'])
             tflag=np.array(df['tflag'])
             for old_key, new_key, unit in zip (old_keys, new_keys, units_list):
                 clean_data[new_key] = np.array(df.to_dict('list')[old_key])[zflag+pflag+tflag>=4]*units(unit)
             clean_data['site_info'] = {
                     'site-id'   : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['ID'].str.strip().values[0],
                     'site-name' : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['NAME'].str.strip().values[0],
-                    'site-lctn' : 'no-site-location',
+                    'site-lctn' : '',
                     'site-latlon' : get_latlon('igra', station),
                     'site-elv'  : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['EL(m)'].values[0],
                     'source'    : 'RAOB OBSERVED PROFILE',
                     'model'     : 'no-model',
                     'fcst-hour' : 'no-fcst-hour',
                     'run-time'  : ['none', 'none', 'none', 'none'],
                     'valid-time': [year, month, day, hour]}
@@ -914,15 +914,15 @@
     # GET ARCHIVE DATA FROM THE IEM SERVERS. CORRECT GFS & NAM MODEL NAMES
     # if date variables (year, month, day) are given, the user has 'selected' a 
     # archived forecast for the given date 
     else:
         if model not in ['gfs', 'nam', 'namnest', 'rap', 'hrrr']:
             raise ValueError(f"{model} is not a valid model option. Valid models include ['GFS', 'NAM', 'NAMNEST', 'RAP', 'HRRR']")
         if model == 'namnest':
-            model == 'nam4km'
+            model = 'nam4km'
         if model == 'gfs':
             model3 = 'gfs3' 
         else:
             model3 = model
         data_conn = f'https://mtarchive.geol.iastate.edu/{run_year}/{run_month}/{run_day}/bufkit/{run_hour}/{model}/{model3}_{station.lower()}.buf'  
 
 
@@ -951,16 +951,16 @@
     recordSounding = False
     
     # SET UP DATE / TIME OBJECTS FROM THE BUFKIT FILE
     run_time = buf_file[4][buf_file[4].index('TIME') + 7:(buf_file[4].index('TIME')+9)+9]
     run_dt = datetime(int(f'20{run_time[0:2]}'), int(run_time[2:4]), int(run_time[4:6]), int(run_time[7:9])) 
     fct_dt = run_dt + timedelta(hours = fcst_hour)
     hr_deltas = {
-         'gfs':[3,180], 'hrrr':[1,48],
-         'rap':[1,51],  'nam':[3,48],
+         'gfs':[1,180], 'hrrr':[1,48],
+         'rap':[1,51],  'nam':[1,48],
          'namnest':[1,60],  'nam4km':[1,60],
          'sref':[1,84],     'hiresw':[1,48]}
     stp_dt = fct_dt + timedelta(hours = hr_deltas[model][0])
     
     if hr_deltas[model][1] < fcst_hour:
             raise ValueError(f'Invalid forecast hour -- BUFKIT only stores up to F0{hr_deltas[model][1]} for the {str.upper(model)}')
     
@@ -1463,15 +1463,15 @@
 
 
 #####################
 # PLOTTTING FUNCTIONS  
 #########################################################################
 
 # Soundings 
-def build_sounding(clean_data, style='full', color_blind=False, dark_mode=False, storm_motion='right_moving', special_parcels=None, save=False, filename='sounderpy_sounding'):
+def build_sounding(clean_data, style='full', color_blind=False, dark_mode=False, storm_motion='right_moving', special_parcels=None, show_radar=True, radar_time='sounding', map_zoom=2, modify_sfc=None, save=False, filename='sounderpy_sounding'):
     
     '''
        Return a full sounding plot of SounderPy data, ``plt`` 
 
        :param clean_data: the dictionary of data to be plotted (see :doc:`gettingdata`)
        :type clean_data: dict, required
        :param style: may be `simple` or `full`. Default is `full`.
@@ -1492,17 +1492,17 @@
        :rtype: plt
     '''
     
     print(f'> SOUNDING PLOTTER FUNCTION --\n---------------------------------')
         
     if style == 'full':
         if save == True:
-            __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels).savefig(filename, bbox_inches='tight')
+            __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels, show_radar, radar_time, map_zoom, modify_sfc).savefig(filename, bbox_inches='tight')
         else:
-            __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels).show()
+            __full_sounding(clean_data, color_blind, dark_mode, storm_motion, special_parcels, show_radar, radar_time, map_zoom, modify_sfc).show()
     elif style == 'simple':
         if save == True:
             __simple_sounding(clean_data, color_blind, dark_mode, storm_motion).savefig(filename, bbox_inches='tight')
         else:
             __simple_sounding(clean_data, color_blind, dark_mode, storm_motion).show()
 
 
@@ -1627,15 +1627,15 @@
         
         
         
         
 # print out data to console
 def print_variables(clean_data):
     
-    sounding_params(clean_data).print_vals()
+    sounding_params(clean_data, storm_motion='right_moving', sfc_correction=None).print_vals()
     
 #############################################################################################################################
     
 
     
     
 ##################
```

### Comparing `sounderpy-3.0.3/src/sounderpy.egg-info/PKG-INFO` & `sounderpy-3.0.4.dev1/src/sounderpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.3
+Version: 3.0.4.dev1
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
-Author-email: "Kyle J Gillett, Central Michigan University" <kjgillett10@gmail.com>
+Author-email: "Kyle J Gillett, University of North Dakota" <kjgillett10@gmail.com>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
-Project-URL: My Website, https://kylegillettwx.wordpress.com/
+Project-URL: My Website, https://kylegillettphoto.com
 Keywords: meteorology,science,data-analysis,weather,forecasting
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cartopy>=0.21.0
 Requires-Dist: cdsapi>=0.6.1
 Requires-Dist: ecape-parcel>=1.2.0.2
-Requires-Dist: matplotlib<=3.7.1,>=3.3.0
+Requires-Dist: matplotlib>=3.3.0
 Requires-Dist: metpy>=1.5.1
 Requires-Dist: netcdf4>=1.6.4
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.2.0
-Requires-Dist: arm_pyart>=1.16.1
 Requires-Dist: siphon>=0.9
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: xarray>=0.18.0
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 </div>
 
 # SounderPy, the vertical profile data retrieval and analysis tool for Python
-LATEST VERSION: v3.0.3 |  RELEASED: March, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
+LATEST VERSION: v3.0.4 |  RELEASED: May, 2024  |  COPYRIGHT Kyle J Gillett, 2023, 2024
 
 A Python package that helps you to access and plot vertical profile data for meteorological analysis 
 
 [![PyPI Package](https://img.shields.io/pypi/v/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://github.com/kylejgillett/sounderpy/blob/main/LICENSE.txt)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
@@ -173,29 +173,29 @@
    <img src="https://kylejgillett.github.io/sounderpy/_images/example-hodograph_dark.png" width="600">
    </div>
 
 ### To learn more about what you can do with SounderPy, [check out the documentation](https://kylejgillett.github.io/sounderpy/)
 ------
 
 ## AUTHORS AND CONTRIBUTORS
-### **AUTHOR: Kyle J Gillett, Central Michigan University** 
+### **AUTHOR: Kyle J Gillett, University of North Dakota** 
 ##### *CONTRIBUTOR: Scott Thomas, NWS Grand Rapids | VWP Hodograph, Buoy-sites listing*
 ##### *CONTRIBUTOR: Amelia R H Urquhart, University of Oklahoma | ecape-parcels library*
 ##### *CONTRIBUTOR: Daryl Herzmann, Iowa State University | SounderPy Feedstock for conda-forge*
 
 ------
 
 
 ## CITING SOUNDERPY
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10443609.svg)](https://doi.org/10.5281/zenodo.10443609)
 
 
 in AMS format:
 
-- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.3). Py-Pi, https://pypi.org/project/sounderpy/
+- Gillett, K., 2024: SounderPy: Vertical Profile Data Retrieval & Analysis Tool for Python (Version 3.0.4). Py-Pi, https://pypi.org/project/sounderpy/
 
 ------
 
 
 
 ## REFERENCES
 - Harris, C.R., Millman, K.J., van der Walt, S.J. et al. Array programming with NumPy. Nature 585, 357–362 (2020). DOI: 10.1038/s41586-020-2649-2.
```

### Comparing `sounderpy-3.0.3/src/sounderpy.egg-info/SOURCES.txt` & `sounderpy-3.0.4.dev1/src/sounderpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

