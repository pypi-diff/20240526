# Comparing `tmp/assessment_episode_matcher-0.3.1.tar.gz` & `tmp/assessment_episode_matcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assessment_episode_matcher-0.3.1.tar", last modified: Fri May 24 22:36:06 2024, max compression
+gzip compressed data, was "assessment_episode_matcher-0.4.0.tar", last modified: Sun May 26 01:12:40 2024, max compression
```

## Comparing `assessment_episode_matcher-0.3.1.tar` & `assessment_episode_matcher-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:06.013474 assessment_episode_matcher-0.3.1/
--rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      523 2024-05-24 22:36:06.013474 assessment_episode_matcher-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-24 22:35:01.000000 assessment_episode_matcher-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.772793 assessment_episode_matcher-0.3.1/assessment_episode_matcher/
--rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/audits.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.842630 assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/__init__.py
--rw-rw-rw-   0        0        0     3799 2024-05-23 04:08:55.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/az_blob_query.py
--rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/az_tables_query.py
--rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.853477 assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/
--rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/__init__.py
--rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/audit.py
--rw-rw-rw-   0        0        0      604 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/episodes.py
--rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/data_config.py
--rw-rw-rw-   0        0        0     5365 2024-05-17 19:24:47.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.867480 assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/
--rw-rw-rw-   0        0        0     1615 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/NADAbase.py
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/__init__.py
--rw-rw-rw-   0        0        0     2393 2024-05-24 22:30:10.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/main.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.893780 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/aod.py
--rw-rw-rw-   0        0        0    10886 2024-05-24 22:29:38.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/assessments.py
--rw-rw-rw-   0        0        0     6886 2024-05-24 22:28:14.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/episodes.py
--rw-rw-rw-   0        0        0     2941 2024-05-23 02:41:28.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/main.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.925336 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/__init__.py
--rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/date_checks.py
--rw-rw-rw-   0        0        0     5688 2024-05-18 20:56:49.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/errors.py
--rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/increasing_slack.py
--rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/main.py
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/matching_stats.py
--rw-rw-rw-   0        0        0     1993 2024-05-19 23:10:24.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/mytypes.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.943108 assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/__init__.py
--rw-rw-rw-   0        0        0     4852 2024-05-24 21:59:34.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/bootstrap.py
--rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/log_management.py
--rw-rw-rw-   0        0        0     8955 2024-05-24 22:33:21.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/test_surveytxt.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:05.952333 assessment_episode_matcher-0.3.1/assessment_episode_matcher/tests/
--rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/tests/matching_test.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:06.000608 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/base.py
--rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/ccare_to_aztable.py
--rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/df_ops_base.py
--rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/dtypes.py
--rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/environment.py
--rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/fromstr.py
--rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/group_utils.py
--rw-rw-rw-   0        0        0    11492 2024-05-24 22:30:29.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/io.py
--rw-rw-rw-   0        0        0       21 2024-05-24 22:34:24.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher/version.py
-drwxrwxrwx   0        0        0        0 2024-05-24 22:36:06.010431 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/
--rw-rw-rw-   0        0        0      523 2024-05-24 22:36:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2242 2024-05-24 22:36:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 22:36:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-24 22:36:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-24 22:36:05.000000 assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 22:36:06.018701 assessment_episode_matcher-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.569871 assessment_episode_matcher-0.4.0/
+-rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      523 2024-05-26 01:12:40.566872 assessment_episode_matcher-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-24 22:35:01.000000 assessment_episode_matcher-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.263395 assessment_episode_matcher-0.4.0/assessment_episode_matcher/
+-rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/audits.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.338348 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/__init__.py
+-rw-rw-rw-   0        0        0     4487 2024-05-26 00:55:49.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_blob_query.py
+-rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_tables_query.py
+-rw-rw-rw-   0        0        0     1067 2024-05-26 01:04:22.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/file_types.py
+-rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.362000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/__init__.py
+-rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/audit.py
+-rw-rw-rw-   0        0        0      604 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/episodes.py
+-rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_config.py
+-rw-rw-rw-   0        0        0     5365 2024-05-17 19:24:47.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.377893 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/
+-rw-rw-rw-   0        0        0     1615 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/NADAbase.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/__init__.py
+-rw-rw-rw-   0        0        0     2409 2024-05-26 01:03:13.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.410041 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/__init__.py
+-rw-rw-rw-   0        0        0    13006 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/aod.py
+-rw-rw-rw-   0        0        0     8834 2024-05-26 01:07:05.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/assessments.py
+-rw-rw-rw-   0        0        0     6726 2024-05-26 00:23:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/episodes.py
+-rw-rw-rw-   0        0        0     2941 2024-05-23 02:41:28.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.451591 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/__init__.py
+-rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/date_checks.py
+-rw-rw-rw-   0        0        0     5697 2024-05-26 01:09:01.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/errors.py
+-rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/increasing_slack.py
+-rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/main.py
+-rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/matching_stats.py
+-rw-rw-rw-   0        0        0     1993 2024-05-19 23:10:24.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/mytypes.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.471242 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/__init__.py
+-rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/bootstrap.py
+-rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/log_management.py
+-rw-rw-rw-   0        0        0     8652 2024-05-26 01:04:25.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/test_surveytxt.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.485705 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/
+-rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/matching_test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.547697 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/base.py
+-rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/ccare_to_aztable.py
+-rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/df_ops_base.py
+-rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/dtypes.py
+-rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/environment.py
+-rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/fromstr.py
+-rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/group_utils.py
+-rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/io.py
+-rw-rw-rw-   0        0        0       21 2024-05-26 01:12:15.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/version.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.561874 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:12:40.570870 assessment_episode_matcher-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.4.0/setup.py
```

### Comparing `assessment_episode_matcher-0.3.1/LICENSE` & `assessment_episode_matcher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/PKG-INFO` & `assessment_episode_matcher-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.3.1
+Version: 0.4.0
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.3.1/README.md` & `assessment_episode_matcher-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/az_blob_query.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_blob_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import os
+
 import logging
 from typing import Any
-from io import BytesIO, StringIO
-import tempfile
+from io import BytesIO
 import pandas as pd
 from azure.storage.blob import BlobServiceClient #, BlobClient, ContainerClient
-from assessment_episode_matcher.utils.environment import ConfigKeys, ConfigManager
 
+from assessment_episode_matcher.utils.environment import ConfigKeys, ConfigManager
+from assessment_episode_matcher.azutil.file_types import BlobCSVFilePrepper, BlobParquetFilePrepper
 # import mylogging
 
 # logging = mylogging.get('azure.storage')
 
+
 class AzureBlobQuery(object):
   def __init__(self):
       config = ConfigManager().config
     
       # self.connection_string = str(config.get(ConfigKeys.AZURE_STORAGE_CONNECTION_STRING,"Help"))
       self.connection_string = str(config.get(ConfigKeys.AZURE_BLOB_CONNECTION_STRING.value,"Help"))
       
@@ -51,47 +52,66 @@
       
       except Exception as e:
         # Log the exception
         logging.error(f"An error occurred while loading data from Blob Storage: {str(e)}")
         # You may want to display a user-friendly message in the Streamlit app
         # st.warning("An error occurred while loading the data. Please try again later.")
         return None       
-      
-  def _get_parquet(self, df:pd.DataFrame) -> bytes:
-    with tempfile.TemporaryDirectory() as temp_dir:
-        temp_file_path = os.path.join(temp_dir, "temp.parquet")
-        df.to_parquet(temp_file_path, engine="pyarrow")
-
-        # Read the Parquet file into memory
-        with open(temp_file_path, "rb") as file:
-            parquet_data = file.read()
-            return parquet_data
-
 
 
   def write_data(self, container_name:str, blob_url:str
                  , data:pd.DataFrame) -> dict[str, Any]:
-    
-    # csv_buffer = StringIO()
-    # data.to_csv(csv_buffer, index=False)
-    
 
-    # Define the blob client
-    # container_name = "atom-matching"
-    # blob_name = f"{container_name}/{blob_url}"
     blob_client = self.blob_service_client.get_blob_client(container=container_name
                                                       , blob=blob_url)
-    pq_data = self._get_parquet(data)
-    result_dict = blob_client.upload_blob(pq_data, overwrite=True)
-    # Upload the CSV to blob storage
-    # result_dict = blob_client.upload_blob(csv_buffer.getvalue()
-    #                                       , overwrite=True)
+    if blob_url[-3:] =='csv':
+      p = BlobCSVFilePrepper()
+      file = p.get_file_for_blob(data)
+    else:
+      p = BlobParquetFilePrepper()
+      file = p.get_file_for_blob(data)
+       
+    result_dict = blob_client.upload_blob(file, overwrite=True)
+
     return result_dict 
 
-    # return func.HttpResponse(
-    #     "DataFrame stored in blob storage successfully.",
-    #     status_code=200
-    # )     
+
+
+  # def _get_parquet(self, df:pd.DataFrame) -> bytes:
+  #   with tempfile.TemporaryDirectory() as temp_dir:
+  #       temp_file_path = os.path.join(temp_dir, "temp.parquet")
+  #       df.to_parquet(temp_file_path, engine="pyarrow")
+
+  #       # Read the Parquet file into memory
+  #       with open(temp_file_path, "rb") as file:
+  #           parquet_data = file.read()
+  #           return parquet_data
+
+
+
+  # def write_data(self, container_name:str, blob_url:str
+  #                , data:pd.DataFrame) -> dict[str, Any]:
+    
+  #   # csv_buffer = StringIO()
+  #   # data.to_csv(csv_buffer, index=False)
+    
+
+  #   # Define the blob client
+  #   # container_name = "atom-matching"
+  #   # blob_name = f"{container_name}/{blob_url}"
+  #   blob_client = self.blob_service_client.get_blob_client(container=container_name
+  #                                                     , blob=blob_url)
+  #   pq_data = self._get_parquet(data)
+  #   result_dict = blob_client.upload_blob(pq_data, overwrite=True)
+  #   # Upload the CSV to blob storage
+  #   # result_dict = blob_client.upload_blob(csv_buffer.getvalue()
+  #   #                                       , overwrite=True)
+  #   return result_dict 
+
+  #   # return func.HttpResponse(
+  #   #     "DataFrame stored in blob storage successfully.",
+  #   #     status_code=200
+  #   # )     
        
 # data = load_data('path/to/yourfile.parquet')
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/az_tables_query.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_tables_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/azutil/helper.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/helper.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/audit.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/audit.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/configs/episodes.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/episodes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/data_config.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_config.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/data_prep.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_prep.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/NADAbase.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/NADAbase.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/exporters/main.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 #     path = self.config.get("location")
 #     if not path:
 #       raise FileNotFoundError("CSVExporter:No file-path was passed in")
     
 #     data.to_csv(f"{path}{data_name}.csv", index=False)
 
 
-class ParquetExporter(DataExporter):
+# class ParquetExporter(DataExporter):
 
-  def export_data(self, data_name:str, data:pd.DataFrame):
-    path = self.config.get("location")
-    if not path:
-      raise FileNotFoundError("ParquetExporter:No file-path was passed in")
+#   def export_data(self, data_name:str, data:pd.DataFrame):
+#     path = self.config.get("location")
+#     if not path:
+#       raise FileNotFoundError("ParquetExporter:No file-path was passed in")
     
-    data.to_parquet(f"{path}{data_name}.parquet", index=False)
+#     data.to_parquet(f"{path}{data_name}.parquet", index=False)
     
 
 class AzureBlobExporter(DataExporter):
   blobClient:AzureBlobQuery
 
   def __init__(self, container_name:str, config:Optional[dict]=None) -> None:
     if config:
@@ -49,16 +49,16 @@
     if hasattr(self, "config"):
       folder_path = self.config.get("location")
       if folder_path:
         full_path = f"{folder_path}/{data_name}"
   
     result = self.blobClient.write_data(container_name=self.container_name
                                         , blob_url=full_path
-                                        ,data=data)
-    print(result)
+                                        ,data=data)    
+    return result
     
 
 
 # class AuditExporter(DataExporter):
 #   container_prefix = "audit-matching"
 
 #   def __init__(self, config) -> None:
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/aod.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/aod.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/assessments.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/assessments.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,17 @@
      return df
   return df[df ['Program'].isin(filters['Program'])]
 
 
 
 def import_data(asmt_st:str, asmt_end:str
                 , file_source:FileSource
+                , prefix:str, suffix:str
                 ,purpose:Purpose, refresh:bool=True
-                ) -> tuple [pd.DataFrame, str]:
+                ) -> tuple[pd.DataFrame, str|None]:
   
   """
     Returns 2 values - the 2nd is a path to the cached to
 
     1. If processed file for the period exists:
         if asking to be refreshed, go to #2
         else return file
@@ -35,131 +36,86 @@
 
         if timestamp on raw.parquet is more recent than processed.parquet,
           (or same period processed.parquet does not exist)
           call process(raw_df) and write to /processed
 
     3. Raw Does NOT exist:
 
-
-
   """
 
-  processed_folder =  Bootstrap.get_path("processed_dir") / "ATOM"
-  source_folder = Bootstrap.get_path("in_dir") / "ATOM"
   filters = data_config.ATOM_DB_filters[purpose]
-  
-  # period_range = f"{asmt_st}-{asmt_end}"
-  fname = io.get_filename("ATOM", asmt_st
-                       , asmt_end, "AllPrograms")
-                       
-  processed_filepath = processed_folder.joinpath(f"{fname}.parquet") # f"{processed_folder}/{fname}"
-  
-  logging.info(f"Attempting to load processed data from {processed_filepath}")
 
+  # fname = io.get_filename(prefix, asmt_st
+  #                      , asmt_end, suffix)
+                   
   file_path, best_start_date, best_end_date = \
-    io.load_for_period(processed_folder
-                        , file_source
+    io.load_for_period(
+                       file_source
                           , asmt_st
                           , asmt_end
-                          ,prefix="ATOM_"
-                          , suffix="AllPrograms.parquet"
+                          ,prefix=f"{prefix}_"
+                           , suffix=f"{suffix}.parquet"
                           )
-  # if best_start_date and best_end_date:
-  #   fname = io.get_filename("ATOM", best_start_date.strftime("%Y%m%d")
-  #                       , best_end_date.strftime("%Y%m%d"), "AllPrograms")
-    
+      
   # TO DO check if recent or needs to be refreshed
   if file_path:
     processed_df = file_source.load_parquet_file_to_df(file_path)
     if has_data(processed_df):
       logging.debug("found & returning processed parquet file.")
-      return processed_df, ""
-    
-  logging.info ("Loading from Raw.parquet")
-  
-  file_path, best_start_date, best_end_date = \
-    io.load_for_period(source_folder
-                      , file_source
-                        , asmt_st
-                        , asmt_end
-                        , prefix="ATOM_"
-                        , suffix="AllPrograms.csv"
-                        )
-  
-  raw_df = file_source.load_csv_file_to_df(file_path, dtype=str)
-  # TO DO check if recent or needs to be refreshed
-  if not(isinstance(raw_df, type(None)) or raw_df.empty):
-    processed_df = io.process_assment(raw_df)
-    # use the same start and end date as the raw filename
-    if best_start_date and best_end_date:
-      # period_range = f"{best_start_date.strftime("%Y%m%d")}-{best_end_date.strftime("%Y%m%d")}"
-      fname = io.get_filename("ATOM", best_start_date.strftime("%Y%m%d")
-                      , best_end_date.strftime("%Y%m%d"), "AllPrograms")
-
-    processed_file = processed_folder.joinpath(f"{fname}.parquet")#  f"{processed_folder}/{fname}"
-    logging.warn("writing processed only to the local folder. ")
-    #TODO : this only writes to the local one.. need to write to blob
+      return processed_df ,  None
   
-    # io.write_parquet(processed_df,processed_file)
-
   else:
       logging.info("Raw file doesn't exist either. load from DB. " \
               + "\n Hardcoding 20160701 as start date and today as end date.")
       today = datetime.now()
       today_str = today.strftime('%Y%m%d')
       today_int = int(today_str)
       
-      raw_df = io.get_from_source("ATOM", 20160701
+      raw_df = io.get_from_source(prefix,  20160701
                                   , today_int, filters=filters)     
-      fname =   io.get_filename("ATOM", asmt_st
-                      , today_str, "AllPrograms")
-      preprocessed_file = source_folder.joinpath(f"{fname}.parquet")
-      # io.write_parquet(raw_df, preprocessed_file)
-      logging.warn("wrote pre-processed only to the local folder. ")
+      fname =   io.get_filename(prefix, asmt_st
+                      , today_str, suffix=suffix)
+
       processed_df = io.process_assment(raw_df)
-      return processed_df, str(processed_folder.joinpath(f"{fname}.parquet"))
-      
-  
-  
+      logging.warn("Must cache {fname}  ")
+      if not refresh:
+        return processed_df, fname #, str(processed_folder.joinpath(f"{fname}.parquet"))
       
+
   #   # get the last modified date of the file
   #   # get the last modified date of ATOMs in the period of interest (assessmentDate)
   #   # if the last modified date of the file is after the last modified date of ATOMs, then return the processed_df
   #   # else query Azure data to get the latest ATOMs and merge them into the processed_df and save to disk to override
-    
-  #   # TODO :
 
-  if not refresh:
-    logging.info("Returning cached (processed) assessment data.")
-    return processed_df, ""
-  # Data has been loaded in processed_df, but needs refresh. 
+ # Data has been loaded in processed_df, but needs refresh. 
   # refresh only processed file?
-  processed_file = processed_folder.joinpath(f"{fname}.parquet")# f"{processed_folder}/{fname}" 
+  # processed_file = processed_folder.joinpath(f"{fname}.parquet")# f"{processed_folder}/{fname}" 
   fetched_df, was_refreshed = io.get_data('ATOM'
                     ,int(asmt_st), int(asmt_end)
                     , processed_df
-                    , processed_file
+                    # , processed_file
                     , filters=filters                
                     , refresh=refresh)
   
   # if not has_data(atom_df):
   #    logging.info("Returning Empty Dataframe.")
   #    return pd.DataFrame()
   
   if was_refreshed:
     today = datetime.today()
     today_str = today.strftime("%Y%m%d")
     fname = io.get_filename("ATOM", asmt_st
                        , today_str, "AllPrograms")
-    processed_file = processed_folder.joinpath(f"{fname}.parquet")
-    # io.write_parquet(fetched_df, processed_file)
+
     processed_df = fetched_df
-    logging.info("Caching and returning refreshed assessment data.")
+    logging.info(f"Must Cache {fname} and returning refreshed assessment data.")
+  else:
+    logging.info("Tried to refersh , but Nothing was refreshed")
 
-  return processed_df, str(processed_file)
+  return processed_df, fname #, str(processed_file)
 
   
 # if __name__ == '__main__':
 #   from assessment_episode_matcher.utils.environment import ConfigManager
 #   ConfigManager.setup('dev')
 #   cfg = ConfigManager().config
 #   asmt_st, asmt_end = "20220101", "20240411"
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/episodes.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/episodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from assessment_episode_matcher.utils.df_ops_base import has_data
 from assessment_episode_matcher.utils import io
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
 
 # from utils.io import read_parquet, write_parquet
 
 def prepare(ep_df1:pd.DataFrame, start_date:str, end_date:str) -> pd.DataFrame:
-  processed_folder = Bootstrap.get_path("processed_dir")
+  # processed_folder = Bootstrap.get_path("processed_dir")
 
   ep_df = ep_df1[EpCfg.columns_of_interest].copy()
   ep_df['Program'] = ep_df['ESTABLISHMENT IDENTIFIER'].map(EstablishmentID_Program)
   
 #  convert_to_datetime(atom_df['AssessmentDate'], format='%Y%m%d')
   ep_df[EpCfg.date_cols[0]] = convert_to_datetime(ep_df[EpCfg.date_cols[0]],  format='%d%m%Y'
                                                   , fill_blanks=False)
@@ -43,70 +43,70 @@
 #   #   fname = io.get_filename("MDS", best_start_date.strftime("%Y%m%d")
 #   #                       , best_end_date.strftime("%Y%m%d"), "AllPrograms")
 #     return processed_df, fname
   
 
 
 
-def import_data(eps_st:str,  eps_end:str, file_source:FileSource, prefix:str, suffix:str) -> pd.DataFrame:
+def import_data(eps_st:str,  eps_end:str, file_source:FileSource
+                    , prefix:str, suffix:str) -> tuple  [pd.DataFrame, str|None]:
+                
+                 
   """
     Load processed episodes dataframe from disk
     If not available, load raw, process and save, and then return processed_df
     prefix: MDS
     suffix: AllPrograms
   """  
-  processed_folder = Bootstrap.get_path("processed_dir") / "MDS"
-  source_folder =  Bootstrap.get_path("in_dir") / "MDS"
-  fname =  f'{prefix}_{eps_st}-{eps_end}_{suffix}' #NSW_
+
+  # source_folder =  Bootstrap.get_path("in_dir") / "MDS"
+  # fname =  f'{prefix}_{eps_st}-{eps_end}_{suffix}' #NSW_
   # fname_eps =  f'{source_folder}{filename}' #NSW_MDS_1jan2020-31dec2023.csv'#TEST_NSWMDS.csv'
   
-  filepath = processed_folder.joinpath(f"{fname}.parquet")
-  logging.info(f"Attempting to load data from {filepath}")
-
+  # filepath = processed_folder.joinpath(f"{fname}.parquet")
+  # logging.info(f"Attempting to load data from {filepath}")
+  
   # processed_df, fname_final = get_data(source_folder, eps_st, eps_end)
-  file_path, best_start_date, best_end_date = io.load_for_period(processed_folder
-                          , file_source
+  file_path, best_start_date, best_end_date = io.load_for_period(
+                           file_source
                           , eps_st
                           , eps_end
-                          ,prefix="MDS_"
-                          , suffix="AllPrograms.parquet"
+                          ,prefix=f"{prefix}_"
+                          , suffix=f"{suffix}.parquet"
                           )
   if file_path:
     processed_df = file_source.load_parquet_file_to_df(file_path)
     # processed_df = io.read_parquet_to_df(Path(file_path))
     if not(isinstance(processed_df, type(None)) or processed_df.empty):
       logging.debug(f"found & returning parquet file. {file_path}")
-      return processed_df
+      return processed_df, None
   
-  filepath = source_folder.joinpath(f"{fname}.csv")
-  logging.info(f"Attempting to load data from {filepath}")
 
-  # processed_df, fname_final = get_data(source_folder, eps_st, eps_end)
-  file_path, best_start_date, best_end_date = io.load_for_period(source_folder
-                        , file_source 
+  file_path, best_start_date, best_end_date = io.load_for_period(
+                         file_source 
                           , eps_st
                           , eps_end
-                          ,prefix="MDS_"
-                          , suffix="AllPrograms.csv"
+                          ,prefix=f"{prefix}_"
+                           , suffix=f"{suffix}.csv"
                           )
   if not file_path:
     raise FileNotFoundError("No MDS file was found")
   
   raw_df = file_source.load_csv_file_to_df(file_path, dtype=str)
   # raw_df = io.read_csv_to_df(Path(file_path), dtype=str)
   if not has_data(raw_df):
     logging.info(f"No Raw episode Data. Returning empty. {file_path}")
-    return raw_df
+    return raw_df, None
   
   raw_df.dropna(subset=['START DATE'], inplace=True)
   # TODO: log the dropped episodes
   raw_df['END DATE'] = raw_df['END DATE'].apply(lambda x: blank_to_today_str(x))
 
   processed_df = prepare(raw_df, eps_st, eps_end)
-  return processed_df
+  return processed_df, file_path
 
 
 # def import_data(eps_st:str,  eps_end:str, file_source:FileSource, prefix:str, suffix:str) -> pd.DataFrame:
 #   """
 #     Load processed episodes dataframe from disk
 #     If not available, load raw, process and save, and then return processed_df
 #     prefix: MDS
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/importers/main.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/date_checks.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/date_checks.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/errors.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 
 def write_validation_results(errors_warnings:dict[str, pd.DataFrame]
                              , audit_exporter: DataExporter):
     
     for ew_type_name, errs_warns in errors_warnings.items():
       if utdf.has_data(errs_warns):
-        audit_exporter.export_data(ew_type_name, errs_warns)       
+        audit_exporter.export_data(f"{ew_type_name}.csv", errs_warns)       
        
     
 
     # if utdf.has_data(dates_ewdf):
     #   audit_exporter.export_data("dates_ew", dates_ewdf)
     #   # dates_ewdf.to_csv(f'{output_folder}dates_ewdf.csv'
     #   #                   , index=False)
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/increasing_slack.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/increasing_slack.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/main.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/matching/matching_stats.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/matching_stats.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/mytypes.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/mytypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/bootstrap.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,21 @@
 #     processed_dir = data_dir / 'processed'
 #     processed_dir.mkdir(exist_ok=True)
 
 #     return data_dir, in_dir, out_dir, ew_dir, processed_dir
 
 def setup_directories(root: Path, env:str=""):
     # suffix = config.get("env_suffix")
+    
     if env == 'dev' or env == 'test':
-        suffix = f"{os.sep}{env}"
-
-    data_dir = Path(f'{root}{os.sep}data{suffix}')
+        data_dir =  root / "data" / "dev"
+    else:
+      data_dir =  root / "data"
+       
+    #Path(f'{root}{os.sep}data{suffix}')
     # data_dir.mkdir(exist_ok=True)
     in_dir = data_dir / 'in'
     # in_dir.mkdir(exist_ok=True)
     out_dir = data_dir / 'out'
     # out_dir.mkdir(exist_ok=True)
     ew_dir = out_dir / 'errors_warnings'
     # ew_dir.mkdir(exist_ok=True)
@@ -79,31 +82,31 @@
 
   def __new__(cls):
     if cls._instance is None:
         cls._instance = super(Bootstrap, cls).__new__(cls)
         # cls._instance.env = 'local'
     return cls._instance
   
-  @classmethod
-  def __getattr__(cls, key) -> Any:
-      if key in cls.data:
-          return cls.data[key]
-      raise AttributeError(f"No attribute named '{key}' found")
-  
-  @classmethod
-  def __getitem__(cls, key: str) -> Any:
-      return cls.__getattr__(key)
+  # @classmethod
+  # def __getattr__(cls, key) -> Any:
+  #     if key in cls.data:
+  #         return cls.data[key]
+  #     raise AttributeError(f"No attribute named '{key}' found")
+  
+  # @classmethod
+  # def __getitem__(cls, key: str) -> Any:
+  #     return cls.__getattr__(key)
 
   @classmethod
   def get(cls, key: str, default=None) -> Any:
       return cls.data.get(key, default)
 
-  @classmethod
-  def get_path(cls, key: str, default=None) -> Path:
-      return Path(cls.data.get(key, default))
+  # @classmethod
+  # def get_path(cls, key: str, default=None) -> Path:
+  #     return Path(cls.data.get(key, default))
   
   @classmethod
   def set(cls, key:str, value:str):
       cls.data[key] = value
   
   @classmethod
   def set_dirs(cls, dirs:dict):
@@ -115,16 +118,16 @@
   @classmethod
   def setup(cls, root: Path, env:str=""):
       print("setting up config")
       cls.config = setup_config(root, env)
       
       print(".....Done setting up config")
 
-      dirs =  setup_directories(root, env)
-      cls.set_dirs(dirs)
+      # dirs =  setup_directories(root, env)
+      # cls.set_dirs(dirs)
 
       print("GOING to set up logging")
       # cls.logger, cls.today_log_dir = setup_logging(env)
       print("Done setting up logging")
       return cls
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/setup/log_management.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/log_management.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/test_surveytxt.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/test_surveytxt.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,47 +44,55 @@
         
 #     return st
     
 
 def main3():
     # TODO:
     # envinronemnt setup : Config setup, Expected Directories create, logging setup
-    bstrap = Bootstrap.setup(project_directory, env="dev")
+    bstrap = Bootstrap.setup(project_directory, env="prod")
     container = "atom-matching"
+    ep_folder, asmt_folder = "MDS", "ATOM"
+    
     cfg = bstrap.config #, bstrap.logger
     # ConfigManager.setup('dev')
     # cfg = ConfigManager().config
     slack_for_matching = int(cfg.get(ConfigKeys.MATCHING_NDAYS_SLACK.value, 7))
-    # refresh_assessments = False #cfg.get( ConfigKeys.REFRESH_ATOM_DATA, True )
-    # reporting_start = date(2024, 1, 1)
-    # reporting_end = date(2024, 3, 31)
-
+    
     reporting_start_str, reporting_end_str =  '20220101', '20240331'
+
     reporting_start, reporting_end = get_date_from_str (reporting_start_str,"%Y%m%d") \
                                       , get_date_from_str (reporting_end_str,"%Y%m%d")
 
     ep_file_source:FileSource = BlobFileSource(container_name=container
-                                            , folder_path="MDS")
+                                            , folder_path=ep_folder)
 
-    episode_df = EpisodesImporter.import_data(
+    episode_df, ep_cache_to_path = EpisodesImporter.import_data(
                             reporting_start_str, reporting_end_str
                             , ep_file_source
-                            , prefix="MDS", suffix="AllPrograms")
+                            , prefix=ep_folder, suffix="AllPrograms")
     if not utdf.has_data(episode_df):
       logging.error("No episodes")
       return json.dumps({"result":"no episode data"})
+    #TODO:
+    if ep_cache_to_path:
+      if ep_cache_to_path[-3:] =='csv':
+         ep_cache_to_path = f"{ep_cache_to_path[:-3]}parquet"
+         
+      exp = AzureBlobExporter(container_name=ep_file_source.container_name) #
+      exp.export_data(data_name=ep_cache_to_path, data=episode_df)   
                         # func.HttpResponse(body=json.dumps({"result":"no episode data"}),
                         #         mimetype="application/json", status_code=200)
 
     
     atom_file_source:FileSource = BlobFileSource(container_name=container
-                                            , folder_path="ATOM")
+                                            , folder_path=asmt_folder)
     atoms_df, atom_cache_to_path = ATOMsImporter.import_data(
                             reporting_start_str, reporting_end_str
                             , atom_file_source
+                            , prefix=asmt_folder, suffix="AllPrograms"
                             , purpose=Purpose.NADA, refresh=True)
     
     if atom_cache_to_path:
       exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
       exp.export_data(data_name=atom_cache_to_path, data=atoms_df)    
                             # , prefix="MDS", suffix="AllPrograms")
     if not utdf.has_data(atoms_df):
@@ -93,47 +101,35 @@
 
     a_df, e_df, inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom = \
       match_helper.get_data_for_matching2(episode_df, atoms_df
                                         , reporting_start, reporting_end, slack_for_matching=7)    
     if not utdf.has_data(a_df) or not utdf.has_data(e_df):
         print("No data to match. Ending")
         return None    
-    # e_df.to_csv('data/out/active_episodes.csv')
+   
     final_good, ew = match_helper.match_and_get_issues(e_df, a_df
                                           , inperiod_atomslk_notin_ep
                                           , inperiod_epslk_notin_atom, slack_for_matching)
 
     warning_asmt_ids  = final_good.SLK_RowKey.unique()
-    
-
-    # ae = AuditExporter(config={'location' : f'{bstrap.ew_dir}'})
-
-    # FIXME : Incorrect location goes to C:/aftab.jal within the blob srtorage :
+   
     ae = AzureBlobExporter(container_name=atom_file_source.container_name
-                           ,config={'location' : f'{Bootstrap.get_path("ew_dir")}'}) #
-    
-
+                           ,config={'location' : 'errors_warnings'})
 
     process_errors_warnings(ew, warning_asmt_ids, dk.client_id.value
                             , period_start=reporting_start
                             , period_end=reporting_end
                             , audit_exporter=ae)
   
 
     df_reindexed = final_good.reset_index(drop=True)
-    # df_reindexed.to_csv(f'{bstrap.out_dir}/reindexed.csv', index_label="index")
 
     exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-    exp.export_data(data_name="NADA/reindexed.parquet", data=df_reindexed)      
-    # try:
-    #   #  atom_file_source:FileSource = BlobFileSource(container_name="atom-matching"
-    #   #                                       , folder_path="ATOM")
-      
-    #   exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-    #   exp.export_data(data_name=atom_cache_to_path, data=df_reindexed)
+    exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.parquet", data=df_reindexed)      
+
     #   # logging.info("Result object", json.dumps(result))
        
     # finally:
     return df_reindexed
     # nada_importfile:Path = Path("data/out") / \
     #                        f"{reporting_start}_{reporting_end}_surveytxt.csv"
     # nada = generate_nada_export(df_reindexed, outfile=nada_importfile)
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/tests/matching_test.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/base.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/ccare_to_aztable.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/ccare_to_aztable.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/df_ops_base.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/df_ops_base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/dtypes.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/environment.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/environment.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/fromstr.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/fromstr.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/group_utils.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/group_utils.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher/utils/io.py` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,25 +179,25 @@
     
     return merged_updated, True
 
 
 #TODO : store /load parquet file from file/blob storage
 def get_data(table:str, start_date:int, end_date:int
              , cache_data:pd.DataFrame
-             , download_filepath:Path #= ""
+            #  , download_filepath:Path #= ""
              , filters:dict|None={}
              , refresh:bool=True) -> tuple[pd.DataFrame, bool]:
   #
   # get from ATOM Azure DB and save to disk
   #
   result_df = pd.DataFrame()
   was_refreshed = False
   if utdf.has_data(cache_data):
       # if os.path.exists(f"{download_filepath}"):
-      logging.info(f"Using cached data from {download_filepath}")
+      logging.info(f"Using cached data ")
       # result_df = read_parquet(f"{cache_or_download_filepath}")
 
       if refresh:
         result_df, was_refreshed = handle_refresh(cache_data
                                   , table
                                   , start_date
                                   , end_date
@@ -219,15 +219,15 @@
 
   return processed_df, True
 
 
 # TODO sort by the period: end_date  part ofthe file which would be the latest refreshed date
 # we want the most recent to be on top so when it matches against the func params, 
 # we get the cache file with the latest data
-def load_for_period(path: Path, file_source:FileSource, st_yyyymmdd: str
+def load_for_period(file_source:FileSource, st_yyyymmdd: str
                     , ed_yyyymmdd: str, prefix: str, suffix:str="") \
                       -> tuple[str, datetime|None, datetime|None]:
     """
     Load the file with the filename pattern if there are multiple limit matches to the one that is the best fit for the date range.
     
     :param path: The directory path where the files are located
     :param filename: The base filename pattern (e.g., "ATOM_")
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/PKG-INFO` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.3.1
+Version: 0.4.0
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.3.1/assessment_episode_matcher.egg-info/SOURCES.txt` & `assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 assessment_episode_matcher.egg-info/SOURCES.txt
 assessment_episode_matcher.egg-info/dependency_links.txt
 assessment_episode_matcher.egg-info/requires.txt
 assessment_episode_matcher.egg-info/top_level.txt
 assessment_episode_matcher/azutil/__init__.py
 assessment_episode_matcher/azutil/az_blob_query.py
 assessment_episode_matcher/azutil/az_tables_query.py
+assessment_episode_matcher/azutil/file_types.py
 assessment_episode_matcher/azutil/helper.py
 assessment_episode_matcher/configs/__init__.py
 assessment_episode_matcher/configs/audit.py
 assessment_episode_matcher/configs/episodes.py
 assessment_episode_matcher/exporters/NADAbase.py
 assessment_episode_matcher/exporters/__init__.py
 assessment_episode_matcher/exporters/main.py
```

### Comparing `assessment_episode_matcher-0.3.1/setup.py` & `assessment_episode_matcher-0.4.0/setup.py`

 * *Files identical despite different names*

