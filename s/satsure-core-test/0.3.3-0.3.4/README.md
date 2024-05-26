# Comparing `tmp/satsure-core-test-0.3.3.tar.gz` & `tmp/satsure-core-test-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.3.3.tar", last modified: Sun May 26 13:40:48 2024, max compression
+gzip compressed data, was "satsure-core-test-0.3.4.tar", last modified: Sun May 26 14:46:31 2024, max compression
```

## Comparing `satsure-core-test-0.3.3.tar` & `satsure-core-test-0.3.4.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.896773 satsure-core-test-0.3.3/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.3/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 13:40:48.896565 satsure-core-test-0.3.3/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.3/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.879595 satsure-core-test-0.3.3/satsure_core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.879805 satsure-core-test-0.3.3/satsure_core/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.881157 satsure-core-test-0.3.3/satsure_core/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       98 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      780 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/extraction.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.882634 satsure-core-test-0.3.3/satsure_core/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      342 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1338 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5930 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_raster_ops.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1103 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/gdal/_resolution.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.883168 satsure-core-test-0.3.3/satsure_core/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.883938 satsure-core-test-0.3.3/satsure_core/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.886712 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.887773 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3217 2024-05-25 16:40:08.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.888210 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-25 16:40:08.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3279 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.888652 satsure-core-test-0.3.3/satsure_core/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1191 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.889094 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2501 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/core/test_extraction.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.891842 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1063 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      328 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1360 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      312 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_resolution.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      896 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_is_same_size.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1620 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_mask.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_raster.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1485 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1412 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_vector.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1119 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1058 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_resolution.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.893575 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_mask_cloud.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_merge.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_offset_file.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_resample_file.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.895369 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.895676 satsure-core-test-0.3.3/satsure_core/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.3/satsure_core/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 13:40:48.896318 satsure-core-test-0.3.3/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3481 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-26 13:40:48.000000 satsure-core-test-0.3.3/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-26 13:40:48.896829 satsure-core-test-0.3.3/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-26 13:38:31.000000 satsure-core-test-0.3.3/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.663819 satsure-core-test-0.3.4/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.4/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 14:46:31.663618 satsure-core-test-0.3.4/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.4/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.649558 satsure-core-test-0.3.4/satsure_core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.649785 satsure-core-test-0.3.4/satsure_core/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.650982 satsure-core-test-0.3.4/satsure_core/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       98 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      780 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/extraction.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.652323 satsure-core-test-0.3.4/satsure_core/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      342 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1338 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5930 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_raster_ops.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1103 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_resolution.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.652695 satsure-core-test-0.3.4/satsure_core/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.653556 satsure-core-test-0.3.4/satsure_core/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.655917 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.656214 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3543 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.656696 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1481 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3336 2024-05-26 14:33:40.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.657139 satsure-core-test-0.3.4/satsure_core/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1191 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.657502 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2501 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/test_extraction.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.659943 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1063 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      328 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1360 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_projection.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      312 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_resolution.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      896 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_is_same_size.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1620 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_mask.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_raster.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1485 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1412 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_vector.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1119 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_extents.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1058 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_resolution.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.660899 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_mask_cloud.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_merge.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_offset_file.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_resample_file.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.662523 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      578 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      984 2024-05-26 14:31:14.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.662803 satsure-core-test-0.3.4/satsure_core/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.663399 satsure-core-test-0.3.4/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3547 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-26 14:46:31.663876 satsure-core-test-0.3.4/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-26 14:45:10.000000 satsure-core-test-0.3.4/setup.py
```

### Comparing `satsure-core-test-0.3.3/PKG-INFO` & `satsure-core-test-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.3
+Version: 0.3.4
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/config.py` & `satsure-core-test-0.3.4/satsure_core/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/core/downloader.py` & `satsure-core-test-0.3.4/satsure_core/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/core/extraction.py` & `satsure-core-test-0.3.4/satsure_core/satelite/core/extraction.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/core/uploader.py` & `satsure-core-test-0.3.4/satsure_core/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/gdal/_extents.py` & `satsure-core-test-0.3.4/satsure_core/satelite/gdal/_extents.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/gdal/_projection.py` & `satsure-core-test-0.3.4/satsure_core/satelite/gdal/_projection.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/gdal/_raster_ops.py` & `satsure-core-test-0.3.4/satsure_core/satelite/gdal/_raster_ops.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/gdal/_resolution.py` & `satsure-core-test-0.3.4/satsure_core/satelite/gdal/_resolution.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/raster/raster.py` & `satsure-core-test-0.3.4/satsure_core/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/get_tiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 from os import environ
+from typing import List
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
 from satsure_core.satelite.config import DBSession
 
 
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.db = DBSession.create()
 
-    def fetch_tile_from_db(self, sql_query, geom_):
+    def fetch_tile_from_db(self, sql_query: text, geom_list: List) -> List:
         """
             Fetch tile from database
         :param sql_query:
-        :param geom_:
+        :param geom_list:
         :return:
         """
 
-        result = self.db.execute(sql_query,
-                                 {"geojson_geometry": str(geom_)})
+        result = self.db.execute(
+            sql_query,
+            {
+                "minx": geom_list['minx'][0],
+                "miny": geom_list['miny'][0],
+                "maxx": geom_list['maxx'][0],
+                "maxy": geom_list['maxy'][0],
+            },
+        )
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
         """
         tile_list = set()
         sql_query = text(
-            f"""SELECT tile FROM tileids WHERE ST_Intersects( geometry,
-                                            ST_GeomFromGeoJSON(:geojson_geometry)) """
-        )
-
-        for geom_ in geom_list:
-            rows = self.fetch_tile_from_db(sql_query, geom_)
-            for row in rows:
-                tile_list.add(row[0])
+            """SELECT tile FROM tileids
+                            WHERE ST_Intersects(
+                                geometry,
+                                ST_MakeEnvelope(:minx, :miny, :maxx, :maxy, 4326) -- 4326 is the SRID, adjust if needed
+                            )
+                            """)
+
+        rows = self.fetch_tile_from_db(sql_query, geom_list)
+        for row in rows:
+            tile_list.add(row[0])
 
         tile_list = list(tile_list)
         self.db.close()
 
         return tile_list
 
     def get_tile_from_rids(self, rids: list, shape_path: str):
```

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l1c_urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import re
 from pathlib import PosixPath
 from typing import List, Tuple
 
 from google.cloud import storage
 from google.oauth2 import service_account
-
+from airflow.models import Variable
 from satsure_core.satelite.config import GCP_BASE_URL, key_json, S3_L1C_BUCKET
 from satsure_core.satelite.core import Downloader
 from satsure_core.satelite.models.s2_enum import ProcessingLevel, BaseBands
 
 
 class S2L1CUrls:
     """
@@ -26,16 +26,16 @@
         tile codes and available dates from the GCS bucket "gcp-public-data-sentinel-2."
         The manifest files provide metadata for Sentinel-2 scenes.
 
         :param tile_code:
         :param from_date:
         :return:
         """
-        credentials = service_account.Credentials.from_service_account_file(
-            key_json)
+        gcp = Variable.get("gcp_value")
+        credentials = service_account.Credentials.from_service_account_info(gcp)
         gcs = storage.Client(credentials=credentials)
         gcs_bucket = gcs.get_bucket(S3_L1C_BUCKET)
         prefix = f"tiles/{tile_code[:2]}/{tile_code[2]}/{tile_code[-2:]}/"
         blobs = gcs_bucket.list_blobs(
             max_results=10000, prefix=prefix, delimiter="/")
         next(blobs, ...)
         date = str(from_date).replace("-", "")
```

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/conftest.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/core/test_extraction.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/core/test_extraction.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_get_projection.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_projection.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_is_same_size.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_is_same_size.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_mask.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_mask.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_raster.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_reproject_vector.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_vector.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_extents.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_extents.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/gdal/test_set_resolution.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_resolution.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_mask_cloud.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_mask_cloud.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_merge.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_merge.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_normalised_difference_index.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_normalised_difference_index.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_offset_file.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_offset_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/raster/test_resample_file.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_resample_file.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.3.4/satsure_core/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.3/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.3.4/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.3
+Version: 0.3.4
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.3/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.3.4/satsure_core_test.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 satsure_core/satelite/tests/raster/test_resample_file.py
 satsure_core/satelite/tests/sentinel2/__init__.py
 satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
 satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
 satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
 satsure_core/satelite/tests/sentinel2/test_general_indices.py
 satsure_core/satelite/tests/sentinel2/test_get_tile.py
+satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
 satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
 satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
 satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
 satsure_core/satelite/tests/sentinel2/test_validate.py
 satsure_core/satelite/validators/__init__.py
 satsure_core/satelite/validators/check_shape_of_rid.py
 satsure_core_test.egg-info/PKG-INFO
```

