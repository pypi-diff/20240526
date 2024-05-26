# Comparing `tmp/satsure-core-test-0.3.4.tar.gz` & `tmp/satsure-core-test-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.3.4.tar", last modified: Sun May 26 14:46:31 2024, max compression
+gzip compressed data, was "satsure-core-test-0.3.5.tar", last modified: Sun May 26 16:16:42 2024, max compression
```

## Comparing `satsure-core-test-0.3.4.tar` & `satsure-core-test-0.3.5.tar`

### file list

```diff
@@ -1,92 +1,61 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.663819 satsure-core-test-0.3.4/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.4/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 14:46:31.663618 satsure-core-test-0.3.4/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.4/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.649558 satsure-core-test-0.3.4/satsure_core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.649785 satsure-core-test-0.3.4/satsure_core/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.650982 satsure-core-test-0.3.4/satsure_core/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       98 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6427 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      780 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/extraction.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.652323 satsure-core-test-0.3.4/satsure_core/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      342 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1338 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2984 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5930 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_raster_ops.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1103 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/gdal/_resolution.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.652695 satsure-core-test-0.3.4/satsure_core/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       46 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.653556 satsure-core-test-0.3.4/satsure_core/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      113 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8980 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.655917 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.656214 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2880 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3543 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.656696 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4026 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1481 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2702 2024-05-22 06:42:15.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3336 2024-05-26 14:33:40.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2940 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.657139 satsure-core-test-0.3.4/satsure_core/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1191 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.657502 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2501 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/core/test_extraction.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.659943 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1063 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_create_jpeg_image.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      328 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1360 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_projection.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      312 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_get_resolution.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      896 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_is_same_size.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1620 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_mask.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      748 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_raster.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1485 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_using_raster.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1412 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_reproject_vector.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1119 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_extents.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1058 2024-05-25 16:40:38.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/gdal/test_set_resolution.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.660899 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      993 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_mask_cloud.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      690 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_merge.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1097 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_normalised_difference_index.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      530 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_offset_file.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      645 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/raster/test_resample_file.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.662523 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      397 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      443 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1169 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1331 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1352 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      578 2024-05-26 14:02:21.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      335 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      984 2024-05-26 14:31:14.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      911 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.662803 satsure-core-test-0.3.4/satsure_core/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-22 06:34:45.000000 satsure-core-test-0.3.4/satsure_core/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:46:31.663399 satsure-core-test-0.3.4/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3547 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       13 2024-05-26 14:46:31.000000 satsure-core-test-0.3.4/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-26 14:46:31.663876 satsure-core-test-0.3.4/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      502 2024-05-26 14:45:10.000000 satsure-core-test-0.3.4/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.862421 satsure-core-test-0.3.5/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.5/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 16:16:42.862228 satsure-core-test-0.3.5/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-19 09:09:36.000000 satsure-core-test-0.3.5/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.852378 satsure-core-test-0.3.5/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.853119 satsure-core-test-0.3.5/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     6366 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.853443 satsure-core-test-0.3.5/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5973 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.853731 satsure-core-test-0.3.5/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.854053 satsure-core-test-0.3.5/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.856768 satsure-core-test-0.3.5/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.857245 satsure-core-test-0.3.5/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.857625 satsure-core-test-0.3.5/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2553 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3310 2024-05-26 16:15:54.000000 satsure-core-test-0.3.5/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.857879 satsure-core-test-0.3.5/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.860057 satsure-core-test-0.3.5/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.861197 satsure-core-test-0.3.5/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-26 14:55:28.000000 satsure-core-test-0.3.5/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-26 16:16:42.861999 satsure-core-test-0.3.5/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      536 2024-05-26 16:16:42.000000 satsure-core-test-0.3.5/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-26 16:16:42.000000 satsure-core-test-0.3.5/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-26 16:16:42.000000 satsure-core-test-0.3.5/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      147 2024-05-26 16:16:42.000000 satsure-core-test-0.3.5/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-26 16:16:42.000000 satsure-core-test-0.3.5/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-26 16:16:42.862470 satsure-core-test-0.3.5/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      609 2024-05-26 16:16:41.000000 satsure-core-test-0.3.5/setup.py
```

### Comparing `satsure-core-test-0.3.4/PKG-INFO` & `satsure-core-test-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.4
+Version: 0.3.5
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/config.py` & `satsure-core-test-0.3.5/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/core/downloader.py` & `satsure-core-test-0.3.5/satelite/core/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,14 @@
         :return:
         """
         request = self.retry_request(retries)
         response = request.get(source)
         if response.status_code == 200:
             with open(destination, 'wb') as f:
                 f.write(response.content)
-            print("download done for", source, destination)
-
             return True
 
         return False
 
     @staticmethod
     def validate_fields(tile_code: str, from_date: str,
                         download_path: PosixPath,
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/core/uploader.py` & `satsure-core-test-0.3.5/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/gdal/_raster_ops.py` & `satsure-core-test-0.3.5/satelite/gdal/gdal_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
+import re
 import subprocess
 from pathlib import Path, PosixPath
 from tempfile import NamedTemporaryFile
-from typing import Dict, Optional, Tuple, Union
+from typing import Optional, Union, Tuple,Dict
 
-from osgeo import gdal
-from osgeo.gdalconst import GA_ReadOnly
-
-from satsure_core.satelite.core import Downloader
+from satelite.core import Downloader
 
 
 def create_jpeg_image(
-    input_file: PosixPath,
-    output_file: Optional[str] = None,
-    bands_position: Tuple[int, int, int] = (3, 2, 1),
-    quality: int = 10,
-    target_resolution: int = 100,
-):
+        input_file: PosixPath,
+        output_file: Optional[str] = None,
+        bands_position: Tuple[int, int, int] = (3, 2, 1),
+        quality: int = 10,
+        target_resolution: int = 100):
     """Generates JPG image for a given tif
 
     Args:
         input_file (PosixPath): Path of the input file
         output_file (Optional[PosixPath], optional): Output path for the file. If not proivded, defaults to input file by changing extension. Defaults to None.
         quality (int): Compression ratio. (how much you want to compress)
         bands_position (Iterable[int, int, int], optional): List of rgb bands to use. Defaults to (3, 2, 1).
@@ -39,55 +36,56 @@
         f"QUALITY={int(quality)}",
         f"{input_file}",
         f"{output_file}",
     )
     subprocess.run(command, shell=False, capture_output=True)
 
 
-def is_same_size(raster_path_1: str, raster_path_2: str) -> bool:
+def reproject(
+        input_file: PosixPath,
+        output_file: PosixPath,
+        target_crs: str) -> None:
+    """
+     reproject the given polygon file
+    :param input_file:
+    :param output_file:
+    :param target_crs:
+    :return:
     """
-    Compare size (width, height) of two rasters
+    command = (
+        "gdalwarp", "-t_srs", f"{target_crs}", f"{input_file}",
+        f"{output_file}")
+    subprocess.run(command, shell=False, capture_output=True)
 
-    :param raster_path_1: Path of first raster
-    :param raster_path_2: Path of second raster
-    :returns: Boolean value
-    """
-    raster_1 = gdal.Open(raster_path_1, GA_ReadOnly)
-    raster_2 = gdal.Open(raster_path_2, GA_ReadOnly)
-    return (raster_1.RasterXSize, raster_1.RasterYSize) == (
-        raster_2.RasterXSize,
-        raster_2.RasterYSize,
-    )
 
+def get_projection(file_path: str) -> str:
+    """
+    Function to get projection of file (Vector / Raster)
+    Currently supports only EPSG based projections
+    :param file_path:
+    :return:
+    """
+    command = f"gdalsrsinfo {file_path} -e"
+    projection_str = subprocess.check_output(
+        command, stderr=subprocess.STDOUT, shell=True)
+
+    if "error" in projection_str.decode("utf-8")[:20].lower():
+        raise Exception(projection_str.decode("utf-8"))
+
+    projection_code = re.findall(rb"\nEPSG:(.+?)\n", projection_str)
+    if not projection_code:
+        raise Exception(
+            "Cannot find projection, currently supports only " "EPSG based projections"
+        )
 
-def mask(
-    raster_path: str,
-    mask_raster_path: str,
-    output_path: str,
-    no_data_value: int = 0,
-) -> None:
-    """
-    Mask a specified raster using another raster
-
-    :param raster_path: Path of raster that needs to be masked
-    :param mask_raster_path: Path of mask raster
-    :param output_path: Path of output raster
-    :param no_data_value: Value to use for `No Data` pixels (Defaults to 0)
-    """
-    command = f'gdal_calc.py -A {raster_path} -B {mask_raster_path} --outfile={output_path} --calc="A*B" --NoDataValue={no_data_value}'
-
-    subprocess.check_output(command, stderr=subprocess.STDOUT, shell=True)
-
-
-def clip_with_shp(
-    input_file: PosixPath,
-    shp_path: PosixPath,
-    output_folder: PosixPath,
-    output_file: Union[str, None] = None,
-) -> PosixPath:
+    return f"EPSG:{projection_code[0].decode('utf-8')}"
+
+
+def clip_with_shp(input_file: PosixPath, shp_path: PosixPath,
+                  output_folder: PosixPath, output_file: Union[str, None] = None) -> PosixPath:
     """
     Function to clip a raster file using a shapefile
 
     Parameters:
         input_file          - str, path to the raster file to be clipped
         shpFile             - str, path to the shapefile by which input_file should
                               be clipped
@@ -102,76 +100,72 @@
     suffix = input_file.split(".")[-1]
     s3_temp_file = False
     if input_file[:5] == "s3://":
         s3_temp_file = True
         input_file_local = NamedTemporaryFile(delete=False, suffix=f".{suffix}")
         Downloader().download_object_from_s3(input_file, input_file_local.name)
         if suffix == "jpg":
-            Downloader().download_object_from_s3(
-                f"{input_file}.aux.xml", f"{input_file_local.name}.aux.xml"
-            )
+            Downloader().download_object_from_s3(f"{input_file}.aux.xml",
+                                                 f"{input_file_local.name}.aux.xml")
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
-        "gdalwarp",
-        "-q",
-        "-srcnodata",
-        "0",
-        "-dstnodata",
-        "0",
-        "-overwrite",
-        f"{input_file}",
-        f"{outFile}",
-        "-cutline",
-        f"{shp_path}",
-        f"-crop_to_cutline",
-        "-co",
-        "COMPRESS=LZW",
+        "gdalwarp", "-q", "-srcnodata", "0", "-dstnodata", "0", "-overwrite",
+        f"{input_file}", f"{outFile}", "-cutline", f"{shp_path}",
+        f"-crop_to_cutline", "-co", "COMPRESS=LZW")
+    resp = subprocess.run(
+        command,
+        shell=False,
+        capture_output=True
     )
-    resp = subprocess.run(command, shell=False, capture_output=True)
     if s3_temp_file:
         input_file_local.close()
         input_file.unlink()
         if suffix == "jpg":
             Path(f"{input_file_local.name}.aux.xml").unlink()
     if resp.returncode != 0:
         raise ValueError()
 
     return outFile
 
 
-def get_file_info(input_file: PosixPath, crs: bool = False, stats: bool = True) -> Dict:
+def get_file_info(input_file: PosixPath, crs: bool = False,
+                  stats: bool = True) -> Dict:
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
-            result.update({"crs": resp.stdout.decode("utf-8").replace("\n", "")})
+            result.update({"crs": resp.stdout.decode('utf-8').replace('\n', '')})
     if stats:
         command = ("rio", "info", f"--stats", f"{input_file}")
         resp = subprocess.run(command, shell=False, capture_output=True)
         if resp.returncode == 0:
             stats = resp.stdout.decode("utf-8").replace("\n", "").split(" ")
-            result.update(
-                {"stats": {"min": stats[0], "max": stats[1], "mean": stats[2]}}
-            )
+            result.update({
+                "stats": {
+                    "min": stats[0],
+                    "max": stats[1],
+                    "mean": stats[2]
+                }
+            })
 
     return result
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/raster/raster.py` & `satsure-core-test-0.3.5/satelite/raster/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     :param cloud_mask_bands:
     :param cloud_mask_threshold:
     :param target_value:
     :param level:
     :return:
     """
     if len(cloud_mask_bands) != len(cloud_mask_threshold):
-        raise ValueError("cloud_mask_threshold and cloud_mask_bands count is not same")
+        return False
 
     output = Path(output_folder) / output_name
     Path(output_folder).mkdir(exist_ok=True, parents=True)
 
     img_A = rio.open(cloud_mask_bands[0])
     img_B = rio.open(cloud_mask_bands[1])
     img_C = rio.open(input_file)
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.3.5/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path, PosixPath
 from typing import Tuple
 
-from satsure_core.satelite.gdal import create_jpeg_image
-from satsure_core.satelite.raster import merge
+from satelite.gdal.gdal_commands import create_jpeg_image
+from satelite.raster.raster import merge
 
 
 class GenerateBandStack:
     """
     Stack bands based band input
     """
     BANDS = ("B02", "B03", "B04", "B08", "B12")
@@ -68,9 +68,7 @@
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option="COMPRESS=LZW",
                 )
                 if create_jpeg and fcc_path:
                     create_jpeg_image(fcc_path,
                                       bands_position=rgb_bands_position)
-
-        print("Create FCC process done")
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.3.5/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.3.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.3.5/satelite/sentinel2/get_tiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 from os import environ
-from typing import List
 
 import fiona
 from fiona.session import AWSSession
 from sqlalchemy import text
 
-from satsure_core.satelite.config import DBSession
+from satelite.config import DBSession
 
 
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

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.3.5/satelite/sentinel2/indices/general_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path, PosixPath
 from typing import Tuple
 
-from satsure_core.satelite.raster import create_normalised_difference_index, \
+from satelite.raster.raster import create_normalised_difference_index, \
     mask_cloud
 
 
 class GeneralIndices:
     """
      Create indices based on bands
     """
@@ -93,9 +93,7 @@
                 index_path,
                 cloud_mask_output_folder,
                 output_name=f"{date}_{unique_tile}_IS1{band_combination_id}02{file_version}.tif",
                 cloud_mask_bands=cloud_mask_bands_path,
                 cloud_mask_threshold=cloud_mask_threshold,
                 level=self.level
             )
-
-        print("Normalized process is done")
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.3.5/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path, PosixPath
 from typing import List
 
-from satsure_core.satelite.raster import merge
+from satelite.raster.raster import merge
 
 
 class MosaicSameBands:
     """
     Stack similar bands on same date
     """
     BANDS = ("B02", "B03", "B04", "B05", "B08", "B12",)
@@ -46,27 +46,24 @@
                     continue
                 files.sort()
                 date = files[0].stem.split(file_name_delimiter)[
                            date_identifier_position][:8]
                 creation_option = None
                 if input_file_format == "tif":
                     creation_option = "COMPRESS=LZW"
-                output_file_name = f"{date}_{unique_tile}_{band}.{input_file_format}"
                 merge(
                     files,
                     output_folder=str(self.output_folder),
-                    output_name=output_file_name,
+                    output_name=f"{date}_{unique_tile}_{band}.{input_file_format}",
                     output_nodata_value=0,
                     keep_separate=False,
                     output_format=None,
                     output_datatype=None,
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option=creation_option
                 )
 
-                print("Output file name", output_file_name)
                 for file in files:
-                    if file.name == output_file_name:
+                    if file.name == f"{date}_{unique_tile}_{band}.{input_file_format}":
                         continue
-                    print("Deleting duplicate files", file.name)
                     file.unlink()
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.3.5/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.3.5/satelite/sentinel2/s2_l1c_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime
+import json
 import re
+
 from pathlib import PosixPath
 from typing import List, Tuple
 
 from google.cloud import storage
 from google.oauth2 import service_account
-from airflow.models import Variable
-from satsure_core.satelite.config import GCP_BASE_URL, key_json, S3_L1C_BUCKET
-from satsure_core.satelite.core import Downloader
-from satsure_core.satelite.models.s2_enum import ProcessingLevel, BaseBands
+
+from satelite.config import GCP_BASE_URL, key_json, S3_L1C_BUCKET
+from satelite.core.downloader import Downloader
+from satelite.models.s2_enum import ProcessingLevel, BaseBands
 
 
 class S2L1CUrls:
     """
         This class used to fetch L1C urls from given tile code and from date
     """
 
@@ -26,16 +28,17 @@
         tile codes and available dates from the GCS bucket "gcp-public-data-sentinel-2."
         The manifest files provide metadata for Sentinel-2 scenes.
 
         :param tile_code:
         :param from_date:
         :return:
         """
-        gcp = Variable.get("gcp_value")
-        credentials = service_account.Credentials.from_service_account_info(gcp)
+        credentials = service_account.Credentials.from_service_account_file(
+            key_json)
+        credentials = json.loads(credentials)
         gcs = storage.Client(credentials=credentials)
         gcs_bucket = gcs.get_bucket(S3_L1C_BUCKET)
         prefix = f"tiles/{tile_code[:2]}/{tile_code[2]}/{tile_code[-2:]}/"
         blobs = gcs_bucket.list_blobs(
             max_results=10000, prefix=prefix, delimiter="/")
         next(blobs, ...)
         date = str(from_date).replace("-", "")
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.3.5/satelite/sentinel2/s2_l2a_urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from pathlib import PosixPath
 from subprocess import PIPE, Popen
 from typing import List, Tuple
 
-from satsure_core.satelite.config import S3_L2A_BUCKET, S3_L2A_PREFIX
-from satsure_core.satelite.models.s2_enum import ProcessingLevel, BaseBands
-from satsure_core.satelite.core import Downloader
+from satelite.config import S3_L2A_BUCKET, S3_L2A_PREFIX
+from satelite.models.s2_enum import ProcessingLevel, BaseBands
+from satelite.core.downloader import Downloader
 
 
 class S2L2AUrls:
     """
         This class used to fetch L2A urls from given tile code and from date
     """
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/conftest.py` & `satsure-core-test-0.3.5/satelite/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,13 +28,7 @@
     return polygon
 
 
 @pytest.fixture
 def datadir(tmp_path):
     """Fixture to provide access to the test data directory."""
     return Path(__file__).parent / "raster" / "testdata"
-
-
-@pytest.fixture
-def extraction_testdata_dir():
-    """Provide the directory containing test data for extraction"""
-    return Path(__file__).parent / "core" / "testdata" / "extraction"
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 from pathlib import Path
 
 import pytest
 
-from satsure_core.satelite.sentinel2.band_stack import GenerateBandStack
+from satelite.sentinel2.band_stack.generate_band_stack import GenerateBandStack
 
 
 @pytest.mark.skip("need to do upload tif files")
 class TestGenerateBandStack:
 
     def test_create_fcc(self):
         """
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_general_indices.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 from pathlib import Path
 
 import pytest
 
-from satsure_core.satelite.sentinel2.indices.general_indices import GeneralIndices
+from satelite.sentinel2.indices.general_indices import GeneralIndices
 
 
 @pytest.mark.skip("need to add tiff files")
 class TestGeneralIndices:
     """Testcase for General Indices """
 
     def test_general_indices(self):
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_get_tile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from satsure_core.satelite.sentinel2 import GetTiles
-from satsure_core.satelite.config import DBSession
+from satelite.sentinel2 import GetTiles
+from satelite.config import DBSession
 
 
 class TestGetTiles:
 
     def test_get_tile_from_geom(self, monkeypatch):
         """testcase to get tile from geom"""
         geom = [{
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,33 @@
+import datetime
 from pathlib import Path
 
-import pytest
+from satelite.sentinel2 import S2L2AUrls
 
-from satsure_core.satelite.sentinel2 import S2L1CUrls
 
+class TestS2L2AUrls:
 
-class TestS2L1CUrls:
-
-    @pytest.mark.skip(reason="Need gcp.json")
     def test_get_urls(self, monkeypatch):
         """
             Testcase to check get_urls data
         :param monkeypatch:
         :return:
         """
-        params = {
-            "tile_code": "43QDB",
-            "from_date": "2023-05-04",
-            "download_path": Path("sample/temp"),
-        }
+        params = {"tile_code": "43QDB",
+                  "from_date": "2023-05-04",
+                  "download_path": Path("sample/temp")}
 
-        obj = S2L1CUrls()
+        obj = S2L2AUrls()
         result = obj.get_urls(**params)
 
         assert len(result) > 0
 
-    @pytest.mark.skip(reason="Need gcp.json")
-    def test_query_sentinel2_using_gcs(self):
-        """
-        Testcase to check query_sentinel2_using_gcs method
-        :return:
-        """
-        params = {"tile_code": "43QDB", "from_date": "2023-05-04"}
+    def test_query_sentinel_2_using_s3(self):
+        params = {"tile_code": "43QDB",
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

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-import datetime
 from pathlib import Path
 
-from satsure_core.satelite.sentinel2 import S2L2AUrls
+from satelite.sentinel2 import S2L1CUrls
 
 
-class TestS2L2AUrls:
+class TestS2L1CUrls:
 
     def test_get_urls(self, monkeypatch):
         """
             Testcase to check get_urls data
         :param monkeypatch:
         :return:
         """
         params = {"tile_code": "43QDB",
                   "from_date": "2023-05-04",
                   "download_path": Path("sample/temp")}
 
-        obj = S2L2AUrls()
+        obj = S2L1CUrls()
         result = obj.get_urls(**params)
 
         assert len(result) > 0
 
-    def test_query_sentinel_2_using_s3(self):
+    def test_query_sentinel2_using_gcs(self):
+        """
+        Testcase to check query_sentinel2_using_gcs method
+        :return:
+        """
         params = {"tile_code": "43QDB",
-                  "from_date": datetime.datetime.strptime("2023-05-04",
-                                                          "%Y-%m-%d").date()}
+                  "from_date": "2023-05-04"}
 
-        obj = S2L2AUrls()
-        s2_data = obj._query_sentinel_2_using_s3(**params)
+        obj = S2L1CUrls()
+        result = obj._query_sentinel2_using_gcs(**params)
 
-        assert "43QDB" in s2_data[0]
-        assert "L2A" in s2_data[0]
+        assert len(result) > 0
+        assert "43QDB" in result[0]
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.3.5/satelite/tests/sentinel2/test_validate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import pytest
 
-from satsure_core.satelite.core import Downloader
+from satelite.core.downloader import Downloader
 
 
 class TestDownloader:
 
     def test_validate_fields(self):
         """Testcase to validate input params
         """
```

### Comparing `satsure-core-test-0.3.4/satsure_core/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.3.5/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.3.4/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.3.5/satsure_core_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.3.4
+Version: 0.3.5
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: boto3
 Requires-Dist: fiona
```

