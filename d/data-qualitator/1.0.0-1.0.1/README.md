# Comparing `tmp/data_qualitator-1.0.0.tar.gz` & `tmp/data_qualitator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_qualitator-1.0.0.tar", last modified: Sat May 25 08:27:20 2024, max compression
+gzip compressed data, was "data_qualitator-1.0.1.tar", last modified: Sat May 25 08:33:58 2024, max compression
```

## Comparing `data_qualitator-1.0.0.tar` & `data_qualitator-1.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.086338 data_qualitator-1.0.0/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1069 2024-03-25 10:46:06.000000 data_qualitator-1.0.0/LICENSE.txt
--rw-r--r--   0 jaymilagroso   (501) staff       (20)    32692 2024-05-25 08:27:20.086502 data_qualitator-1.0.0/PKG-INFO
--rw-r--r--   0 jaymilagroso   (501) staff       (20)    30614 2024-03-31 11:20:46.000000 data_qualitator-1.0.0/README.md
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.080114 data_qualitator-1.0.0/data_qualitator/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:53:31.000000 data_qualitator-1.0.0/data_qualitator/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      398 2024-03-24 11:16:47.000000 data_qualitator-1.0.0/data_qualitator/factory.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1258 2024-03-31 02:04:20.000000 data_qualitator-1.0.0/data_qualitator/provider.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.081025 data_qualitator-1.0.0/data_qualitator/services/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:56:58.000000 data_qualitator-1.0.0/data_qualitator/services/__init__.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.081127 data_qualitator-1.0.0/data_qualitator/services/filesystem/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:57:07.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/__init__.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.081605 data_qualitator-1.0.0/data_qualitator/services/filesystem/csv/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:57:12.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/csv/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      427 2024-03-29 08:15:54.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/csv/builder.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1938 2024-03-24 11:16:47.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/csv/service.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.082110 data_qualitator-1.0.0/data_qualitator/services/filesystem/parquet/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:58:15.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/parquet/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      451 2024-03-29 08:15:36.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/parquet/builder.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1971 2024-03-24 12:44:37.000000 data_qualitator-1.0.0/data_qualitator/services/filesystem/parquet/service.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.082334 data_qualitator-1.0.0/data_qualitator/services/gcp/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 10:43:31.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/__init__.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.082438 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:00:37.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/__init__.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.082901 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:05:36.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      547 2024-03-29 08:16:03.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/builder.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     2253 2024-03-29 03:50:04.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/service.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.083625 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:14:21.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      571 2024-03-29 08:16:10.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/builder.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     2273 2024-03-29 03:50:04.000000 data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/service.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.084189 data_qualitator-1.0.0/data_qualitator/services/sql/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-29 23:07:44.000000 data_qualitator-1.0.0/data_qualitator/services/sql/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      366 2024-03-30 07:57:26.000000 data_qualitator-1.0.0/data_qualitator/services/sql/builder.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1788 2024-03-30 07:58:12.000000 data_qualitator-1.0.0/data_qualitator/services/sql/service.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.084581 data_qualitator-1.0.0/data_qualitator/utils/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-25 05:13:15.000000 data_qualitator-1.0.0/data_qualitator/utils/__init__.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      285 2024-03-31 02:02:49.000000 data_qualitator-1.0.0/data_qualitator/utils/constants.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.080897 data_qualitator-1.0.0/data_qualitator.egg-info/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)    32692 2024-05-25 08:27:20.000000 data_qualitator-1.0.0/data_qualitator.egg-info/PKG-INFO
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1646 2024-05-25 08:27:20.000000 data_qualitator-1.0.0/data_qualitator.egg-info/SOURCES.txt
--rw-r--r--   0 jaymilagroso   (501) staff       (20)        1 2024-05-25 08:27:20.000000 data_qualitator-1.0.0/data_qualitator.egg-info/dependency_links.txt
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      218 2024-05-25 08:27:20.000000 data_qualitator-1.0.0/data_qualitator.egg-info/requires.txt
--rw-r--r--   0 jaymilagroso   (501) staff       (20)       16 2024-05-25 08:27:20.000000 data_qualitator-1.0.0/data_qualitator.egg-info/top_level.txt
--rw-r--r--   0 jaymilagroso   (501) staff       (20)       84 2024-03-25 05:30:29.000000 data_qualitator-1.0.0/pyproject.toml
--rw-r--r--   0 jaymilagroso   (501) staff       (20)      875 2024-05-25 08:27:20.086845 data_qualitator-1.0.0/setup.cfg
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1976 2024-03-31 11:19:14.000000 data_qualitator-1.0.0/setup.py
-drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:27:20.086091 data_qualitator-1.0.0/tests/
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1741 2024-03-31 13:18:15.000000 data_qualitator-1.0.0/tests/test_filesystem_csv_service.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1765 2024-05-25 08:22:50.000000 data_qualitator-1.0.0/tests/test_filesystem_parquet_service.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     2016 2024-05-25 08:22:46.000000 data_qualitator-1.0.0/tests/test_googlecloudplatform_bigquery_service.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1875 2024-05-25 08:22:52.000000 data_qualitator-1.0.0/tests/test_googlecloudplatform_cloudstorage_csv.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     1899 2024-05-25 08:22:56.000000 data_qualitator-1.0.0/tests/test_googlecloudplatform_cloudstorage_parquet.py
--rw-r--r--   0 jaymilagroso   (501) staff       (20)     2131 2024-05-25 08:23:06.000000 data_qualitator-1.0.0/tests/test_postgresql_service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.935197 data_qualitator-1.0.1/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1069 2024-03-25 10:46:06.000000 data_qualitator-1.0.1/LICENSE.txt
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)    32572 2024-05-25 08:33:58.935292 data_qualitator-1.0.1/PKG-INFO
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)    30494 2024-05-25 08:33:33.000000 data_qualitator-1.0.1/README.md
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.928887 data_qualitator-1.0.1/data_qualitator/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:53:31.000000 data_qualitator-1.0.1/data_qualitator/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      398 2024-03-24 11:16:47.000000 data_qualitator-1.0.1/data_qualitator/factory.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1258 2024-03-31 02:04:20.000000 data_qualitator-1.0.1/data_qualitator/provider.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.929897 data_qualitator-1.0.1/data_qualitator/services/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:56:58.000000 data_qualitator-1.0.1/data_qualitator/services/__init__.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.930004 data_qualitator-1.0.1/data_qualitator/services/filesystem/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:57:07.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/__init__.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.930488 data_qualitator-1.0.1/data_qualitator/services/filesystem/csv/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:57:12.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/csv/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      427 2024-03-29 08:15:54.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/csv/builder.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1938 2024-03-24 11:16:47.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/csv/service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.931250 data_qualitator-1.0.1/data_qualitator/services/filesystem/parquet/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-24 08:58:15.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/parquet/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      451 2024-03-29 08:15:36.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/parquet/builder.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1971 2024-03-24 12:44:37.000000 data_qualitator-1.0.1/data_qualitator/services/filesystem/parquet/service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.931489 data_qualitator-1.0.1/data_qualitator/services/gcp/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 10:43:31.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/__init__.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.931591 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:00:37.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/__init__.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.932072 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:05:36.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      547 2024-03-29 08:16:03.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/builder.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     2253 2024-03-29 03:50:04.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.932642 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-28 11:14:21.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      571 2024-03-29 08:16:10.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/builder.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     2273 2024-03-29 03:50:04.000000 data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.933175 data_qualitator-1.0.1/data_qualitator/services/sql/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-29 23:07:44.000000 data_qualitator-1.0.1/data_qualitator/services/sql/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      366 2024-03-30 07:57:26.000000 data_qualitator-1.0.1/data_qualitator/services/sql/builder.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1788 2024-03-30 07:58:12.000000 data_qualitator-1.0.1/data_qualitator/services/sql/service.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.933498 data_qualitator-1.0.1/data_qualitator/utils/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        0 2024-03-25 05:13:15.000000 data_qualitator-1.0.1/data_qualitator/utils/__init__.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      285 2024-03-31 02:02:49.000000 data_qualitator-1.0.1/data_qualitator/utils/constants.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.929756 data_qualitator-1.0.1/data_qualitator.egg-info/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)    32572 2024-05-25 08:33:58.000000 data_qualitator-1.0.1/data_qualitator.egg-info/PKG-INFO
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1646 2024-05-25 08:33:58.000000 data_qualitator-1.0.1/data_qualitator.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)        1 2024-05-25 08:33:58.000000 data_qualitator-1.0.1/data_qualitator.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      218 2024-05-25 08:33:58.000000 data_qualitator-1.0.1/data_qualitator.egg-info/requires.txt
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)       16 2024-05-25 08:33:58.000000 data_qualitator-1.0.1/data_qualitator.egg-info/top_level.txt
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)       84 2024-03-25 05:30:29.000000 data_qualitator-1.0.1/pyproject.toml
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)      875 2024-05-25 08:33:58.935644 data_qualitator-1.0.1/setup.cfg
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1976 2024-05-25 08:33:42.000000 data_qualitator-1.0.1/setup.py
+drwxr-xr-x   0 jaymilagroso   (501) staff       (20)        0 2024-05-25 08:33:58.934922 data_qualitator-1.0.1/tests/
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1741 2024-03-31 13:18:15.000000 data_qualitator-1.0.1/tests/test_filesystem_csv_service.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1765 2024-05-25 08:22:50.000000 data_qualitator-1.0.1/tests/test_filesystem_parquet_service.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     2016 2024-05-25 08:22:46.000000 data_qualitator-1.0.1/tests/test_googlecloudplatform_bigquery_service.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1875 2024-05-25 08:22:52.000000 data_qualitator-1.0.1/tests/test_googlecloudplatform_cloudstorage_csv.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     1899 2024-05-25 08:22:56.000000 data_qualitator-1.0.1/tests/test_googlecloudplatform_cloudstorage_parquet.py
+-rw-r--r--   0 jaymilagroso   (501) staff       (20)     2131 2024-05-25 08:23:06.000000 data_qualitator-1.0.1/tests/test_postgresql_service.py
```

### Comparing `data_qualitator-1.0.0/LICENSE.txt` & `data_qualitator-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/PKG-INFO` & `data_qualitator-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_qualitator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data quality checking made easy!
 Home-page: https://github.com/jmilagroso/data_qualitator
 Download-URL: https://github.com/jmilagroso/data_qualitator/releases
 Author: Jay Milagroso
 Author-email: j.milagroso@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jmilagroso/data_qualitator/issues
@@ -47,21 +47,17 @@
 ```
 
 Upgrade pip to latest version
 ```cli
 pip install --upgrade pip
 ```
 
-Install "test version" of Data Quality test package.
+Install  Data Quality package.
 ```cli
-pip install \
--i https://test.pypi.org/simple/ \
---extra-index-url https://pypi.org/simple \
-data-qualitator \
---no-cache-dir
+pip install data-qualitator
  ```
 
 ## Create data quality instance
 
 Import modules
 ```python
 from data_qualitator import provider
```

### Comparing `data_qualitator-1.0.0/README.md` & `data_qualitator-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,17 @@
 ```
 
 Upgrade pip to latest version
 ```cli
 pip install --upgrade pip
 ```
 
-Install "test version" of Data Quality test package.
+Install  Data Quality package.
 ```cli
-pip install \
--i https://test.pypi.org/simple/ \
---extra-index-url https://pypi.org/simple \
-data-qualitator \
---no-cache-dir
+pip install data-qualitator
  ```
 
 ## Create data quality instance
 
 Import modules
 ```python
 from data_qualitator import provider
```

### Comparing `data_qualitator-1.0.0/data_qualitator/provider.py` & `data_qualitator-1.0.1/data_qualitator/provider.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/filesystem/csv/service.py` & `data_qualitator-1.0.1/data_qualitator/services/filesystem/csv/service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/filesystem/parquet/service.py` & `data_qualitator-1.0.1/data_qualitator/services/filesystem/parquet/service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/builder.py` & `data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/builder.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/csv/service.py` & `data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/csv/service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/builder.py` & `data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/builder.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/gcp/cloudstorage/parquet/service.py` & `data_qualitator-1.0.1/data_qualitator/services/gcp/cloudstorage/parquet/service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator/services/sql/service.py` & `data_qualitator-1.0.1/data_qualitator/services/sql/service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/data_qualitator.egg-info/PKG-INFO` & `data_qualitator-1.0.1/data_qualitator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-qualitator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Data quality checking made easy!
 Home-page: https://github.com/jmilagroso/data_qualitator
 Download-URL: https://github.com/jmilagroso/data_qualitator/releases
 Author: Jay Milagroso
 Author-email: j.milagroso@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jmilagroso/data_qualitator/issues
@@ -47,21 +47,17 @@
 ```
 
 Upgrade pip to latest version
 ```cli
 pip install --upgrade pip
 ```
 
-Install "test version" of Data Quality test package.
+Install  Data Quality package.
 ```cli
-pip install \
--i https://test.pypi.org/simple/ \
---extra-index-url https://pypi.org/simple \
-data-qualitator \
---no-cache-dir
+pip install data-qualitator
  ```
 
 ## Create data quality instance
 
 Import modules
 ```python
 from data_qualitator import provider
```

### Comparing `data_qualitator-1.0.0/data_qualitator.egg-info/SOURCES.txt` & `data_qualitator-1.0.1/data_qualitator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/setup.cfg` & `data_qualitator-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data_qualitator
-version = 1.0.0
+version = 1.0.1
 author = Jay Milagroso
 author_email = j.milagroso@gmail.com
 description = Data quality checking made easy!
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/jmilagroso/data_qualitator
 project_urls =
```

### Comparing `data_qualitator-1.0.0/setup.py` & `data_qualitator-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "data_qualitator.services.filesystem.parquet",
         "data_qualitator.services.gcp",
         "data_qualitator.services.gcp.cloudstorage",
         "data_qualitator.services.gcp.cloudstorage.csv",
         "data_qualitator.services.gcp.cloudstorage.parquet",
         "data_qualitator.services.sql",
     ],
-    version="1.0.0",
+    version="1.0.1",
     license="MIT",
     description="Data quality checking made easy!",
     author="Jay Milagroso",
     author_email="j.milagroso@gmail.com",
     url="https://github.com/jmilagroso/data_qualitator",
     download_url="https://github.com/jmilagroso/data_qualitator/releases",
     keywords=[
```

### Comparing `data_qualitator-1.0.0/tests/test_filesystem_csv_service.py` & `data_qualitator-1.0.1/tests/test_filesystem_csv_service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/tests/test_filesystem_parquet_service.py` & `data_qualitator-1.0.1/tests/test_filesystem_parquet_service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/tests/test_googlecloudplatform_bigquery_service.py` & `data_qualitator-1.0.1/tests/test_googlecloudplatform_bigquery_service.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/tests/test_googlecloudplatform_cloudstorage_csv.py` & `data_qualitator-1.0.1/tests/test_googlecloudplatform_cloudstorage_csv.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/tests/test_googlecloudplatform_cloudstorage_parquet.py` & `data_qualitator-1.0.1/tests/test_googlecloudplatform_cloudstorage_parquet.py`

 * *Files identical despite different names*

### Comparing `data_qualitator-1.0.0/tests/test_postgresql_service.py` & `data_qualitator-1.0.1/tests/test_postgresql_service.py`

 * *Files identical despite different names*

