# Comparing `tmp/satsure-core-test-0.3.2.tar.gz` & `tmp/satsure-core-test-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.3.2.tar", last modified: Sat May 25 15:58:35 2024, max compression
+gzip compressed data, was "satsure-core-test-0.3.3.tar", last modified: Sun May 26 13:40:48 2024, max compression
```

## Comparing `satsure-core-test-0.3.2.tar` & `satsure-core-test-0.3.3.tar`

### file list

```diff
@@ -1,76 +1,91 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.779073 satsure-core-test-0.3.2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.2/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-25 15:58:35.778843 satsure-core-test-0.3.2/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.2/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.768617 satsure-core-test-0.3.2/satsure_core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.768844 satsure-core-test-0.3.2/satsure_core/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.769702 satsure-core-test-0.3.2/satsure_core/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770152 satsure-core-test-0.3.2/satsure_core/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       69 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5986 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770632 satsure-core-test-0.3.2/satsure_core/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.770955 satsure-core-test-0.3.2/satsure_core/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773104 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773420 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3543 2024-05-25 15:57:49.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.773887 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1481 2024-05-24 12:42:18.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.774171 satsure-core-test-0.3.2/satsure_core/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.774857 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      671 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      431 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_get_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      711 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_reproject.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.775949 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_mask_cloud.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_merge.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_offset_file.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_resample_file.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.777642 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      578 2024-05-24 10:57:38.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      884 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.777938 satsure-core-test-0.3.2/satsure_core/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.2/satsure_core/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 15:58:35.778575 satsure-core-test-0.3.2/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2790 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-25 15:58:35.000000 satsure-core-test-0.3.2/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-25 15:58:35.779130 satsure-core-test-0.3.2/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-25 15:58:32.000000 satsure-core-test-0.3.2/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.896773 satsure-core-test-0.3.3/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.3/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 13:40:48.896565 satsure-core-test-0.3.3/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.3/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.879595 satsure-core-test-0.3.3/satsure_core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.879805 satsure-core-test-0.3.3/satsure_core/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.881157 satsure-core-test-0.3.3/satsure_core/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       98 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      780 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/extraction.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.882634 satsure-core-test-0.3.3/satsure_core/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      342 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1338 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5930 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_raster_ops.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1103 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_resolution.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.883168 satsure-core-test-0.3.3/satsure_core/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.883938 satsure-core-test-0.3.3/satsure_core/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.886712 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.887773 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3217 2024-05-25 16:40:08.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.888210 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-25 16:40:08.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.888652 satsure-core-test-0.3.3/satsure_core/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1191 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.889094 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2501 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/test_extraction.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.891842 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1063 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      328 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1360 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      312 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_resolution.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      896 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_is_same_size.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1620 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_mask.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_raster.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1485 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1412 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_vector.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1119 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1058 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_resolution.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.893575 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_mask_cloud.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_merge.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_offset_file.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_resample_file.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.895369 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.895676 satsure-core-test-0.3.3/satsure_core/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.896318 satsure-core-test-0.3.3/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3481 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-26 13:40:48.896829 satsure-core-test-0.3.3/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-26 13:38:31.000000 satsure-core-test-0.3.3/setup.py
```

### Comparing `satsure-core-test-0.3.2/PKG-INFO` & `satsure-core-test-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.2
+Version: 0.3.3
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/config.py` & `satsure-core-test-0.3.3/satsure_core/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/core/downloader.py` & `satsure-core-test-0.3.3/satsure_core/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/core/uploader.py` & `satsure-core-test-0.3.3/satsure_core/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.3.3/satsure_core/satelite/gdal/_raster_ops.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-import re
 import subprocess
 from pathlib import Path, PosixPath
 from tempfile import NamedTemporaryFile
-from typing import Optional, Union, Tuple,Dict
+from typing import Dict, Optional, Tuple, Union
+
+from osgeo import gdal
+from osgeo.gdalconst import GA_ReadOnly
 
 from satsure_core.satelite.core import Downloader
 
 
 def create_jpeg_image(
-        input_file: PosixPath,
-        output_file: Optional[str] = None,
-        bands_position: Tuple[int, int, int] = (3, 2, 1),
-        quality: int = 10,
-        target_resolution: int = 100):
+    input_file: PosixPath,
+    output_file: Optional[str] = None,
+    bands_position: Tuple[int, int, int] = (3, 2, 1),
+    quality: int = 10,
+    target_resolution: int = 100,
+):
     """Generates JPG image for a given tif
 
     Args:
         input_file (PosixPath): Path of the input file
         output_file (Optional[PosixPath], optional): Output path for the file. If not proivded, defaults to input file by changing extension. Defaults to None.
         quality (int): Compression ratio. (how much you want to compress)
         bands_position (Iterable[int, int, int], optional): List of rgb bands to use. Defaults to (3, 2, 1).
@@ -36,56 +39,55 @@
         f"QUALITY={int(quality)}",
         f"{input_file}",
         f"{output_file}",
     )
     subprocess.run(command, shell=False, capture_output=True)
 
 
-def reproject(
-        input_file: PosixPath,
-        output_file: PosixPath,
-        target_crs: str) -> None:
-    """
-     reproject the given polygon file
-    :param input_file:
-    :param output_file:
-    :param target_crs:
-    :return:
-    """
-    command = (
-        "gdalwarp", "-t_srs", f"{target_crs}", f"{input_file}",
-        f"{output_file}")
-    subprocess.run(command, shell=False, capture_output=True)
-
-
-def get_projection(file_path: str) -> str:
-    """
-    Function to get projection of file (Vector / Raster)
-    Currently supports only EPSG based projections
-    :param file_path:
-    :return:
+def is_same_size(raster_path_1: str, raster_path_2: str) -> bool:
     """
-    command = f"gdalsrsinfo {file_path} -e"
-    projection_str = subprocess.check_output(
-        command, stderr=subprocess.STDOUT, shell=True)
-
-    if "error" in projection_str.decode("utf-8")[:20].lower():
-        raise Exception(projection_str.decode("utf-8"))
+    Compare size (width, height) of two rasters
 
-    projection_code = re.findall(rb"\nEPSG:(.+?)\n", projection_str)
-    if not projection_code:
-        raise Exception(
-            "Cannot find projection, currently supports only " "EPSG based projections"
-        )
-
-    return f"EPSG:{projection_code[0].decode('utf-8')}"
+    :param raster_path_1: Path of first raster
+    :param raster_path_2: Path of second raster
+    :returns: Boolean value
+    """
+    raster_1 = gdal.Open(raster_path_1, GA_ReadOnly)
+    raster_2 = gdal.Open(raster_path_2, GA_ReadOnly)
+    return (raster_1.RasterXSize, raster_1.RasterYSize) == (
+        raster_2.RasterXSize,
+        raster_2.RasterYSize,
+    )
 
 
-def clip_with_shp(input_file: PosixPath, shp_path: PosixPath,
-                  output_folder: PosixPath, output_file: Union[str, None] = None) -> PosixPath:
+def mask(
+    raster_path: str,
+    mask_raster_path: str,
+    output_path: str,
+    no_data_value: int = 0,
+) -> None:
+    """
+    Mask a specified raster using another raster
+
+    :param raster_path: Path of raster that needs to be masked
+    :param mask_raster_path: Path of mask raster
+    :param output_path: Path of output raster
+    :param no_data_value: Value to use for `No Data` pixels (Defaults to 0)
+    """
+    command = f'gdal_calc.py -A {raster_path} -B {mask_raster_path} --outfile={output_path} --calc="A*B" --NoDataValue={no_data_value}'
+
+    subprocess.check_output(command, stderr=subprocess.STDOUT, shell=True)
+
+
+def clip_with_shp(
+    input_file: PosixPath,
+    shp_path: PosixPath,
+    output_folder: PosixPath,
+    output_file: Union[str, None] = None,
+) -> PosixPath:
     """
     Function to clip a raster file using a shapefile
 
     Parameters:
         input_file          - str, path to the raster file to be clipped
         shpFile             - str, path to the shapefile by which input_file should
                               be clipped
@@ -100,72 +102,76 @@
     suffix = input_file.split(".")[-1]
     s3_temp_file = False
     if input_file[:5] == "s3://":
         s3_temp_file = True
         input_file_local = NamedTemporaryFile(delete=False, suffix=f".{suffix}")
         Downloader().download_object_from_s3(input_file, input_file_local.name)
         if suffix == "jpg":
-            Downloader().download_object_from_s3(f"{input_file}.aux.xml",
-                                                 f"{input_file_local.name}.aux.xml")
+            Downloader().download_object_from_s3(
+                f"{input_file}.aux.xml", f"{input_file_local.name}.aux.xml"
+            )
         input_file = Path(input_file_local.name)
     else:
         input_file = Path(input_file)
     shp_path = Path(shp_path)
     output_folder = Path(output_folder)
     output_folder.mkdir(exist_ok=True, parents=True)
 
     file_name = input_file.name
 
     if output_file is not None:
         out_fname_path = Path(output_file)
         file_name = out_fname_path.stem + input_file.suffix
     outFile = output_folder.joinpath(file_name)
     command = (
-        "gdalwarp", "-q", "-srcnodata", "0", "-dstnodata", "0", "-overwrite",
-        f"{input_file}", f"{outFile}", "-cutline", f"{shp_path}",
-        f"-crop_to_cutline", "-co", "COMPRESS=LZW")
-    resp = subprocess.run(
-        command,
-        shell=False,
-        capture_output=True
+        "gdalwarp",
+        "-q",
+        "-srcnodata",
+        "0",
+        "-dstnodata",
+        "0",
+        "-overwrite",
+        f"{input_file}",
+        f"{outFile}",
+        "-cutline",
+        f"{shp_path}",
+        f"-crop_to_cutline",
+        "-co",
+        "COMPRESS=LZW",
     )
+    resp = subprocess.run(command, shell=False, capture_output=True)
     if s3_temp_file:
         input_file_local.close()
         input_file.unlink()
         if suffix == "jpg":
             Path(f"{input_file_local.name}.aux.xml").unlink()
     if resp.returncode != 0:
         raise ValueError()
 
     return outFile
 
 
-def get_file_info(input_file: PosixPath, crs: bool = False,
-                  stats: bool = True) -> Dict:
+def get_file_info(input_file: PosixPath, crs: bool = False, stats: bool = True) -> Dict:
     """
         Getting file info using rio
     :param input_file:
     :param crs:
     :param stats:
     :return:
     """
 
     result = {}
     if crs:
         command = ("rio", "info", f"--crs", f"{input_file}")
         resp = subprocess.run(command, shell=False, capture_output=True)
         if resp.returncode == 0:
-            result.update({"crs": resp.stdout.decode('utf-8').replace('\n', '')})
+            result.update({"crs": resp.stdout.decode("utf-8").replace("\n", "")})
     if stats:
         command = ("rio", "info", f"--stats", f"{input_file}")
         resp = subprocess.run(command, shell=False, capture_output=True)
         if resp.returncode == 0:
             stats = resp.stdout.decode("utf-8").replace("\n", "").split(" ")
-            result.update({
-                "stats": {
-                    "min": stats[0],
-                    "max": stats[1],
-                    "mean": stats[2]
-                }
-            })
+            result.update(
+                {"stats": {"min": stats[0], "max": stats[1], "mean": stats[2]}}
+            )
 
     return result
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/raster/raster.py` & `satsure-core-test-0.3.3/satsure_core/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/get_tiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 from os import environ
-from typing import List
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
 from satsure_core.satelite.config import DBSession
 
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.db = DBSession.create()
 
-    def fetch_tile_from_db(self, sql_query: text, geom_list: List) -> List:
+    def fetch_tile_from_db(self, sql_query, geom_):
         """
             Fetch tile from database
         :param sql_query:
-        :param geom_list:
+        :param geom_:
         :return:
         """
 
-        result = self.db.execute(
-            sql_query,
-            {
-                "minx": geom_list['minx'][0],
-                "miny": geom_list['miny'][0],
-                "maxx": geom_list['maxx'][0],
-                "maxy": geom_list['maxy'][0],
-            },
-        )
+        result = self.db.execute(sql_query,
+                                 {"geojson_geometry": str(geom_)})
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
         sql_query = text(
-            """SELECT tile FROM tileids
-                            WHERE ST_Intersects(
-                                geometry,
-                                ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
-                            )
-                            """)
-
-        rows = self.fetch_tile_from_db(sql_query, geom_list)
-        for row in rows:
-            tile_list.add(row[0])
+            f"""SELECT tile FROM tileids WHERE ST_Intersects( geometry,
+                                            ST_GeomFromGeoJSON(:geojson_geometry)) """
+        )
+
+        for geom_ in geom_list:
+            rows = self.fetch_tile_from_db(sql_query, geom_)
+            for row in rows:
+                tile_list.add(row[0])
 
         tile_list = list(tile_list)
         self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/conftest.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,7 +28,13 @@
     return polygon
 
 
 @pytest.fixture
 def datadir(tmp_path):
     """Fixture to provide access to the test data directory."""
     return Path(__file__).parent / "raster" / "testdata"
+
+
+@pytest.fixture
+def extraction_testdata_dir():
+    """Provide the directory containing test data for extraction"""
+    return Path(__file__).parent / "core" / "testdata" / "extraction"
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 from pathlib import Path
 
 from satsure_core.satelite.gdal import create_jpeg_image
 
 
 class TestCreateJPEGImage:
     """create JPEG Images"""
@@ -19,7 +20,17 @@
         )
 
         assert (
             output_file.suffix.lower() == ".jpg"
             or output_file.suffix.lower() == ".jpeg"
         )
         output_file.unlink()
+
+    def test_output_file_is_none(self, datadir):
+        input_file = datadir / "input1.tif"
+        expected_output_file = datadir / "input1.jpg"
+
+        assert not os.path.isfile(str(expected_output_file))
+        create_jpeg_image(input_file=input_file, bands_position=("1"))
+        assert os.path.isfile(str(expected_output_file))
+
+        expected_output_file.unlink()
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/gdal/test_reproject.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 import rasterio
-from satsure_core.satelite.gdal import reproject
+
+from satsure_core.satelite.gdal import reproject_raster
 
 
 class TestReprojectRaster:
     """test reproject of the raster"""
 
     def test_reproject_raster(self, datadir: Path) -> None:
         """_summary_
@@ -14,11 +15,13 @@
             datadir (Path): _description_
             tmp_path (Path): _description_
         """
 
         input_file = datadir / "input1.tif"
         output_file = datadir / "output_reproject.tif"
         target_crs = "EPSG:4326"
-        reproject(input_file=input_file, output_file=output_file, target_crs=target_crs)
+        reproject_raster(
+            input_file=input_file, output_file=output_file, target_crs=target_crs
+        )
         with rasterio.open(output_file) as src:
             assert src.crs.to_string() == target_crs
         Path(output_file).unlink()
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_mask_cloud.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_mask_cloud.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_merge.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_merge.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_normalised_difference_index.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_normalised_difference_index.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_offset_file.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_offset_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/raster/test_resample_file.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_resample_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,33 @@
+import datetime
 from pathlib import Path
 
-from satsure_core.satelite.sentinel2 import S2L1CUrls
+from satsure_core.satelite.sentinel2 import S2L2AUrls
 
 
-class TestS2L1CUrls:
+class TestS2L2AUrls:
 
     def test_get_urls(self, monkeypatch):
         """
             Testcase to check get_urls data
         :param monkeypatch:
         :return:
         """
         params = {"tile_code": "43QDB",
                   "from_date": "2023-05-04",
                   "download_path": Path("sample/temp")}
 
-        obj = S2L1CUrls()
+        obj = S2L2AUrls()
         result = obj.get_urls(**params)
 
         assert len(result) > 0
 
-    def test_query_sentinel2_using_gcs(self):
-        """
-        Testcase to check query_sentinel2_using_gcs method
-        :return:
-        """
+    def test_query_sentinel_2_using_s3(self):
         params = {"tile_code": "43QDB",
-                  "from_date": "2023-05-04"}
+                  "from_date": datetime.datetime.strptime("2023-05-04",
+                                                          "%Y-%m-%d").date()}
 
-        obj = S2L1CUrls()
-        result = obj._query_sentinel2_using_gcs(**params)
+        obj = S2L2AUrls()
+        s2_data = obj._query_sentinel_2_using_s3(**params)
 
-        assert len(result) > 0
-        assert "43QDB" in result[0]
+        assert "43QDB" in s2_data[0]
+        assert "L2A" in s2_data[0]
```

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.3.3/satsure_core/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.2/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.3.3/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.2
+Version: 0.3.3
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.2/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.3.3/satsure_core_test.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 README.md
 setup.py
 satsure_core/__init__.py
 satsure_core/satelite/__init__.py
 satsure_core/satelite/config.py
 satsure_core/satelite/core/__init__.py
 satsure_core/satelite/core/downloader.py
+satsure_core/satelite/core/extraction.py
 satsure_core/satelite/core/uploader.py
 satsure_core/satelite/gdal/__init__.py
-satsure_core/satelite/gdal/gdal_commands.py
+satsure_core/satelite/gdal/_extents.py
+satsure_core/satelite/gdal/_projection.py
+satsure_core/satelite/gdal/_raster_ops.py
+satsure_core/satelite/gdal/_resolution.py
 satsure_core/satelite/models/__init__.py
 satsure_core/satelite/models/s2_enum.py
 satsure_core/satelite/raster/__init__.py
 satsure_core/satelite/raster/raster.py
 satsure_core/satelite/sentinel2/__init__.py
 satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
 satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
@@ -24,31 +28,41 @@
 satsure_core/satelite/sentinel2/s2_l2a_urls.py
 satsure_core/satelite/sentinel2/band_stack/__init__.py
 satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
 satsure_core/satelite/sentinel2/indices/__init__.py
 satsure_core/satelite/sentinel2/indices/general_indices.py
 satsure_core/satelite/tests/__init__.py
 satsure_core/satelite/tests/conftest.py
+satsure_core/satelite/tests/core/__init__.py
+satsure_core/satelite/tests/core/test_extraction.py
 satsure_core/satelite/tests/gdal/__init__.py
 satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+satsure_core/satelite/tests/gdal/test_get_extents.py
 satsure_core/satelite/tests/gdal/test_get_projection.py
+satsure_core/satelite/tests/gdal/test_get_resolution.py
+satsure_core/satelite/tests/gdal/test_is_same_size.py
+satsure_core/satelite/tests/gdal/test_mask.py
 satsure_core/satelite/tests/gdal/test_reproject.py
+satsure_core/satelite/tests/gdal/test_reproject_raster.py
+satsure_core/satelite/tests/gdal/test_reproject_using_raster.py
+satsure_core/satelite/tests/gdal/test_reproject_vector.py
+satsure_core/satelite/tests/gdal/test_set_extents.py
+satsure_core/satelite/tests/gdal/test_set_resolution.py
 satsure_core/satelite/tests/raster/__init__.py
 satsure_core/satelite/tests/raster/test_mask_cloud.py
 satsure_core/satelite/tests/raster/test_merge.py
 satsure_core/satelite/tests/raster/test_normalised_difference_index.py
 satsure_core/satelite/tests/raster/test_offset_file.py
 satsure_core/satelite/tests/raster/test_resample_file.py
 satsure_core/satelite/tests/sentinel2/__init__.py
 satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
 satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
 satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
 satsure_core/satelite/tests/sentinel2/test_general_indices.py
 satsure_core/satelite/tests/sentinel2/test_get_tile.py
-satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
 satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
 satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
 satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
 satsure_core/satelite/tests/sentinel2/test_validate.py
 satsure_core/satelite/validators/__init__.py
 satsure_core/satelite/validators/check_shape_of_rid.py
 satsure_core_test.egg-info/PKG-INFO
```

